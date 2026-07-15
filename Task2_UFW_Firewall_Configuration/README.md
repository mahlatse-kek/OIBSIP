## Steps On How To Complete Task 2 (UFW Firewall)

Step 1: You need a Linux environment

UFW is Linux-only.

Step 2:	Open PowerShell as Administrator (right-click Start → “Windows PowerShell (Admin)” or “Terminal (Admin)”).

Step 3: Run This Code

wsl --install

Step 4: Restart Your Laptop When Prompted

Step 5: After restart, Ubuntu should launch automatically (or search “Ubuntu” in the Start menu). First launch will ask you to create a username and password for your Linux user if you did not log in before remember these, you will need the password for sudo commands.

## Steps Once You Are In The Ubuntu Terminal

Step 1: sudo apt update && sudo apt upgrade -y

Step 2: Run The Task 2 Command

**Install UFW**
sudo apt install ufw -y

**Enable UFW**
sudo ufw enable

(It will warn you about disrupting SSH connections, type y to confirm, this is fine in WSL.)

Step 3:

**Allow SSH**
sudo ufw allow ssh

**Deny HTTP**
sudo ufw deny http

**Two Extra Rules**
sudo ufw allow https
sudo ufw deny from 192.168.1.100

**Check Status - SCREENSHOT THIS**
sudo ufw status verbose

Take a screenshot after each command runs and definitely one of the final status verbose output, that’s a required deliverable.

## A Way To Test It In WSL.

**1. Install a simple test tool (usually already there)**
python3 --version

**2. Start a basic web server on port 80 (needs sudo since it's a low port)**
sudo python3 -m http.server 80 &

**3. Try to reach it — this should be BLOCKED by your "deny http" rule**
curl http://localhost

**4. Now compare against an allowed port, to show the firewall is selectively working**
sudo python3 -m http.server 8000 &
curl http://localhost:8000

**5. Stop both test servers when done**
sudo kill %1 %2

## Testing Environment Note:

This task was completed using WSL2 (Windows Subsystem for Linux) running Ubuntu, since a full Linux VM wasn’t available. WSL2 uses its own internal networking stack so blocked traffic was verified by attempting to reach a local test server (python3 -m http.server) on the denied port (80) versus an allowed port (8000) from within the same WSL instance, using curl. The denied port returned a connection failure while the allowed port served content normally, confirming the UFW rule was correctly enforced.

# 🎮 Fedora Terminal RPG: The Handbook

> **Welcome, Player.**
> You have just logged into **Fedora Linux**, a powerful operating system where the keyboard is mightier than the mouse. Your quest is to master the **Terminal**—the command center of your digital world.
>
> Each **Level** below grants you new powers (commands). Complete the **Missions** to gain XP and level up.

---

## 🗺️ Quest Map (Table of Contents)

| Level | Title | Skill |
|:-----:|:------|:------|
| 1 | First Steps in the Dark | Navigation |
| 2 | The Builder | File Management |
| 3 | The Scribe | Text Editing |
| 4 | The Summoner | Installing Software |
| 5 | The Oracle | System Monitoring |
| 6 | The Signalman | Networking |
| 7 | The Artificer | External Media (USB) |
| 8 | The Seeker | Search & Grep |
| 9 | The Void Walker | Remote Access (SSH & Curl) |
| 10 | The Automaton | Bash Scripting |
| 11 | The Overlord | Systemd Services |
| 12 | God Mode | Power User Tricks |
| ★ | Bonus Level | Permissions & Ownership |

---

## Level 1: First Steps in the Dark
*Navigation & Orientation*

The terminal is a dark void. You must learn to see where you are.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `whoami` | Reveal your identity. |
| `pwd` | **P**rint **W**orking **D**irectory. Where are you? |
| `ls` | **L**i**s**t. Look around. What files are here? |
| `ls -la` | Long format + hidden files. Full details. |
| `cd [dir]` | **C**hange **D**irectory. Teleport to a new location. |
| `cd ..` | Retreat one step back. |
| `cd ~` | Teleport home. |
| `cd -` | Return to previous location. |
| `clear` | Wipe the screen. Fresh start. |

> 💡 **Pro Tip**: Press `Tab` to auto-complete paths and commands!

> 🛡️ **Loot Acquired**: `whoami`, `pwd`, `ls`, `cd`, `clear`

### ⚔️ Mission
1. Open your terminal (`Super` key → type "Terminal").
2. Find out who you are: `whoami`.
3. Check where you are: `pwd`.
4. List all files including hidden ones: `ls -la`.
5. Enter the `/etc` dungeon: `cd /etc` and look around.
6. Teleport back home: `cd ~`.

---

## Level 2: The Builder
*File Management*

You can now move. It is time to create and destroy.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `mkdir [name]` | **M**a**k**e **Dir**ectory. Create a new folder. |
| `mkdir -p a/b/c` | Create nested folders in one command. |
| `touch [file]` | Summon an empty file into existence. |
| `cp [src] [dest]` | **C**o**p**y. Clone an object. |
| `cp -r [dir] [dest]` | Copy a directory recursively. |
| `mv [src] [dest]` | **M**o**v**e or rename an object. |
| `rm [file]` | **R**e**m**ove. Destroy a file. |
| `rm -r [dir]` | Destroy a folder and all contents. ⚠️ **No undo!** |
| `cat [file]` | Display file contents. |
| `less [file]` | Scroll through file (press `q` to quit). |
| `head -n 10 [file]` | Show first 10 lines. |
| `tail -n 10 [file]` | Show last 10 lines. |

> 🛡️ **Loot Acquired**: `mkdir`, `touch`, `cp`, `mv`, `rm`, `cat`, `less`, `head`, `tail`

### ⚔️ Mission
1. Create a directory: `mkdir QuestLog`.
2. Enter it: `cd QuestLog`.
3. Create a file: `touch dragon.txt`.
4. Write something: `echo "A fierce dragon appeared!" > dragon.txt`.
5. Read it: `cat dragon.txt`.
6. Rename it: `mv dragon.txt slain_dragon.txt`.
7. Delete it: `rm slain_dragon.txt`.

---

## Level 3: The Scribe
*Text Editing — [Critical Skill]*

A true Linux wizard writes their own scrolls. You need a text editor.

### 🔮 The Weapon: Nano

`nano` is your starter sword. Simple and reliable.

```bash
nano [filename]
```

**Controls:**
| Key | Action |
|:----|:-------|
| `Ctrl + O` | Save (Write **O**ut) |
| `Ctrl + X` | E**x**it |
| `Ctrl + K` | Cut line |
| `Ctrl + U` | Paste line |
| `Ctrl + W` | Search (Where is) |

> 💡 **Pro Tip**: The `^` symbol in nano means `Ctrl`.

> 🛡️ **Loot Acquired**: `nano`, `cat`

### ⚔️ Mission
1. Create a new file: `nano spellbook.txt`.
2. Type: *"I am learning the ways of Fedora."*
3. Save (`Ctrl+O`, then `Enter`) and Exit (`Ctrl+X`).
4. Read it: `cat spellbook.txt`.

---

## Level 4: The Summoner
*Software Management (DNF5)*

Fedora 43 grants you the power of **DNF5**. Use it to summon new tools.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `sudo dnf update` | Upgrade all tools to latest versions. |
| `sudo dnf install [pkg]` | Summon a new application. |
| `sudo dnf remove [pkg]` | Banish an application. |
| `dnf search [keyword]` | Search the archives for a tool. |
| `dnf info [pkg]` | Get details about a package. |
| `dnf list installed` | List all installed packages. |
| `sudo dnf autoremove` | Remove orphaned dependencies. |

> 🛡️ **Loot Acquired**: `dnf update`, `dnf install`, `dnf remove`, `dnf search`

### ⚔️ Mission
1. Update your system: `sudo dnf update`.
2. Summon the legendary cow: `sudo dnf install cowsay`.
3. Cast the spell: `cowsay "Fedora Rocks!"`.
4. Try a fortune: `sudo dnf install fortune-mod && fortune | cowsay`.

---

## Level 5: The Oracle
*System Monitoring*

See the invisible spirits (processes) running your machine.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `top` | Real-time process viewer. |
| `htop` | Better `top` (install: `sudo dnf install htop`). |
| `ps aux` | Snapshot of all running processes. |
| `kill [PID]` | Terminate a process by ID. |
| `killall [name]` | Terminate all processes by name. |
| `df -h` | Disk space usage (human-readable). |
| `du -sh [dir]` | Folder size. |
| `free -h` | RAM usage. |
| `uptime` | How long has the system been running? |

> 🛡️ **Loot Acquired**: `top`, `htop`, `ps`, `kill`, `df`, `du`, `free`, `uptime`

### ⚔️ Mission
1. Install htop: `sudo dnf install htop`.
2. Run it: `htop`.
3. Find the process using the most CPU (it's at the top!).
4. Press `q` to quit.
5. Check disk space: `df -h`.
6. Check RAM: `free -h`.

---

## Level 6: The Signalman
*Networking*

Connect your console to the vast network.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `ip addr` | Show your IP addresses. |
| `ip link` | Show network interfaces. |
| `ping [host]` | Test connectivity (e.g., `ping google.com`). |
| `nmcli device status` | Show all network devices. |
| `nmcli device wifi list` | Scan for Wi-Fi networks. |
| `nmcli device wifi connect [SSID] password [PASS]` | Connect to Wi-Fi. |
| `nmcli connection show` | Show saved connections. |
| `ss -tuln` | Show listening ports. |

> 🛡️ **Loot Acquired**: `ip`, `ping`, `nmcli`, `ss`

### ⚔️ Mission
1. Check your IP address: `ip addr | grep inet`.
2. Ping Google: `ping -c 4 google.com`.
3. List Wi-Fi networks: `nmcli device wifi list`.

---

## Level 7: The Artificer
*External Media (USB)*

Master the art of mounting external drives.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `lsblk` | List all block devices (disks). |
| `sudo fdisk -l` | Detailed disk information. |
| `sudo mount /dev/sdX1 /mnt` | Mount a drive. |
| `sudo umount /mnt` | Safely eject/unmount. |
| `df -h` | Verify mount and check space. |

> ⚠️ **Warning**: Always `umount` before unplugging!

> 🛡️ **Loot Acquired**: `lsblk`, `mount`, `umount`, `fdisk`

### ⚔️ Mission
1. Plug in a USB drive.
2. Identify it: `lsblk` (look for a new device, usually `sdb`).
3. Create a mount point: `sudo mkdir -p /mnt/usb`.
4. Mount it: `sudo mount /dev/sdb1 /mnt/usb`.
5. Access it: `ls /mnt/usb`.
6. Unmount safely: `sudo umount /mnt/usb`.

---

## Level 8: The Seeker
*Search & Grep*

Finding a needle in a haystack is easy with these spells.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `grep "pattern" [file]` | Search for text in a file. |
| `grep -i "pattern" [file]` | Case-insensitive search. |
| `grep -r "pattern" [dir]` | Search recursively in directories. |
| `grep -n "pattern" [file]` | Show line numbers. |
| `find [path] -name "*.txt"` | Find files by name. |
| `find [path] -type f -size +10M` | Find files larger than 10MB. |
| `locate [filename]` | Fast file search (needs `mlocate`). |
| `which [command]` | Find where a command lives. |

> 🛡️ **Loot Acquired**: `grep`, `find`, `locate`, `which`

### ⚔️ Mission
1. Search for "error" in system logs: `sudo grep -i "error" /var/log/messages`.
2. Find all `.conf` files in /etc: `find /etc -name "*.conf" 2>/dev/null | head`.
3. Find where bash lives: `which bash`.

---

## Level 9: The Void Walker
*Remote Access (SSH & Curl)*

Project your consciousness to other machines.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `ssh user@host` | Connect to a remote server. |
| `ssh -p [port] user@host` | Connect on a specific port. |
| `exit` | Disconnect from remote session. |
| `ssh-keygen -t ed25519` | Generate SSH key pair. |
| `ssh-copy-id user@host` | Copy public key to server. |
| `scp [file] user@host:/path` | Copy file to remote server. |
| `curl [url]` | Fetch URL content. |
| `curl -O [url]` | Download file (keep original name). |
| `curl -I [url]` | Fetch HTTP headers only. |
| `wget [url]` | Download file (alternative). |

> 🛡️ **Loot Acquired**: `ssh`, `ssh-keygen`, `scp`, `curl`, `wget`

### ⚔️ Mission
1. Generate an SSH key: `ssh-keygen -t ed25519` (press Enter for defaults).
2. View your public key: `cat ~/.ssh/id_ed25519.pub`.
3. Download a file: `curl -O https://www.google.com/robots.txt`.
4. Check HTTP headers: `curl -I https://fedoraproject.org`.

---

## Level 10: The Automaton
*Bash Scripting*

Why cast spells manually? Build a golem (script) to do it for you.

### 🔮 Crafting a Golem

1. Create the file: `nano golem.sh`
2. Add the brain (shebang): `#!/bin/bash`
3. Write your spells:

```bash
#!/bin/bash
# My first golem script

echo "🤖 Awakening the golem..."
echo "Current date: $(date)"
echo "Current user: $(whoami)"
echo "Current directory: $(pwd)"

mkdir -p ~/golem_data
echo "Log entry: $(date)" >> ~/golem_data/log.txt
echo "✅ Task complete, master!"
```

4. Give it life: `chmod +x golem.sh`
5. Unleash it: `./golem.sh`

### 🔮 Variables & Logic

```bash
#!/bin/bash
NAME="Wizard"
echo "Hello, $NAME!"

# Conditional logic
if [ -f "/etc/fedora-release" ]; then
    echo "You are running Fedora!"
else
    echo "This is not Fedora."
fi

# Loops
for i in 1 2 3; do
    echo "Count: $i"
done
```

> 🛡️ **Loot Acquired**: `#!/bin/bash`, `chmod +x`, variables, `if/else`, `for` loops

### ⚔️ Mission
1. Create the golem script above.
2. Make it executable: `chmod +x golem.sh`.
3. Run it: `./golem.sh`.
4. Check the log: `cat ~/golem_data/log.txt`.

---

## Level 11: The Overlord
*Systemd Services*

Control the daemons that haunt the background.

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `systemctl status [service]` | Check if a daemon is running. |
| `sudo systemctl start [service]` | Start a daemon now. |
| `sudo systemctl stop [service]` | Stop a daemon now. |
| `sudo systemctl restart [service]` | Restart (after config changes). |
| `sudo systemctl enable [service]` | Start on boot. |
| `sudo systemctl disable [service]` | Don't start on boot. |
| `systemctl list-units --type=service` | List all services. |
| `journalctl -u [service]` | View logs for a service. |
| `journalctl -xe` | View recent error logs. |

> 🛡️ **Loot Acquired**: `systemctl`, `journalctl`

### ⚔️ Mission
1. Check the firewall status: `systemctl status firewalld`.
2. Check SSH daemon: `systemctl status sshd`.
3. View recent errors: `journalctl -xe | head -50`.

---

## Level 12: God Mode
*Power User Tricks*

You have reached the level cap. Unlock the cheats.

### 🔮 Secret Techniques

| Technique | Power |
|:----------|:------|
| `Ctrl + R` | Reverse search command history. |
| `Ctrl + A` | Jump to start of line. |
| `Ctrl + E` | Jump to end of line. |
| `Ctrl + U` | Delete from cursor to start. |
| `Ctrl + K` | Delete from cursor to end. |
| `Ctrl + L` | Clear screen. |
| `!!` | Repeat last command. |
| `!$` | Use last argument of previous command. |
| `cd -` | Return to previous directory. |
| `history` | View command history. |
| `!123` | Run command number 123 from history. |

### 🔮 Aliases (Permanent Shortcuts)

Edit your `.bashrc`:

```bash
nano ~/.bashrc
```

Add these at the end:

```bash
# My custom aliases
alias update='sudo dnf update -y'
alias ll='ls -la'
alias ..='cd ..'
alias ...='cd ../..'
alias grep='grep --color=auto'
alias df='df -h'
alias free='free -h'
```

Apply changes:

```bash
source ~/.bashrc
```

> 🛡️ **Loot Acquired**: Shortcuts, aliases, history tricks

### ⚔️ Mission
1. Try reverse search: `Ctrl+R`, then type "dnf".
2. Add the aliases above to your `.bashrc`.
3. Apply them: `source ~/.bashrc`.
4. Test: type `ll` and enjoy!

---

## ★ Bonus Level: Permissions & Ownership
*The Gatekeeper*

Control who can access your files.

### 🔮 Understanding Permissions

When you run `ls -l`, you see something like:

```
-rwxr-xr-- 1 user group 1234 Jan 1 12:00 file.txt
```

| Symbol | Meaning |
|:-------|:--------|
| `r` | **R**ead |
| `w` | **W**rite |
| `x` | E**x**ecute |
| `-` | No permission |

The 10 characters: `[type][owner][group][others]`

### 🔮 Powers

| Command | Description |
|:--------|:------------|
| `chmod +x [file]` | Make executable. |
| `chmod 755 [file]` | rwx for owner, rx for others. |
| `chmod 644 [file]` | rw for owner, r for others. |
| `chown user:group [file]` | Change ownership. |
| `sudo chown -R user:group [dir]` | Recursive ownership change. |

> 🔢 **Number Codes**: `r=4`, `w=2`, `x=1`. Add them up!
> - `7` = rwx (4+2+1)
> - `5` = rx (4+1)
> - `4` = r (4)

> 🛡️ **Loot Acquired**: `chmod`, `chown`, permission codes

### ⚔️ Mission
1. Create a script: `echo '#!/bin/bash' > test.sh && echo 'echo "Hello!"' >> test.sh`.
2. Try to run it: `./test.sh` (it will fail!).
3. Make it executable: `chmod +x test.sh`.
4. Run it again: `./test.sh` (success!).

---

## 🏆 Achievement Unlocked: Fedora Terminal Master!

```
╔═══════════════════════════════════════════════════════════════╗
║                                                               ║
║   🎮 CONGRATULATIONS! 🎮                                      ║
║                                                               ║
║   You have completed the Fedora Terminal RPG!                 ║
║                                                               ║
║   Skills Acquired:                                            ║
║   ✓ Navigation & File Management                              ║
║   ✓ Text Editing                                              ║
║   ✓ Software Management                                       ║
║   ✓ System Monitoring                                         ║
║   ✓ Networking                                                ║
║   ✓ Remote Access                                             ║
║   ✓ Bash Scripting                                            ║
║   ✓ Service Management                                        ║
║   ✓ Permissions                                               ║
║                                                               ║
║   This is not GAME OVER. This is NEW GAME+.                   ║
║   Keep exploring. Keep building. Keep conquering.             ║
║                                                               ║
╚═══════════════════════════════════════════════════════════════╝
```

---

*Made with ❤️ for Fedora Linux*

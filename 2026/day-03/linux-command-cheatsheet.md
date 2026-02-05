# Linux command cheatsheet
📁 File & Directory Management

ls – List files and directories

pwd – Show current directory path

cd <dir> – Change directory

mkdir <dir> – Create a new directory

rmdir <dir> – Delete an empty directory

cp <src> <dest> – Copy files/directories

mv <src> <dest> – Move or rename files

rm <file> – Delete a file

rm -r <dir> – Delete directory recursively

touch <file> – Create an empty file
=================================================================

📄 File Viewing & Editing

cat <file> – View file content

less <file> – View file page by page

head <file> – Show first 10 lines

tail <file> – Show last 10 lines

tail -f <file> – Live log monitoring

nano <file> – Edit file using nano editor

vi <file> – Edit file using vi editor

🔍 Search & Filters

grep "text" <file> – Search text in a file

find <path> -name "file" – Find files by name

wc -l <file> – Count number of lines

sort <file> – Sort file content

uniq – Remove duplicate lines
=================================================================

⚙️ Permissions & Ownership

chmod 755 <file> – Change file permissions

chown user:group <file> – Change file owner

ls -l – View permissions in detail
=================================================================

🧠 Process & System Monitoring

ps -ef – Show running processes

top – Real-time process monitoring

htop – Enhanced process viewer

kill <pid> – Kill a process

df -h – Disk usage (human readable)

free -m – Memory usage in MB

uptime – System running time
=================================================================

🌐 Networking Commands (Required)

ping <host> – Check network connectivity

ip addr – Show IP address details

curl <url> – API testing / HTTP request

netstat -tulnp – Show listening ports

ss -tuln – Modern replacement for netstat
=================================================================

📦 Package Management (Ubuntu/Debian)

apt update – Update package list

apt install <pkg> – Install a package

apt remove <pkg> – Remove a package

📌 Pro Tip (Interview Friendly)

Combine commands using | (pipe)
Example:

ps -ef | grep java


👉 Finds running Java processes
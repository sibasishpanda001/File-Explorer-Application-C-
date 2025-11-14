# File-Explorer-Application-C-

📁 File Explorer Application (C++)

A Linux-style console-based File Explorer built in C++17 using <filesystem>, with support for file/directory operations, permission simulation, sudo override, and color-coded output — similar to a mini Linux shell.

This project was developed as a 5-day Capstone Project, adding new features each day — ranging from listing files to full permission management.

---

🚀 Features

✔ List files & directories with color-coded permission-style output
✔ Navigate and manage directory structure
✔ Create, delete, and move files & folders
✔ Copy files (with overwrite support)
✔ Simulated Linux-style permissions (rwx in octal format like 755)
✔ .permissions.txt storage to keep custom permissions
✔ “sudo mode” to bypass restrictions for one command
✔ Error handling for invalid operations
✔ Minimal and very fast — built entirely with modern C++17


---

🎯 Objective

To build a C++ console file explorer that interacts with the Linux file system, enabling users to perform file management tasks similar to Linux command-line tools.


---

📅 Day-wise Development Progress

Day 1 — Basic File Listing

Setup project structure
Display files & folders
Add colored output based on file type & permissions


Day 2 — Directory Navigation

Add cd command
Improve path handling
Better error messages


Day 3 — File Manipulation

Add cp, mv, del, mkdir, rmdir
Basic permission checks


Day 4 — File Search

Recursive search (if implemented)
Pattern-based searching (optional)

Day 5 — Permission Management

Implement chmod
Add .permissions.txt storing system
Add fake sudo mode



---

🛠 Installation & Compilation

📌 Requirements
> Linux OS
> g++ with C++17 support
> Terminal access

📌 Build
g++ -std=c++17 main.cpp -o explorer

📌 Run
./explorer

---

🧭 Usage Controls (Commands Guide)

Command	              Usage	             Description

ls		                                   List files with color & permissions
cd <dir>	cd folderName	Change directory
mkdir <name>	mkdir test	Create a new folder
rmdir <name>	rmdir test	Remove directory (only if empty)
del <file>	del note.txt	Delete a file
cp <src> <dest>	cp a.txt b.txt	Copy file to destination
mv <src> <dest>	mv old new	Move or rename file/directory
chmod <file> <perm>	chmod my.txt 755	Change permissions (octal format)
perm <file>	perm my.txt	Show assigned permissions
sudo <cmd>	sudo rm file.txt	Bypass permission for 1 command
help		Show help menu
exit		Quit program

---

📌 How Permissions Work

> Each file/directory has a stored permission string example:
  drwxr-xr-x
  -rw-r--r--
> Changing permissions with octal (e.g., 755) converts into full rwx format
> Permissions are saved into .permissions.txt
> These permissions simulate Linux permissions; actual OS permissions are not changed

---

🔐 Sudo Mode

Sudo applies only for the next command:
   sudo del protected.txt

After executing one command, sudo automatically turns off.


---

🖼 Screenshots

💡 Note: Below are real outputs from the terminal showing how the tool evolved from Day 1 → Day 5.

📸 Day 1 — File Listing Output

![Day 1 Output](ls command.png)

📸 Day 2 — Directory Navigation

(Insert Image Here)

📸 Day 3 — File Manipulation

(Insert Image Here)

📸 Day 4 — File Search

(Insert Image Here)

📸 Day 5 — Permission Management

(Insert Image Here)


---

📚 Project Structure

📁 File-Explorer-Application-C++
│── main.cpp
│── .permissions.txt   (auto-generated)
│── README.md
│── screenshots/       (optional folder)


---

📄 License

This project is open-source and available under the MIT License.


---

👤 Author

Sibasish Panda
Final Year B.Tech (Computer Science)

---

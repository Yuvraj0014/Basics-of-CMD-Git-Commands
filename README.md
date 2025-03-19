## 🖥️ **Introduction to CMD** 🎯📦🚀

The Command Prompt (CMD) is a powerful 🛠️ tool used to execute commands and manage 📁 files and 📂 directories in Windows. This guide will cover essential commands for 🧭 navigating, 🏗️ creating, 📥 copying, and 🗑️ deleting files and folders using CMD. Mastering these commands can significantly enhance your efficiency when working on projects.

---

## 🌟 **Importance of CMD** 🌐🛡️📊

- 📁 Efficient file and folder management.
- 🚀 Quick navigation through directories.
- 🤖 Automation possibilities with batch files.
- 🛡️ Useful for troubleshooting and system management.

---

## 📍 **1. Viewing the Current Directory** 🗺️🔎📍

To view your current directory/path:

```cmd
pwd
```

---

## 🧭 **2. Navigating Through Files and Folders** 🚶‍♂️🛤️📂

### 🏠 **Case A: If the Path is** `C:/user/admin`

```cmd
cd documents
```

### 🏠 **Case B: If the Path is** `C:/user/"user_name"`

First, navigate to the Desktop:

```cmd
cd C:/user/yuvraj/OneDrive/Desktop/
```

Then, open the **📁 Documents** folder:

```cmd
cd documents
```

### 📜 **Listing Files and Folders** 📃🗂️👀

To view all files and folders in the current directory:

```cmd
ls
```

### 🔙 **Going Back a Step** ⬅️🔄🚪

To move one directory up:

```cmd
cd ..
```

---

## 🏗️ **3. Creating Folders** 📦🛠️📁

To create a folder:

```cmd
mkdir folder_name
```

Example:

```cmd
mkdir python
```

---

## 📦 **4. Creating Files and Folders Inside a Directory** 🗂️🖋️📊

Navigate inside a folder:

```cmd
cd python
```

Now, create files or folders:

```cmd
mkdir oops          # 📁 Create a folder
touch forloop.py     # 🐍 Create a Python file
touch data.csv       # 📊 Create a CSV file
```

---

## 🗂️ **5. Copying Files Between Folders** 📥📤🔁

Create a file inside the **oops** folder:

```cmd
touch inheritance.py
```

### 📥 **Copying Files to Another Folder** 📁📦📑

If inside the **oops** folder:

```cmd
cp inheritance.py ..
```

If inside the **python** folder:

```cmd
cp oops/inheritance.py .
```

### 🕵️ **Verifying the File Copy** 🔎🗂️✅

Navigate back and list files:

```cmd
cd ..
ls
```

---

## 🗑️ **6. Deleting Files and Folders** 🧹🚫🗂️

### 🧹 **Deleting Files** 📃❌🗑️

To delete a file:

```cmd
rm data.csv
```

### 🗑️ **Deleting Folders** 🧹📦💥

To delete a folder and all its contents:

```cmd
rm -rf oops
```

---

## 🏡 **7. Returning to the Home Directory** 🏠🛤️⬅️

To return to the home directory:

```cmd
cd ~
```

---

## 🧽 **8. Clearing the Terminal Screen** 🧼🖥️🧹

To clear the screen:

```cmd
clear
```

Alternatively, use this keyboard shortcut:

```
Ctrl + L
```

---

## ✅ **Conclusion** 🎉👏🧑‍💻

These basic CMD commands will assist you in efficiently managing files and folders. 🧑‍💻 Mastering these commands will make navigating through directories and executing tasks much easier, enhancing your productivity when working on projects.

For further exploration, you can refer to CMD documentation or explore more advanced commands. Happy coding! 🎉🚀💻

---
---

## 🖥️ **Introduction to Git** 🎯📦🚀

Git is a distributed version control system that helps developers track changes in code, collaborate with others, and manage software projects efficiently. This guide will cover essential Git commands for initializing repositories, making commits, managing branches, and pushing changes to remote repositories.

---

## 🌟 **Importance of Git** 🌐🛡️📊

- 🌐 Collaborate seamlessly with other developers.
- 🚀 Track changes and maintain version history.
- 🛡️ Manage branches for different features and bug fixes.
- 📦 Synchronize local changes with remote repositories.

---

## 🛠️ **1. Initializing a Repository** 🧑‍💻📂🛠️

To create a new Git repository in your project directory:

```bash
git init
```
This initializes an empty Git repository.

---

## 📤 **2. Adding Files to Staging Area** 📥📦📂

To add all the files in the current directory to the staging area:

```bash
git add .
```
This stages all changes (new, modified, or deleted files).

---

## 🗂️ **3. Committing Changes** 📝🔎✅

To save changes in your repository with a descriptive message:

```bash
git commit -m "Initial commit"
```
The `-m` flag allows you to add a message describing the changes.

---

## 🏷️ **4. Renaming the Branch to Main** 🏷️🧑‍💻🌿

To rename the default branch to `main` (a common practice in modern repositories):

```bash
git branch -M main
```
This command renames the branch to `main`.

---

## 🌐 **5. Adding a Remote Repository** 🔗🌍🛜

To connect your local repository to a remote GitHub repository:

```bash
git remote add origin https://github.com/username/repository.git
```
Replace `username` and `repository.git` with your actual GitHub username and repository name.

---

## 🚀 **6. Pushing Changes to GitHub** 🚢🆙📡

To push your changes from the local branch to the remote branch:

```bash
git push -u origin main
```
The `-u` flag sets the upstream branch to track the remote branch.

---

## ✨ **7. Making Changes in an Existing Repository** 🔄🛠️📝

After making further changes to your project, follow these steps:

### 🛠️ **Add Changes to Staging Area:**
```bash
git add .
```

### 📝 **Commit the Changes with a Message:**
```bash
git commit -m "Your commit message"
```

### 📤 **Push Changes to GitHub:**
```bash
git push -u origin main
```
This will upload the latest changes to your remote repository.

---

## 🆕 **8. First Time Setup vs. Regular Pushing** 🚀🆙🔁

- **First Time Setup:**  
  When connecting to a GitHub repository for the first time, follow all the steps from **`git init`** to **`git push -u origin main`**. This establishes the connection between your local repository and the remote one.

- **Making Changes & Pushing:**  
  After the initial setup, you only need these three commands to add, commit, and push your changes:
  
  ```bash
  git add .
  git commit -m "Your commit message"
  git push
  ```
  Using `git push` without `-u origin main` is sufficient for subsequent pushes, as Git will remember the remote branch.

---

## ✅ **Conclusion** 🎉👏🧑‍💻

These essential Git commands will help you effectively manage your projects and collaborate with your team. By mastering these commands, you can track changes, push code to repositories, and contribute to open-source projects with confidence. Happy coding! 🎉🚀💻

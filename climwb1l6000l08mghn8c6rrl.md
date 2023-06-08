---
title: "Getting Started with Linux with some basic commands"
seoTitle: "Getting Started with Linux"
seoDescription: "Discover the fundamentals and essential commands of Linux in our comprehensive blog. Learn how to navigate, execute commands, and unleash the power."
datePublished: Thu Jun 08 2023 08:47:26 GMT+0000 (Coordinated Universal Time)
cuid: climwb1l6000l08mghn8c6rrl
slug: getting-started-with-linux-with-some-basic-commands
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1686088282020/dcca61fa-2ead-440a-9226-93188aa2ddfe.png
tags: ubuntu, linux, web-development, linux-for-beginners, linux-basics

---

## Introduction

Linux, an open-source operating system known for its stability, flexibility, and security, has gained tremendous popularity in recent years. Its vast ecosystem of distributions, known as <mark>distros</mark>, offers a variety of options suited to different user preferences and needs. For newcomers entering the Linux world, navigating through the diverse commands and concepts can be confusing. This blog post aims to serve as your trusted guide we will discuss about the fundamentals of Linux, which is the best distro for you, and will equip you with essential commands to get started. Together, we will unravel the mysteries of the command line and discover the perfect Linux distro tailored to your needs. Let's begin our exploration and unlock the true potential of Linux!

## Why Linux?

Linux offers numerous advantages that make it an attractive choice for both beginners and experienced users. Here are some compelling reasons why you should consider Linux as your operating system:

### **Open Source and Free**

Linux is an open-source operating system, which means <mark>its source code is freely available to the public</mark>. This allows developers and enthusiasts to study, modify, and distribute Linux without licensing restrictions. As a user, you have the freedom to use Linux for any purpose, share it with others, and contribute to its development. Additionally, most Linux distributions are available for free, providing cost-effective access to a powerful operating system.

### **Stability and Reliability**

Linux is known for its stability and reliability. It is widely used in servers, supercomputers, and other critical systems that require constant uptime. Moreover, Linux's security model and quick response to vulnerabilities contribute to its overall stability.

### **Customizability and Flexibility**

Linux offers a high level of customizability and flexibility. Unlike other operating systems, Linux allows you to tailor your user experience by choosing different desktop environments, themes, and configurations. You can customize every aspect of your Linux system to suit your preferences and workflow. Additionally, Linux supports a wide range of software applications and programming languages, making it a versatile platform for developers and power users.

<mark>This meme just depicts how flexible Linux is:</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686161209282/b01c15cc-6caf-46f5-ba27-d29af4e94a8e.jpeg align="center")

### **Strong Community and Support**

Linux has a vibrant and supportive community of users, developers, and enthusiasts worldwide. Online forums, discussion boards, and dedicated websites provide a wealth of knowledge and resources to assist users at all levels. If you encounter any issues or have questions, the Linux community is there to help you find solutions and share their expertise. <mark>This collaborative environment fosters learning, collaboration, and the continuous improvement of Linux distributions</mark>.

### **Security and Privacy**

Linux is renowned for its security features. Due to its open-source nature, vulnerabilities are discovered and patched quickly by the community. Linux also respects user privacy, providing greater control over data and minimizing the collection of personal information compared to some proprietary operating systems.

### **Command Line Interface**

Using Linux presents educational and learning opportunities. <mark>By exploring the command-line interface and understanding the inner workings of the operating system, you can deepen your knowledge of computer systems and enhance your technical skills</mark>. Linux's open nature encourages exploration and experimentation, making it an ideal platform for individuals interested in learning about operating systems and computer science concepts.

## **Understanding Linux Distributions**

Linux distributions are variations of the Linux operating system that bundle the Linux kernel, essential software, and additional packages into a complete package. Each distribution aims to provide a unique user experience by customizing the software selection, desktop environment, and system configuration.

Some popular Linux distributions include:

* <mark>Ubuntu</mark>: Ubuntu is one of the most popular and beginner-friendly Linux distributions. It emphasizes ease of use, stability, and a large supportive community. It offers a user-friendly graphical interface and extensive software repositories.
    
* <mark>Linux Mint</mark>: Based on Ubuntu, Linux Mint is designed to provide a familiar desktop experience for Windows users. It focuses on simplicity, elegance, and multimedia support.
    
* <mark>Fedora</mark>: Developed by the Fedora Project, Fedora emphasizes the latest software and technologies. It aims to provide a cutting-edge experience while maintaining stability and security.
    
* <mark>Debian</mark>: Known for its stability, Debian is a versatile distribution that focuses on free and open-source software. It offers a wide range of software packages and multiple desktop environment choices.
    

These are just a few examples, and there are many more distributions available to explore. The key is to find one that suits your needs, preferences, and level of familiarity with Linux.

## **Choosing a Beginner-Friendly Linux Distribution:**

When selecting a beginner-friendly distribution, consider the following factors:

### **Ease of Installation**

Look for a distribution that offers a straightforward installation process with good hardware support. Ubuntu and Linux Mint are known for their user-friendly installation wizards.

### **Desktop Environment**

The desktop environment provides the graphical user interface (GUI) for your Linux distribution. Common desktop environments include GNOME, KDE, XFCE, and Cinnamon. Choose a distribution that offers a desktop environment that suits your preferences and provides an intuitive user interface.

### **Community and Support**

Consider the availability of a supportive community that can assist you with any questions or issues you may encounter. Active forums, documentation, and online resources can greatly aid your learning process.

### **Software Repositories**

A distribution with a wide range of software packages in its repositories makes it easier to install and manage applications. Look for a distribution that provides an extensive collection of software and regular updates.

### **Compatibility and Hardware Support**

Ensure that the distribution you choose supports your hardware components, such as <mark>graphics cards, wireless adapters, and peripherals</mark>. Most popular distributions offer good hardware compatibility, but it's always worth checking.

My suggestion for a beginner who is getting started with Linux is to go with Ubuntu.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686212602072/d9a8c826-318e-4d8a-8d34-f3083fb8c088.png align="center")

## **Getting Started with Linux**

Before we delve into the commands, let's cover the fundamental aspects of Linux to help you understand its structure and concepts.

### **Terminal**

The command line interface (CLI) is your gateway to Linux. While graphical interfaces are available, the terminal provides a powerful and efficient way to interact with the operating system. It allows you to execute commands, perform tasks, and automate processes.

### **File System**

Linux follows a hierarchical file system structure. The root directory is denoted by a forward <mark>slash (/)</mark>, and all other directories and files are organized beneath it. Directories are similar to folders, providing a way to organize files and subdirectories. Files can contain data or executable programs.

### **Command Syntax**

Linux commands typically follow the format: `command [options] [arguments]`. <mark>Options modify the behavior of a command, while arguments provide inputs or specify targets. Commands are case-sensitive, so pay attention to the letter casing</mark>.

## **Essential Linux Commands**

Let's explore some essential Linux commands that will help you navigate the file system, manipulate files and directories, and perform basic operations.

### `ls`: List Directory Contents

The `ls` command allows you to view the contents of a directory. Use it without any arguments to list files and directories in the current directory. For example, `ls` will display the files and directories present in your current location.

To list files and directories in a specific directory, provide the directory path as an argument. For example, `ls /home/user/Documents` will display the contents of the "Documents" directory.

```bash
# List files and directories in the current directory
ls
```

### `cd`: Change Directory

With the `cd` command, you can navigate through the file system. Use it followed by the directory name to move to a specific directory. For example, `cd Documents` will take you to the "Documents" directory.

To move up one directory level, use `cd ..`. For example, if you are in the "Documents" directory, `cd ..` will take you back to the parent directory.

To move directly to your home directory, simply type `cd` without any arguments.

```bash
# Change to the specified directory
cd /path/to/directory
```

### `pwd`: Print Working Directory

The `pwd` command helps you identify the current working directory. It displays the full path of your current location in the file system. When you are unsure about your current location, `pwd` will provide the absolute path.

```bash
# Print the current working directory
pwd
```

### `mkdir`: Make Directory

To create a new directory, use the `mkdir` command followed by the desired directory name. For instance, `mkdir NewFolder` will create a new directory named "NewFolder" in your current location.

To create a directory within another directory, specify the path. For example, `mkdir Documents/NewFolder` will create "NewFolder" inside the "Documents" directory.

```bash
# Create a new directory with the specified name
mkdir new_directory
```

### `rm`: Remove

The `rm` command allows you to delete files and directories. Be cautious while using it, as deleted files cannot be recovered. To remove a file, use `rm filename`. For instance, `rm myfile.txt` will delete the file named "myfile.txt" in your current directory.

To delete a directory, add the `-r` option to the `rm` command. This is necessary because directories can contain files and subdirectories. For example, `rm -r directoryname` will delete the directory and its contents recursively.

```bash
# Remove the specified file
rm filename

# Remove a directory and its contents recursively
rm -r directory_name
```

### `cp`: Copy

The `cp` command enables you to copy files and directories. To copy a file, use `cp sourcefile destination`. For example, `cp myfile.txt /home/user/Documents` will copy "myfile.txt" to the "Documents" directory.

To copy a directory and its contents, add the `-r` option to the `cp` command. For instance, `cp -r sourcedirectory destination` will copy the directory and its contents recursively.

```bash
# Copy a file to a new location
cp file.txt /path/to/destination

# Copy a directory and its contents recursively to a new location
cp -r directory_name /path/to/destination
```

### `mv`: Move

With the `mv` command, you can move both files and directories. To move a file, use `mv sourcefile destination`. For example, `mv myfile.txt /home/user/Documents` will move "myfile.txt" to the "Documents" directory.

To move a directory and its contents, add the `-r` option to the `mv` command. For instance, `mv -r sourcedirectory destination` will move the directory and its contents recursively.

```bash
# Move a file to a new location or rename it
mv file.txt /path/to/destination

# Move a directory to a new location or rename it
mv directory_name /path/to/destination
```

### `cat`: Concatenate and Print

The `cat` command allows you to display the contents of a file in the terminal. For example, `cat myfile.txt` will display the contents of "myfile.txt" in your terminal window.

```bash
# Display the contents of the specified file
cat filename
```

### `man`: Manual Pages

The `man` command provides access to Linux manual pages. You can use it to obtain information and usage instructions for various commands. For example, `man ls` will display the manual page for the `ls` command, providing detailed explanations and options.

```bash
# Display the manual page for the specified command
man command_name
```

### `sudo`: Administrative Privileges

On Linux systems, the `sudo` command allows authorized users to execute commands with administrative or root privileges. This is essential for performing tasks that require elevated permissions, such as installing system packages, modifying system configurations, or accessing protected directories.

Using `sudo` before a command allows a user to temporarily elevate their privileges to perform administrative tasks. For example, to install a package system-wide using the package manager, you would use the `sudo` command as follows: `sudo apt install packagename` (replace `apt` with the appropriate package manager for your distribution).

By requiring the use of `sudo` for administrative tasks, Linux promotes the principle of least privilege, enhancing system security by ensuring that users operate with regular user privileges by default and only elevate when necessary.

```bash
# Execute a command with administrative privileges using sudo
sudo command_name
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686161492777/37e96ab2-ab40-4c26-9a1f-c75ac73366fe.jpeg align="center")

## Conclusion

Congratulations! You've taken your first steps into the world of Linux. By familiarizing yourself with these basic commands, you're well on your way to becoming proficient in navigating and interacting with the Linux operating system. Remember, practice is key to mastery, so don't hesitate to explore further and experiment with additional commands and concepts. Linux can be your best friend if you practice the CLI, enjoy your Linux journey, and embrace the power of the command line!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686161579970/aa7634ee-4f9d-4b79-bc8a-1ab42e987515.jpeg align="center")

## **Let's Connect**

If you enjoyed this post and would like to stay updated on my work, feel free to connect with me on social media

* LinkedIn: Click [**here**](https://www.linkedin.com/in/nikhil-mishra-8a6710244)
    
* Github: Click [**here**](https://github.com/mnik7044)
    
* Twitter: Click [**here**](https://twitter.com/nikktwts?t=WxH0im12f-NtbUJGeV2Xsw&s=09)
    

If you find my blog helpful you all can always support me by sponsoring me!
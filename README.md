# 🚀 MEGA File Sharing on Linux Server

This repository provides a step-by-step guide to using MEGA for file sharing on a Linux server. Follow these instructions to install the MEGA command-line tool (`megacmd`), configure your account, and upload files to your MEGA cloud storage.

![MEGA Logo](https://raw.githubusercontent.com/YoloNet/linux-MEGA-FileShared/main/mega.png)

## 📋 Prerequisites

- A Linux server (tested on Ubuntu 20.04) 🐧
- An active MEGA account 📧
- Basic knowledge of command-line operations 💻

## 🛠 Installation

### Step 1: Download the MEGA Command-Line Tool

First, download the `megacmd` package for Ubuntu 20.04:

```sh
wget https://mega.nz/linux/MEGAsync/xUbuntu_20.04/amd64/megacmd-xUbuntu_20.04_amd64.deb
```

You can find installers for different operating systems [here](https://mega.nz/linux/MEGAsync/).


### Step 2: Install the Package

Use dpkg to install the downloaded package:

```sh
sudo dpkg -i megacmd-xUbuntu_20.04_amd64.deb
```

If there are any missing dependencies, install them with:

```sh
sudo apt-get install -f
```

## ⚙️ Configuration

### Step 1: Log In to Your MEGA Account

Open a terminal and run the following command to log in to your MEGA account:

```sh
mega-login your-email@example.com
```

### Step 2: Upload Files to MEGA

To upload a file to your MEGA cloud storage, use the `mega-put` command:

```sh
mega-put /path/to/your/file /path/in/mega/
```

Replace `/path/to/your/file` with the path to the file you want to upload, and `/path/in/mega/` with the path in your MEGA cloud storage where you want to upload the file.

## 📦 Check the Upload

Verify that your file has been uploaded correctly with:

```sh
mega-ls /uploads/
```

## ❓ Troubleshooting

- Login Issues: Ensure your credentials are correct and you have an active internet connection. 🔌
- Upload Issues: Verify the file path and check if you have sufficient storage in your MEGA account. 📂
- Command Not Found: Ensure that `megacmd` is correctly installed and added to your PATH. 🛠

## 📚 Additional Resources

For more information on the MEGA command-line tool, visit the [MEGA Command Line Tool documentation](https://mega.nz/cmd).

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

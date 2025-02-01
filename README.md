# GitNOEncryptor

GitNOEncryptor is a command-line tool written in Python to facilitate uploading and downloading files and directories in GitHub repositories.

## ✨ Features

- 💾 **File Upload** – Upload files and directories to a GitHub repository.
- 🔗 **Simple Download** – Download specific files or entire repositories from GitHub.
- ⏳ **Time Measurement** – Displays the time taken for each operation.
- 👾 **CLI-Friendly and Efficient** – Easy-to-use command-line interface.

## ⚙️ Prerequisites

- Python 3.x: Make sure Python 3 is installed on your system before using GitFileManager.

## 🔧 Setup

Before using GitFileManager, you need to create a `config.json` file in the same directory as the tool. This file is required for authentication with GitHub.

### Example of `config.json`
```json
{
  "username": "your-username",
  "token": "your-github-token"
}
```

## 📚 Command-Line Options

| Argument                     | Description |
|------------------------------|-------------|
| `--upload_file`              | Uploads a file to GitHub. |
| `--upload_dir`               | Uploads an entire directory to GitHub. |
| `--target_repo_url`          | Specifies the destination repository on GitHub. |
| `--download_file_repo`       | Downloads a specific file from GitHub. |
| `--download_repo`            | Downloads an entire repository from GitHub. |
| `--dest_dir`                 | Sets the local directory where downloaded files will be stored. |
| `--time`                     | Measures execution time of operations in seconds. |

## 🚀 Usage

### 1⃣ Upload a file

```bash
python3 gitfilemanager.py --upload_file /path/to/file.txt --target_repo_url https://github.com/user/repository/
```

### 2⃣ Download a file

```bash
python3 gitfilemanager.py --download_file_repo https://github.com/user/repository/blob/main/file.txt --dest_dir /destination/path/
```

### 3⃣ Upload an entire directory

```bash
python3 gitfilemanager.py --upload_dir /path/to/directory/ --target_repo_url https://github.com/user/repository/
```

### 4⃣ Download an entire repository

```bash
python3 gitfilemanager.py --download_repo https://github.com/user/repository/ --dest_dir /destination/path/
```

## 🏰 Contribution

Feel free to open issues and pull requests!

📄 License: MIT

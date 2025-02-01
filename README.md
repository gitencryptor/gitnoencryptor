# GitNOEncryptor

GitNOEncryptor is a command-line tool written in Python to facilitate uploading and downloading files and directories in GitHub repositories.

## ✨ Features

- 💾 **File Upload** – Upload files and directories to a GitHub repository.
- 🔗 **Simple Download** – Download specific files or entire repositories from GitHub.
- ⏳ **Time Measurement** – Displays the time taken for each operation.
- 👾 **CLI-Friendly and Efficient** – Easy-to-use command-line interface.

## ⚙️ Prerequisites

- Python 3.x: Make sure Python 3 is installed on your system before using GitNOEncryptor.

## 🔧 Configuration

- Before using GitNOEncryptor, you need to create a `config.json` file in the same directory as the tool. This file is required for authentication with GitHub.

### `config.json` Example
```json
{
  "username": "your-username",
  "token": "your-github-token"
}
```

## 📜 Command Line Options

| Argument                  | Description                                                       |
| ------------------------- | ----------------------------------------------------------------- |
| `--upload_local_file`      | Uploads the specified file to GitHub.                             |
| `--upload_local_batch_file`| Uploads a list of files to GitHub.                                |
| `--upload_dir_file`        | Uploads all files from a specified directory to GitHub.           |
| `--target_repo_url`        | Specifies the destination repository URL for uploads or downloads.|
| `--download_url_file_repo` | Downloads a specific file from a GitHub URL.                      |
| `--download_url_batch_file`| Downloads a list of files from GitHub using their URLs.           |
| `--dest_dir`               | Sets the local directory where downloaded files will be stored.   |
| `--time`                   | Measures execution time of operations.                            |



## 🛠 Usage

### 1️⃣ Upload a file

```bash
python3 gitnoencryptor.py --upload_file /path/to/file.txt --target_repo_url https://github.com/user/repository/
```

### 2️⃣ Download a file

```bash
python3 gitnoencryptor.py --download_file_repo https://github.com/user/repository/blob/main/file.txt --dest_dir /destination/path/
```

### 3️⃣ Upload an entire directory

```bash
python3 gitnoencryptor.py --upload_dir /path/to/directory/ --target_repo_url https://github.com/user/repository/
```

### 4️⃣ Download an entire repository

```bash
python3 gitnoencryptor.py --download_repo https://github.com/user/repository/ --dest_dir /destination/path/
```

📄 License: MIT

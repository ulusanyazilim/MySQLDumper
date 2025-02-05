# MySQLDumper 

## Backup & Restore for MySQL Databases with Php 7.4+

MySQLDumper is a powerful tool for backing up and restoring MySQL databases. Originally developed by Daniel Schlichtholz and the MySQLDumper team, the project had been discontinued at version **1.24**. However, the community has revived it with PHP 7.4+ support and necessary bug fixes.

👉 **Previous version (1.24) can be found here:** [MySQLDumper 1.24](https://github.com/DSB/MySQLDumper)

### 🌟 Updated Version: 1.25

This new release brings:
- **PHP 7.4+ compatibility**
- Security enhancements
- Various bug fixes

We extend our gratitude to the original developers for their contributions. Their work laid the foundation for this project, and we aim to continue improving it.

## ✨ Features
- **Easy to Use:** Web-based interface for effortless backup and restore operations.
- **Supports Large Databases:** Backups are split into smaller parts to prevent timeout issues.
- **Advanced Compression:** Supports ZIP and BZIP2 compression.
- **Scheduled Backups:** Automate backups at specified intervals.
- **Multi-Language Support:** UI available in multiple languages.
- **Database Repair:** Built-in tools for fixing corrupted MySQL tables.
- **Perl Backup Support:** Option to use a Perl script for improved backup performance.

## 🔍 Installation

1. **Download the Files**  
   - [Download the latest version from GitHub](https://github.com/ulusanyazilim/MySQLDumper)
   - Upload the files to your web server.

2. **Server Requirements**  
   - PHP 7.4 or later  
   - MySQL 3.23 or later  
   - Web server (Apache, Nginx, etc.)

3. **Start Installation**  
   - Open your browser and navigate to `http://yourdomain.com/mysqldumper/`
   - Follow the setup wizard to configure database access and other settings.

## 🛠 Usage

1. **Backup Process**  
   - Log in to the web interface.
   - Navigate to the "Backup" tab and select the database.
   - Click "Start Backup" to begin.

2. **Restore Process**  
   - Go to the "Restore" tab and choose a backup file.
   - Click "Start Restore" to restore your database.

## 📖 Legacy Documentation Highlights

Since version 1.25 retains the core functionality of version 1.24 (except for PHP 7.4+ compatibility and bug fixes), here are some useful legacy features:

### **Installation (Legacy)**
- Unzip the package and upload it to your server.
- Ensure `config.php` has write permissions (`chmod 777`).
- Open `http://yourserver/MySQLDumper` to complete the setup.
- If safe mode is enabled, manually create necessary directories.

### **Perl Backup (Legacy)**
- Copy `crondump.pl`, `perltest.pl`, and `simpletest.pl` to the `cgi-bin` directory.
- Edit `crondump.pl` and configure `$absolute_path_of_configdir`.
- Set `chmod 755` permissions on these scripts.
- If needed, rename `.pl` files to `.cgi` and adjust settings.

### **Configuration Settings (Legacy)**
- **Table Prefix Filtering:** Dump only tables with a specific prefix.
- **GZip Compression:** Reduce backup file size.
- **Backup File Directory:** Define custom storage paths.
- **Batch Processing:** Adjust the number of records processed per cycle to avoid timeouts.

## 📊 Development and Contributions
This is a community-driven project. If you encounter issues or have feature requests, feel free to open a [Pull Request](https://github.com/ulusanyazilim/MySQLDumper/pulls) or submit an issue.

## 🛡️ Security Best Practices
- Store backup files in a **non-public** directory.
- Secure login credentials to prevent unauthorized access.

---
**License:** GNU GPL v2  
Special thanks to the **original MySQLDumper team** and **Daniel Schlichtholz** for their invaluable contributions! 🙌


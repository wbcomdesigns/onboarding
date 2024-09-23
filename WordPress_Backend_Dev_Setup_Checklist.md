
# WordPress Backend Development System Setup

## Windows Setup Checklist

### 1. Local Development Environment
- **Flywheel Local:**
  - Download and install [Flywheel Local for Windows](https://localwp.com/).
  - Configure Local for WordPress development (set up PHP version, database settings, and HTTPS).

### 2. Code Editor
- **Visual Studio Code:**
  - Download and install [Visual Studio Code for Windows](https://code.visualstudio.com/Download).
  - Install relevant extensions:
    - **PHP Intelephense** (for PHP development).
    - **WordPress Snippets** (for WordPress-specific code).
    - **ESLint** (for JavaScript linting).
    - **Prettier** (for code formatting).

### 3. Version Control
- **GitHub Desktop:**
  - Download and install [GitHub Desktop for Windows](https://desktop.github.com/).
  - Configure your GitHub account and repository settings.
- **Git:**
  - Install [Git for Windows](https://git-scm.com/download/win).
  - Configure global git settings:
    ```
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

### 4. Database Management
- Use the **Adminer** or **phpMyAdmin** bundled with Flywheel Local to manage databases.

### 5. PHP & Composer
- **PHP:** Install the version you’re working with from the [Windows PHP repository](https://windows.php.net/download/).
- **Composer:** Download and install [Composer](https://getcomposer.org/download/) for managing dependencies:
  ```
  composer -v
  ```

### 6. Debugging Tools
- **Xdebug:** Verify Xdebug is properly configured in Flywheel Local.
- **Query Monitor:** Install Query Monitor in your WordPress site to check database queries and performance.


## Ubuntu Setup Checklist

### 1. Local Development Environment
- **Flywheel Local:**
  - Download and install [Flywheel Local for Ubuntu](https://localwp.com/releases/). Use the `.deb` file.
  - Configure Local for your preferred PHP version and database settings.

### 2. Code Editor
- **Visual Studio Code:**
  - Install VS Code from the terminal:
    ```
    sudo snap install code --classic
    ```
  - Install the same relevant extensions as on Windows.

### 3. Version Control
- **GitHub Desktop (Alternative: GitKraken or CLI):**
  - GitHub Desktop is not natively available for Linux. Consider using **GitKraken** or the Git CLI instead.
  - **GitKraken:** Download from the [GitKraken website](https://www.gitkraken.com/).
  - **Git CLI:**
    ```
    sudo apt update
    sudo apt install git
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

### 4. Database Management
- Use **Adminer** or **phpMyAdmin** from Flywheel Local or directly install them using terminal commands for standalone use.

### 5. PHP & Composer
- **PHP:** Install the desired PHP version:
  ```
  sudo apt install php
  ```
- **Composer:** Install Composer globally:
  ```
  sudo apt update
  sudo apt install curl php-cli php-mbstring unzip
  curl -sS https://getcomposer.org/installer | php
  sudo mv composer.phar /usr/local/bin/composer
  composer -v
  ```

### 6. Debugging Tools
- **Xdebug:** Ensure that Xdebug is enabled in Flywheel Local.
- **Query Monitor:** Install the Query Monitor plugin in your WordPress instance for query analysis.


## General Tools (Both Windows & Ubuntu)

- **Node.js:** Install Node.js for building front-end assets, running tasks, etc.:
  - Windows: [Node.js installer](https://nodejs.org/).
  - Ubuntu: 
    ```
    sudo apt install nodejs npm
    ```

- **WP-CLI:** Install WP-CLI for managing WordPress via the command line:
  - Windows: [Install WP-CLI manually](https://wp-cli.org/#installing).
  - Ubuntu:
    ```
    curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
    chmod +x wp-cli.phar
    sudo mv wp-cli.phar /usr/local/bin/wp
    wp --info
    ```



# WordPress Theme Development Setup (For Block Development)

## 1. Local Development Environment
- **Flywheel Local:**
  - Download and install [Flywheel Local](https://localwp.com/) for WordPress theme development.
  - Configure Local for WordPress development (set up PHP version, database settings, and HTTPS).
  - Install a clean WordPress environment to start developing the theme.

## 2. Code Editor
- **Visual Studio Code:**
  - Download and install [Visual Studio Code](https://code.visualstudio.com/).
  - Install relevant extensions:
    - **PHP Intelephense** (for PHP development).
    - **WordPress Snippets** (for WordPress-specific code).
    - **ESLint** (for JavaScript and React linting).
    - **Prettier** (for code formatting).
    - **GitLens** (for Git integration in VS Code).
    - **Gutenberg Block Snippets** (for block editor development).
    - **WordPress Block Editor Tools** (for Gutenberg block development assistance).

## 3. Version Control
- **GitHub Desktop:**
  - Download and install [GitHub Desktop](https://desktop.github.com/) for version control.
  - Configure GitHub repositories for theme and block development.
- **Git CLI:**
  - Install Git and configure global git settings:
    ```
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

## 4. WordPress Theme Development Setup
- **Theme Starter Files:**
  - Set up a theme folder in the `wp-content/themes/` directory.
  - Use [Underscores](https://underscores.me/) or [WP Rig](https://wprig.io/) as starter theme options.
  - Ensure the theme supports the WordPress Block Editor by adding `add_theme_support( 'align-wide' );` and `add_theme_support( 'editor-styles' );` in your `functions.php`.

## 5. Block Development Setup
- **Node.js and npm:** Install Node.js to use JavaScript tooling and build processes for Gutenberg blocks.
  - Windows: Download [Node.js](https://nodejs.org/en/).
  - Ubuntu: Install via terminal:
    ```
    sudo apt install nodejs npm
    ```
- **WordPress Scripts Package:**
  - Install [@wordpress/scripts](https://developer.wordpress.org/block-editor/reference-guides/packages/packages-scripts/) to streamline block development:
    ```
    npm init @wordpress/block
    ```

- **Webpack Configuration:**
  - Ensure Webpack is properly configured to bundle JavaScript and CSS files for block development.
  
- **Block JSON Configuration:**
  - Each block should have a `block.json` file that defines the block’s metadata. Use WordPress Block API standards to ensure proper registration.

## 6. Gutenberg Block Development Workflow
- **Create Custom Blocks:**
  - Set up your first custom block by following the WordPress [block development guide](https://developer.wordpress.org/block-editor/getting-started/create-block/).
  - Use JSX (JavaScript XML) and React to build interactive block features.
  
- **Dynamic Blocks:**
  - For blocks that display dynamic content, use PHP for rendering in combination with JavaScript.
  
- **Block Variations:**
  - Explore block variations and custom controls to create flexible blocks for the editor.

## 7. Debugging Tools for Block Development
- **Query Monitor:** Install the [Query Monitor plugin](https://wordpress.org/plugins/query-monitor/) to debug database queries and performance issues.
- **Debug Bar:** Install the [Debug Bar plugin](https://wordpress.org/plugins/debug-bar/) for additional debugging.
- **Browser Developer Tools:** Use Chrome or Firefox Developer Tools to inspect JavaScript errors or issues with block rendering.

## 8. Block Styling and Responsive Design
- **Editor Styles:** Create a `editor-style.css` file in your theme to customize the block editor’s appearance.
- **Responsive Styles:** Ensure that blocks are responsive by adding media queries in both the frontend and editor stylesheets.

## 9. PHP & Composer
- **PHP:** Ensure the correct version of PHP is installed:
  - Windows: [PHP for Windows](https://windows.php.net/download/).
  - Ubuntu: Install via terminal:
    ```
    sudo apt install php
    ```
- **Composer:** Install Composer globally for managing PHP dependencies if necessary:
  - Windows: [Download Composer](https://getcomposer.org/download/).
  - Ubuntu:
    ```
    curl -sS https://getcomposer.org/installer | php
    sudo mv composer.phar /usr/local/bin/composer
    composer -v
    ```

## 10. WP-CLI
- **WP-CLI:** Install WP-CLI for managing WordPress via command line:
  - Windows: [Install WP-CLI manually](https://wp-cli.org/#installing).
  - Ubuntu:
    ```
    curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
    chmod +x wp-cli.phar
    sudo mv wp-cli.phar /usr/local/bin/wp
    wp --info
    ```

## 11. Additional Tools
- **Node.js Task Runners:** Use Gulp or Webpack for automating tasks like minifying assets or watching file changes.
- **Lighthouse Audits:** Use Google Lighthouse (available in Chrome DevTools) to audit the theme's performance and accessibility.


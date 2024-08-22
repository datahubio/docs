# Site Configuration Options

This document provides an overview of the configuration options available in the `config.json` file for your site.

```json
{
  "title": "Site Title",
  "logo": "path/to/logo.png",
  "description": "",
  "showSideBar": false,
  "showEditLink": false,
  "contentInclude": [],
  "contentExclude": [],
  "social": [
    { "label": "linkedin", "href": "https://linkedin.com/user" }
  ],
  "analytics": "UA-XXXXXXXXX-X",
  "author": {
    "name": "Author Name",
    "url": "https://github.com/author-name"
  },
  "navLinks": [
    { "href": "/contact", "name": "Contact" }
  ]
}
```

## General Settings

### 1. **`title`**
- **Description**: The title of your site
- **Example**:
  
  ```json
  "title": "My Awesome Site"
  ```

### 2. **`logo`** 
- **Description**: The path to your site's logo file
- **Example**:
 
  ```json
  "logo": "images/logo.png"
  ```

### 3. **`description`** 
- **Description**: A site description that will be displayed in the footer.
- **Example**:
  
  ```json
  "description": "Lorem ipsum dolor sit amed."
  ```

### 4. **`showSideBar`** 
- **Description**: Enables or disables the sidebar on your site.
- **Usage**: Set this to `true` to display the sidebar, or `false` to hide it and use default site header
  
  ```json
  "showSideBar": true
  ```
- **Default:** `false`

### 5. **`showEditLink`** 
- **Description**: Displays a link allowing users to edit the current page on the GitHub repository.
- **Usage**: Set this to `true` to show the edit link, or `false` to hide it.

  ```json
  "showEditLink": false
  ```
- **Default:** `false`

## Content Management

### 6. **`contentInclude`**
- **Description**: Specifies a list of file paths or directory paths to be explicitly included on the site. If not set, all files will be included by default.
- **Example**:
  
  ```json
  "contentInclude": [
    "index.md", 
    "/blog", 
    "/another-folder"
  ] 
  ```

### 7. **`contentExclude`**
- **Description**: Specifies a list of file paths or directory paths to be excluded from the site. Files or directories listed here will not be included in the site's content.
- **Example**:
  
  ```json
  "contentExclude": [
    "/blog/trash",
    "/archive",
    "/old-file.md"
  ]
  ```

## Social Media Links

### 8. **`social`** 
- **Description**: Configures social media links that will appear in the footer and header of the site.
- **Structure**: Each object in the list contains:
  - `label`: The name of the social media platform (e.g., "facebook").
  - `href`: The URL to your profile on that platform.

- **Example**:

  ```json
  "social": [
    { "label": "youtube", "href": "https://youtube.com/user" },
    { "label": "facebook", "href": "https://www.facebook.com/user" },
    { "label": "linkedin", "href": "https://www.linkedin.com/user" },
    { "label": "twitter", "href": "https://twitter.com/user" },
    { "label": "instagram", "href": "https://instagram.com/user" },
    { "label": "github", "href": "https://github.com/user" },
    { "label": "discord", "href": "https://discord.com/user" }
  ]
  ```

## Analytics

### 9. **`analytics`** 
- **Description**: The Google Analytics key used to track user interactions on your site.
- **Example**:

  ```json
  "analytics": "UA-XXXXXXXXX-X"
  ```

## Author Information

### 10. **`author`**
- **Description**: Contains information about the author of the site.
- **Fields**:
  - `name`: The author’s name.
  - `url`: A link to the author’s personal page or profile.

- **Example**:

  ```json
  "author": {
    "name": "User Name",
    "url": "https://github.com/user-name"
  }
  ```

## Navigation Menu

### 11. **`navLinks`**
- **Description**: Defines the site navigation menu. Each object in the array represents a navigation link.
- **Structure**:
  - `href`: The URL or path to navigate to.
  - `name`: The display name of the link.

- **Example**:

  ```json
  "navLinks": [
    { "href": "/about", "name": "About" },
    { "href": "/contact", "name": "Contact" }
  ]
  ```

---

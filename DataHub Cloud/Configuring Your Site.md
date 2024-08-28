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

## **`title`**

- **Description**: The title of your site displayed in the navbar (or the sidebar). It's also used as a default value for SEO title on all your site's pages.
- **Example**:
  
  ```json
  "title": "My Awesome Site"
  ```

## **`logo`**

- **Description**: The path to your site's logo.
- **Example**:
 
  ```json
  "logo": "images/logo.png"
  ```

## **`description`**

- **Description**: The site description that will be displayed in the footer. It's also used as a default value for SEO description on all your site's pages.
- **Example**:
  
  ```json
  "description": "Lorem ipsum dolor sit amed."
  ```

### **`showSideBar`**

- **Description**: Enables or disables the sidebar on your site.
- **Usage**: Set this to `true` to display the sidebar, or `false` to hide it and use the default site navbar.
  
  ```json
  "showSideBar": true
  ```
- **Default:** `false`

### **`showEditLink`**

- **Description**: Displays "Edit this page" link at the bottom of each page, allowing users to contribute to your site's GitHub repository.
- **Usage**: Set this to `true` to show the edit link.

  ```json
  "showEditLink": false
  ```
- **Default:** `false`

### **`contentInclude`**

- **Description**: Specifies a list of files or directories to be explicitly included on the site. If not set or if set to `[]`, all files will be included.
- **Example**:
  
  ```json
  "contentInclude": [
    "index.md", 
    "/blog", 
    "/another-folder"
  ] 
  ```

### **`contentExclude`**

- **Description**: Specifies a list of files or directories to be excluded from the site.
- **Example**:
  
  ```json
  "contentExclude": [
    "/blog/trash",
    "/archive",
    "/old-file.md"
  ]
  ```

Can be used along with `contentInclude` to exclude some files/subdirectories from the ones specified in `contentInclude`. For example:

  ```json
  "contentInclude": [
    "/blog"
  ],
  "contentExclude": [
    "/blog/archive"
  ]
  ```

The above configuration will only include `/blog` folder contents, excluding `/blog/archive` subdirectory.

### **`social`**

- **Description**: Configures social media links that will appear in the footer and the navbar.
- **Structure**: Each object in the list contains:
  - `label`: The name of the social media platform (e.g., "facebook"). Currenctly supported are: `youtube`, `facebook`, `linkedin`, `twitter`, `instagram`, `github`, `discord`.
  - `href`: The URL to your profile on that platform.

- **Example**:

  ```json
  "social": [
    { "label": "youtube", "href": "https://youtube.com/user" },
    { "label": "facebook", "href": "https://www.facebook.com/user" }
  ]
  ```

### **`analytics`**

- **Description**: The Google Analytics key used to track user interactions on your site.
- **Example**:

  ```json
  "analytics": "UA-XXXXXXXXX-X"
  ```

### **`author`**
- **Description**: Contains information about the author of the site. If set, will include "Created by {author.name}" in the footer.
- **Fields**:
  - `name`: The author’s name.
  - `url`: A link to the author’s personal page or profile. 🚧

- **Example**:

  ```json
  "author": {
    "name": "User Name",
    "url": "https://github.com/user-name"
  }
  ```

### **`navLinks`**
- **Description**: Defines the site navigation links. Each object in the array represents a navigation link.
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


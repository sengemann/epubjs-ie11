# EPUB.js for IE11 Example

A basic epub.js reader for testing IE11

## Setup

### Dependencies 
- npm 5.6.0
- epubjs v0.3.83
- jQuery 3.3.1

### Nginx

```
server {
    server_name     local.epub.com;
    location / {
        root        <DIRECTORY_TO_YOUR_LOCAL_REPO>;
        index	    index.html;
    }
    error_page  405     =200 $uri;
}
```
### Host

```
127.0.0.1   local.epub.com
```

- Run `npm install`
- Start nginx `sudo nginx`
- Navigate to http://local.epub.com
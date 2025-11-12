Vulnerability Discovery: Directory Listing Enabled at dipersip.riau.go.id

This repository documents the discovery of a Directory Listing Enabled vulnerability on the website https://dipersip.riau.go.id
, specifically in the directory path /wp-content/themes/Dunava/lib/css/.

Tools Used:

Xray: Utilized for scanning the website and detecting vulnerabilities such as Directory Listing.

Vulnerability Description:

The website https://dipersip.riau.go.id
 exposes sensitive information through Directory Listing Enabled on the path /wp-content/themes/Dunava/lib/css/. This allows unauthorized users to view the contents of the directory and access sensitive files, potentially leading to data leakage.

Example of Directory Listing:

The directory at /wp-content/themes/Dunava/lib/css/ is exposed and can be accessed publicly, revealing files such as:

admin-style.css

defaults.css

ie.css

reset.css

Screenshot:

Steps to Reproduce:

Visit the URL: https://dipersip.riau.go.id/wp-content/themes/Dunava/lib/css/
.

Observe the directory listing being publicly exposed with file names and sizes.

This could expose critical assets and configuration files that should be restricted from public access.

Mitigation Recommendations:

Disable Directory Listing on the web server by adjusting the server configuration (e.g., Apache .htaccess or Nginx configuration).

Ensure that sensitive directories are protected with appropriate access controls.

Limit public access to non-essential files, particularly configuration and script files.

License:

This project is intended for educational purposes and ethical hacking only. Always ensure that any security testing is conducted responsibly and with proper authorization from relevant authorities.

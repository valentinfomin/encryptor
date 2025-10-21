## Support
If you like my work, consider supporting me:
[Buy me a coffee ☕](https://www.buymeacoffee.com/watchdogalert)

# encryptor
chrome plugin that encrypt web messages for secure messaging.

Text Encrypt/Decrypt Chrome Extension
This Chrome extension lets you encrypt and decrypt selected text on any webpage using AES-256-CBC encryption with a shared secret keyword. It's simple, secure, and works without popups.
Features

How It Works

Set Keyword: The first time you encrypt/decrypt, a prompt asks for a keyword. It's saved securely and reused.
Encrypt/Decrypt: Select text, use the context menu to encrypt or decrypt, and the text is replaced instantly.
Change Key: Update the keyword anytime via the context menu.
Notifications confirm success or show errors (e.g., "No text selected!" or "Invalid format!").

Installation

Clone or download this repository.
Open Chrome, go to chrome://extensions/, and enable "Developer Mode."
Click "Load unpacked" and select the extension folder.
Ensure crypto-js.min.js and icon files (icon16.png, icon48.png, icon128.png) are in the folder.

Usage

Encrypt: Select text (e.g., "Hello, world!"), right-click, choose "Encrypt Selected Text." The text becomes encrypted (e.g., SALT.IV.CIPHERTEXT).
Decrypt: Select encrypted text, right-click, choose "Decrypt Selected Text" to get the original text back.
Change Key: Right-click, select "Change Encryption Key," and enter a new keyword in the prompt.
Works in text fields (e.g., forms) and on static pages, including WhatsApp Web.

Notes

Security: The keyword is stored in Chrome’s storage. To clear it, use chrome.storage.sync.remove('encryptionKey') in the console or change it via the menu.
Compatibility: Tested on Chrome 66+ with HTTPS sites. Works on WhatsApp Web and most webpages.
Dependencies: Requires crypto-js.min.js for encryption (included).

Files

manifest.json: Extension configuration.
background.js: Manages context menu and notifications.
content.js: Handles encryption, decryption, and text replacement.
crypto-js.min.js: CryptoJS library for AES encryption.
icon*.png: Icons for the extension and notifications.

Feel free to use the plugin as extra leyer of protection for messahngers telegram, whatsupp, email, web chats, facebok etc. 

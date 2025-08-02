# File Smuggling with HTML and JavaScript

This project demonstrates a file smuggling technique using HTML and JavaScript. The code converts a Base64-encoded payload into a downloadable executable file via the browser, leveraging Blob objects and programmatic download triggers.

## How It Works

- The `base64ToArrayBuffer` function converts a Base64 string to a binary array.
- A Blob object is created from this binary data with a generic MIME type.
- The browser is instructed to download this Blob as a file (`update.exe`).
- The technique can bypass some security controls by delivering files through trusted browser features.

## Usage

1. Replace the placeholder string `'PUT YOUR CODE'` with your Base64-encoded payload.
2. Open the HTML file in a modern browser.
3. The browser will automatically trigger the download of the executable file.

## Security Notice

This technique can be used for malicious purposes, such as delivering malware. Use it only for educational or authorized testing purposes. Always ensure you have permission before testing such code.

## Security and Protection Tips

- **Use updated antivirus and endpoint protection** solutions that can detect suspicious downloads and behaviors.
- **Configure email and web gateways** to inspect and block suspicious file downloads, especially those triggered via browser scripts.
- **Educate users** about the risks of downloading files from untrusted or unknown sources.
- **Use browser security features** like disabling automatic downloads or scripts from untrusted websites.
- **Implement Content Security Policy (CSP)** headers on your web applications to restrict unauthorized script execution.
- **Monitor network traffic** for unusual or unexpected file download activities.

## Disclaimer

The author is not responsible for any misuse of this code.

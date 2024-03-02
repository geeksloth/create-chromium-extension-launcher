# create-chromium-extension-launcher
A guideline to make a launcher to the Chromium-based browser's extension for Debian distros Linux.

Full tutorial video here:

[![GeekSloth's using LINE in Kali Linux](https://img.youtube.com/vi/ZUuXnljSLNI/0.jpg)](https://www.youtube.com/watch?v=ZUuXnljSLNI)


# Briefly procedures
1. Install Chromium-based browser, e.g., Brave or Google Chrome, on your Debian-based distros.
2. Install your extension via [https://chromewebstore.google.com/](https://chromewebstore.google.com/). Then click the *three dots* menu of the extension, and choose *manage extension*. 
3. Launching it from terminal by copy the *extension id* and replace it at `<<extension_id>>` in the below command. Don't forget to change the `brave-browser` to your browser binary, in my case, it is Brave browser.
```bash
brave-browser --app=chrome-extension://<<extension_id>>/index.html
```

4. Create the shortcuts
- Right click on the desktop, add new launcher, then add the command and configure what ever your want.
- Add the launcher you created to panel or dock.
- Copy it in to `/usr/share/applications` directory by using the *sudo* user.

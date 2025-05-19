# 📱 Instagram Unfollowers

This version utilizes the Instagram API for better performance.  

## 🖥️ Desktop Usage

1. Copy the code from: 

<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>نسخ الرابط</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f6f6f6;
      padding: 30px;
      text-align: center;
    }

    #linkBox {
      background: #ffffff;
      padding: 15px;
      border: 1px solid #ccc;
      border-radius: 8px;
      display: inline-block;
      margin-bottom: 15px;
      font-size: 18px;
    }

    #copyBtn {
      background-color: #4CAF50;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
    }

    #copyBtn:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <h2>رابط الكود</h2>

  <div id="linkBox">
    <a href="https://pastebin.com/iW9VW3Qv" target="_blank" id="linkText">
      https://pastebin.com/iW9VW3Qv
    </a>
  </div>

  <br>
  <button id="copyBtn">📋 نسخ الرابط</button>

  <script>
    document.getElementById("copyBtn").addEventListener("click", function () {
      const link = document.getElementById("linkText").href;
      navigator.clipboard.writeText(link).then(() => {
        alert("✅ تم نسخ الرابط!");
      }).catch(err =


3. Go to Instagram website and log in to your account

4. Open the developer console:
   - Windows: `Ctrl + Shift + J`
   - Mac OS: `⌘ + ⌥ + I`

5. Paste the code and you'll see this interface:

    <img src="./assets/initial.png" alt="Initial screen" />

6. Click "RUN" to start scanning

7. After scanning completes, you'll see the results:

    <img src="./assets/results.png" alt="Results screen" />

8. 🤍 Whitelist users by clicking their profile image

9. ✅ Select users to unfollow using the checkboxes

10. ⚙️ Customize script timings via the "Settings" button:

    <img src="./assets/settings.png" alt="Settings screen" />

## 📱 Mobile Usage

For Android users who want to use it on mobile:

1. Download the latest version of [Eruda Android Browser](https://github.com/liriliri/eruda-android/releases/)
2. Open Instagram web through the Eruda browser
3. Follow the same steps as desktop (the console will be automatically available when clicking the eruda icon)

## ⚡ Performance Notes

- Processing time increases with the number of users to check
- Script works on both Chromium and Firefox-based browsers
- The script takes a few more seconds to load on mobile

## 🛠️ Development

- Node version: 16.14.0 (If using nvm, run `nvm use`)
- After modifying `main.tsx`, run the "build" command to format, compress, and convert your code
- Automatic re-building can be done using nodemon build-dev

## ⚖️ Legal & License

**Disclaimer:** This tool is not affiliated, associated, authorized, endorsed by, or officially connected with Instagram.

⚠️ Use at your own risk!

📜 Licensed under the [MIT License](LICENSE)
- ✅ Free to use, copy, and modify
- 🤝 Open source and community-friendly
- 📋 See [LICENSE](LICENSE) file for full terms

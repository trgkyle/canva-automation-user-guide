[![Download Here](https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge)](https://chromewebstore.google.com/detail/canva-automation-auto-can/henpgladfodcidlnpdadgdlamegalije)

# 🚀 Canva Automation v1.0.1 - canva.com AI Automation [![Tiếng Việt](https://img.shields.io/badge/Tiếng%20Việt-green)](README_vi.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md)

**Canva Automation** is a powerful productivity tool that automates your creative workflow on Canva AI (`canva.com`). Instead of manually copying and entering prompts one by one, you can queue dozens or hundreds of prompts to automatically generate batch responses, images, and text outputs at scale.

-----

## ✨ Key Features

* **🚀 Batch Processing:** Queue large sets of prompts and let the extension handle the automation process, including prompt submission and content generation on Canva.
* **💬 Text Processing (Text-to-Text):** Process multiple text prompts in sequence, combining text generation tasks or starting new conversation threads automatically.
* **💬 Ingredients-to-Text (Image+Text input):** Provide prompt descriptions alongside uploaded images (Ingredients) to generate structured text and analysis.
* **🖼️ Text-to-Image Batching:** Generate multiple high-quality images with full support for various aspect ratios (16:9, 9:16, 1:1, 3:4, 4:3).
* **🖼️ Image-to-Image:** Transform or enhance existing images using AI with custom text prompts.
* **⚙️ Professional Automation Controls:**
    * **Random Delays:** Introduce smart delays between prompt submissions to handle rate limits gracefully.
    * **Auto Download:** Automatically download generated images and outputs upon completion.
    * **Auto Rename:** Automatically rename downloaded files based on project settings.
* **📊 Side Panel Queue Monitoring:** Monitor progress with active prompt tracking, delay count-down, and a visual status bar in the Chrome Side Panel.
* **📂 Organized File Management:** Download files into customized subfolders based on your projects under Chrome's download folder.
* **📄 Spreadsheet Import:** Import batch prompts directly from `.txt`, `.xlsx`, or `.csv` files with column preview.
* **🎯 Range Run:** Select and execute a specific subset of prompts (e.g. from prompt #5 to #20).
* **🌐 Multi-language Support:** English, Tiếng Việt, 中文, 한국어, Español, 日本語.

-----

## 📥 Installation

### Method 1: Chrome Web Store (Recommended)
1. Visit the [Chrome Web Store](https://chromewebstore.google.com/detail/canva-automation-auto-can/henpgladfodcidlnpdadgdlamegalije) and click **Add to Chrome**.

---

## 📖 User Guide

### Getting Started

1. **Navigate to Canva AI**
   - Open [canva.com](https://www.canva.com/ai).
   - Ensure you are logged into your Canva account.

2. **Open the Extension**
   - Click the extension icon in the Chrome toolbar. We recommend pinning it for quick access.
   - The side panel will open.

3. **Configure Batch Settings**
   - In the **Control** tab, set the **Save to folder** name to organize your downloads.
   - In the **Setting** tab, customize your default modes, aspect ratios, download options, and random delays.

4. **Select a Mode**
   - Click one of the mode buttons: **Text Processing**, **Ingredients to Text**, **Text to Image**, or **Image to Image**.

---

### Mode Instructions

#### 1. Text Processing Mode
1. Select **Text Processing** mode.
2. Enter prompts in the text box (separate prompts with a **blank line**).
3. Alternatively, click **Upload .txt file** or **Upload .xlsx / .csv** to import prompts.
4. (Optional) Use **Range Run** to select specific prompt indices to execute.
5. Click **Run** to start processing text prompts automatically.

**Example Prompt:**
```
Write a compelling product description for a minimalist bamboo water bottle.

Create 5 engaging social media post ideas for a eco-friendly coffee brand.

Generate a summary of modern UI/UX design trends for 2026.
```

#### 2. Ingredients-to-Text Mode
1. Select **Ingredients to Text** mode.
2. Drag & drop or click to upload your source image(s) (PNG, JPG, GIF up to 10MB each).
3. Input prompts describing your analysis request (separated by blank lines).
4. (Optional) Toggle **Auto-add character images** to match images with character names in prompts based on filenames.
5. Click **Run**.

#### 3. Text-to-Image Mode
1. Select **Text to Image** mode.
2. Enter detailed prompts separated by blank lines.
3. Configure the desired **Default Aspect Ratio** (16:9, 9:16, 1:1, 3:4, 4:3) and **Image Model** in Settings.
4. Set **Outputs Image per Prompt** (1 to 50) in Settings.
5. Click **Run** to batch generate images.

**Example Prompt:**
```
A futuristic cyberpunk city with neon lights glowing in rain, cinematic lighting, ultra-detailed.

A serene Japanese garden during autumn with vibrant red maple leaves and a koi pond.
```

#### 4. Image-to-Image Mode
1. Select **Image to Image** mode.
2. Upload the source image(s) you wish to modify.
3. Enter text prompts describing the modifications or style adjustments.
4. Set **Default Image Mode Option** in Settings (*New Image* or *Edit Image* to chain outputs).
5. Click **Run**.

---

## ⚙️ Settings Configuration

Access the **Setting** tab in the side panel to fine-tune automation behavior:

* **Default Mode:** Set the default creation mode when launching the extension.
* **Default Aspect Ratio:** Choose from 16:9 (YouTube), 9:16 (Shorts/Reels), 1:1 (Square), 3:4 (Portrait), or 4:3 (Landscape).
* **Outputs Image per Prompt:** Specify how many images to generate per prompt (1 to 50).
* **Concurrent Prompts:** Number of prompts to process simultaneously.
* **Random Delay:** Set minimum and maximum wait time (in seconds) between handling prompts.
* **Image Model:** Select the AI model for image generation tasks.
* **Default Chat Mode Option:** Choose default chat mode (*New Chat* or *Current Chat* to combine responses).
* **Default Image Mode Option:** Choose default input mode for images (*New Image* or *Edit Image* for chaining).
* **Max Retries on Failure:** Specify retry attempts (1 to 20) if content generation fails.
* **Auto Download Quality (Image):** Set auto-download quality (*No Download*, *1k*).
* **Language:** Switch between English, Tiếng Việt, 中文, 한국어, Español, and 日本語.
* **Download Settings:** Organizes generated outputs into separate project subfolders under Chrome's Download directory.

---

## 💡 Tips & Best Practices

1. **Handling Rate Limits:** If Canva limits your account activity, increase the **Random Delay** between prompts.
2. **Batch Import:** Use the `.xlsx / .csv` import tool to easily preview and import prompts from spreadsheet columns.
3. **Range Execution:** Use the range start/end inputs on the Run button to process subsets of a large prompt list without re-editing.
4. **Auto-naming & Folders:** Name your project folder in the Control tab so that all files are grouped together cleanly in Chrome's Download directory.

---

## 🔧 Troubleshooting

| Issue | Solution |
| :--- | :--- |
| **Extension Not Active** | Make sure you are on [canva.com/ai](https://www.canva.com/ai). Refresh the page (F5 or Ctrl+R) if needed. |
| **Generation Errors** | Click the **Fix Error** button in the extension. The extension will automatically retry up to your configured Max Retries. |
| **Downloads Not Working** | Turn **OFF** the "Ask where to save each file before downloading" setting in your Chrome browser settings. |
| **Authentication / Plan Issues** | Verify you are signed in to both `canva.com` and your extension plan account (via the Plan Banner). |

---

## 🔒 Privacy & Data

* **Local Processing:** All automation actions and page interaction scripts run locally within your browser sandbox.
* **No External Storage:** We do not collect, monitor, or store your prompts, uploaded images, or generated files.
* **Secure Sync:** Settings are saved directly within Chrome's local storage and synced automatically across browser tabs.

---

## 📞 Support

- **Author:** Trường Nguyễn
- **Website:** [kylenguyen.me](https://kylenguyen.me)
- **Feedback:** Use the **Debug Logs** tab (or bug report modal) in the extension to copy debug logs and send them to our support channels.

---

## 📦 Version

Current version: **1.0.1**

---

## 📜 License

Copyright © 2026 **Trường Nguyễn**. All Rights Reserved.

This software is proprietary. Unauthorized copying, modification, or distribution is prohibited.

---

**Made with ❤️ by Trường Nguyễn**

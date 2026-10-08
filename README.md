[![Download Here](https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge)](https://chromewebstore.google.com/detail/canva-automation-auto-can/henpgladfodcidlnpdadgdlamegalije)

# 🚀 Canva Automation v1.0.1 - canva.com AI Automation [![Tiếng Việt](https://img.shields.io/badge/Tiếng%20Việt-green)](README_vi.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md)

**Canva Automation** is a powerful productivity tool that automates your creative workflow on Canva AI (`canva.com`). Instead of manually copying and entering prompts one by one, you can queue dozens or hundreds of prompts to automatically generate batch responses, images, and text outputs at scale.

-----

## ✨ Key Features

* **🚀 Batch Processing:** Queue large sets of prompts and let the extension handle the automation process, including prompt submission and content generation on Canva.
* **🧩 Workflow (visual drag-and-drop editor):** Connect prompts, images and generators on a canvas — e.g. generate images, then edit those images with more prompts automatically. Save several workflows, run one node or all of them, import/export them as files.
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

### 🧩 Workflow (Visual Drag-and-Drop Editor)

Workflow is a visual drag-and-drop editor for flows with several steps — for example: generate a few images, then edit those images with more prompts. It opens in its own window and runs on your open Canva AI tab.

#### Open it

* Click **Workflow** in the Control tab (bottom row).
* Already typed prompts or uploaded images in the side panel? Hover **Workflow** and click **Convert to workflow**: your prompts, each prompt's mode and your images become nodes in the editor, ready to run.

#### The screen

| Area | What it holds |
| :--- | :--- |
| **Left** | **Nodes** (click or drag one onto the canvas) and **Your workflows** (all saved workflows) |
| **Top bar** | The canvas tools: Undo/Redo, **Auto arrange**, fit view, **Example**, clear. On the right: the **Details** button, **Shortcuts** and the Canva AI tab status |
| **Canvas** | Your nodes. Top-left: **Run all** (and **Stop** while running) and **Enable background mode** |

The **Details** button shows what needs attention: **Issues (n)** in red/yellow when something blocks a run, **Running 3/8** while generating. Click it to open a panel with the issues (click one to jump to the node), live progress, the run plan and the settings it uses.

#### Nodes

| Node | What it does |
| :--- | :--- |
| **Enter prompt** | One or more prompts, separated by a **blank line** |
| **Upload image** | Your images (drop files on it). Hover an image: 🔍 to view it larger, ✕ to remove it, the grip in the corner to drag it to another position. The order (or the sort menu) decides which prompt gets which image |
| **Generate Image** | Text to Image, or Image to Image when images are connected. Options: **Image Mode per Prompt**, **Max Input Images per Prompt**, **Auto-add character images** |

Generate nodes are named automatically from their first prompt (`image_…` / `video_…`). Each prompt row shows the images it will receive, so you can check before running. Their preview takes the **aspect ratio** from the settings (a 9:16 node is narrower and taller).

#### Connect nodes

Drag from the round handle on the right of a node and **drop it anywhere on the other node** — the right input is picked for you. Nodes that accept the connection light up while you drag.

| From | To | Meaning |
| :--- | :--- | :--- |
| Enter prompt | Generate Image | The prompts to generate |
| Upload image | Generate Image | Reference images, start frames or components |
| Generate Image | Generate Image | The **generated images** become that node's input (it runs after the images are ready) |

#### Run

* **Run all** (top-left, or `Ctrl/⌘ + Enter`) runs the whole workflow in the right order: nodes waiting for generated images start automatically once those images exist.
* If **Run all** is disabled, the top bar shows **Issues (n)**: click it to see what to fix.
* Each Generate node also has its own **Run** button to run only that node. It is disabled until the nodes it depends on have finished (hover to see why).
* **Stop** cancels what is still running.
* While running, the connections into the node that is generating light up and flow, so you can see where the workflow is.

> ⚠️ **Chrome pauses Canva AI when its tab isn't visible** (for example when the workflow window covers it full screen). Click **Enable background mode** (under **Run all** in the workflow, or in the side panel), then pick the Canva AI tab in Chrome's dialog. This shares the Canva AI tab (nothing is recorded or sent anywhere) so it keeps generating behind other windows. The green **Running in background** badge shows it's on; click ✕ to stop it.

#### Results

Results appear inside each Generate node. Hover a result: 🔍 opens it large, ✕ removes it (the eraser clears all results of the node). Files are still downloaded as usual.

The next node uses the **first result of each prompt**. To choose which one, drag a result by the grip in its top-left corner onto another result to swap them.

#### Manage workflows

Under **Your workflows** (left): **New**, **Import**, and for each workflow the **⋯** menu — **Rename** (or double-click the name), **Duplicate**, **Export**, **Delete**. Everything is saved automatically.

* **Export** downloads a `.json` file. It starts with `//` comment lines that describe every node, property and connection, so you can give the file to an AI assistant and ask it to write new workflows. The comment lines are removed on import.
* **Import** a file with the button, or simply **drag the `.json` file onto the canvas**.

#### Editing shortcuts

Click **Shortcuts** in the top bar (or press `?`) to see them all.

| Action | Keys |
| :--- | :--- |
| Undo / Redo | `Ctrl/⌘ + Z` / `Ctrl/⌘ + Shift + Z` |
| Copy / Cut / Paste nodes (also into another workflow) | `Ctrl/⌘ + C / X / V` |
| Duplicate selection | `Ctrl/⌘ + D` |
| Select all / Add to selection / Box select | `Ctrl/⌘ + A` / `Ctrl/⌘ + click` / `Shift + drag` |
| Auto arrange | `Shift + A` |
| Delete selected | `Delete` |
| Run all / Run in background | `Ctrl/⌘ + Enter` / `Ctrl/⌘ + Shift + Enter` |

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
| **Workflow: generation stays at "Generating" forever** | Chrome paused the hidden Canva AI tab. Turn on **Enable background mode** (or **Run in background**), or keep Canva AI visible. |
| **Workflow: a node's Run button is disabled** | Hover it: run the node it depends on first, or fix the issue shown (e.g. no prompt connected). |
| **Workflow: Run all is disabled** | Click **Issues (n)** in the top bar to see what to fix; click an issue to jump to its node. |
| **Workflow: "No Canva AI tab found"** | Open [Canva AI](https://www.canva.com/ai) in a tab (the green dot in the top bar shows it's connected). |

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

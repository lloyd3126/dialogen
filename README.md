# Gemini 圖文生成工具 / Gemini Dialogue Generator

[中文](#中文說明) | [English](#english)

---

## 中文說明

### 簡介

一個簡單易用的 Gemini AI 圖文生成工具，讓你可以透過自訂對話內容來控制 AI 的回應風格。支援文字和圖片的生成，並提供靈活的對話序列編輯功能。

### 功能特色

- ✨ **對話式介面**：使用對話序列來引導 AI 生成內容
- 🎨 **圖片生成**：使用 Gemini 2.0 Pro Image Preview 生成高品質圖片
- 📝 **文字生成**：使用 Gemini 2.0 Flash 快速生成文字內容
- 🔄 **靈活編輯**：可自由新增、刪除、移動對話內容
- 🖼️ **多種圖片設定**：支援多種長寬比（1:1, 2:3, 3:2, 16:9, 9:16）和解析度（1K, 2K, 4K）
- 💾 **自動儲存**：對話內容自動儲存至瀏覽器，下次開啟自動載入
- 📥 **下載功能**：可下載生成的圖片和文字內容

### 使用方式

1. **取得 API Key**
   - 前往 [Google AI Studio](https://aistudio.google.com/apikey) 取得你的 Gemini API Key
   - 在頁面頂部輸入 API Key（會自動儲存到瀏覽器）

2. **建立對話內容**
   - 點擊「新增」按鈕加入新的對話項目
   - 選擇角色：「請求」（使用者）或「回應」（模型）
   - 選擇類型：「文字」或「圖片」
   - 輸入內容或上傳圖片

3. **生成內容**
   - 在使用者項目中，點擊「生成圖片」或「生成文字」按鈕
   - 等待 AI 處理（會顯示處理時間）
   - 生成的內容會自動加入為模型回應項目

4. **調整圖片設定**
   - 點擊長寬比按鈕（預設 1:1）循環切換不同比例
   - 點擊解析度按鈕（預設 1K）切換圖片大小

5. **下載結果**
   - 在模型回應項目中，點擊「下載」按鈕
   - 圖片會下載為 PNG 格式
   - 文字會下載為 TXT 格式

### 線上體驗

🌐 訪問 [dialogen.nien.cc](https://dialogen.nien.cc) 立即使用

### 技術架構

- **前端**：原生 JavaScript、HTML、CSS
- **API**：Google Gemini API
  - 圖片生成：`gemini-2.0-pro-image-preview`
  - 文字生成：`gemini-2.0-flash-preview`
- **儲存**：瀏覽器 localStorage

### 本地開發

```bash
# 克隆專案
git clone https://github.com/lloyd3126/dialogen.git

# 進入目錄
cd dialogen

# 使用任意 HTTP 伺服器啟動（例如 Python）
python -m http.server 8000

# 或使用 Node.js
npx serve

# 開啟瀏覽器訪問
# http://localhost:8000
```

### 注意事項

- 需要有效的 Google Gemini API Key
- API 使用可能產生費用，請參考 [Google AI 定價](https://ai.google.dev/pricing)
- 圖片生成功能需要使用支援的模型版本
- 所有資料都儲存在本地瀏覽器，不會上傳到伺服器

### 授權

MIT License

---

## English

### Introduction

A simple and intuitive Gemini AI content generation tool that allows you to control AI response style through custom dialogue sequences. Supports both text and image generation with flexible dialogue editing capabilities.

### Features

- ✨ **Dialogue Interface**: Guide AI content generation using conversation sequences
- 🎨 **Image Generation**: Generate high-quality images using Gemini 2.0 Pro Image Preview
- 📝 **Text Generation**: Fast text generation using Gemini 2.0 Flash
- 🔄 **Flexible Editing**: Freely add, delete, and rearrange dialogue content
- 🖼️ **Multiple Image Settings**: Support various aspect ratios (1:1, 2:3, 3:2, 16:9, 9:16) and resolutions (1K, 2K, 4K)
- 💾 **Auto-save**: Dialogue content automatically saved to browser and restored on next visit
- 📥 **Download Function**: Download generated images and text content

### How to Use

1. **Get API Key**
   - Visit [Google AI Studio](https://aistudio.google.com/apikey) to get your Gemini API Key
   - Enter the API Key at the top of the page (automatically saved to browser)

2. **Create Dialogue Content**
   - Click "Add" button to create new dialogue items
   - Select role: "Request" (user) or "Response" (model)
   - Select type: "Text" or "Image"
   - Enter content or upload image

3. **Generate Content**
   - In user items, click "Generate Image" or "Generate Text" button
   - Wait for AI processing (processing time will be displayed)
   - Generated content will be automatically added as model response item

4. **Adjust Image Settings**
   - Click aspect ratio button (default 1:1) to cycle through different ratios
   - Click resolution button (default 1K) to switch image sizes

5. **Download Results**
   - In model response items, click "Download" button
   - Images will be downloaded as PNG format
   - Text will be downloaded as TXT format

### Live Demo

🌐 Visit [dialogen.nien.cc](https://dialogen.nien.cc) to try it now

### Technical Stack

- **Frontend**: Vanilla JavaScript, HTML, CSS
- **API**: Google Gemini API
  - Image generation: `gemini-2.0-pro-image-preview`
  - Text generation: `gemini-2.0-flash-preview`
- **Storage**: Browser localStorage

### Local Development

```bash
# Clone the repository
git clone https://github.com/lloyd3126/dialogen.git

# Enter directory
cd dialogen

# Start with any HTTP server (e.g., Python)
python -m http.server 8000

# Or use Node.js
npx serve

# Open browser and visit
# http://localhost:8000
```

### Notes

- Requires a valid Google Gemini API Key
- API usage may incur costs, please refer to [Google AI Pricing](https://ai.google.dev/pricing)
- Image generation requires supported model versions
- All data is stored locally in the browser and not uploaded to any server

### License

MIT License

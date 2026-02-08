# AliToDaraz - Alibaba to Daraz Price Comparison Chrome Extension 🛍️

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/Ashiq3/alitodaraz/releases)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-orange.svg)](https://github.com/Ashiq3/alitodaraz)
[![Made with React](https://img.shields.io/badge/Made%20with-React-61DAFB.svg)](https://reactjs.org/)
[![Stars](https://img.shields.io/github/stars/Ashiq3/alitodaraz?style=social)](https://github.com/Ashiq3/alitodaraz/stargazers)

**The Ultimate Price Comparison Tool for Dropshippers in Bangladesh**

Compare Alibaba products with Daraz Bangladesh prices instantly using Visual Search AI technology

[🚀 Installation](#installation) • [📖 Usage](#how-to-use) • [🛠️ Development](#development-setup) • [🤝 Contributing](#contributing)

---

## 📋 Overview

**AliToDaraz** is a powerful, open-source Chrome browser extension designed specifically for dropshippers, e-commerce entrepreneurs, and online shoppers in Bangladesh. It enables instant price comparison between **Alibaba.com** (global wholesale marketplace) and **Daraz Bangladesh** (leading local e-commerce platform) using advanced **Visual Search technology** powered by Google Lens AI.

### Why AliToDaraz?

- 🎯 **Find Exact Product Matches**: Even when product titles are completely different between platforms
- 💰 **Verify Profitability**: Compare wholesale prices from Alibaba with retail prices on Daraz
- ⏱️ **Save Time**: No more manual searching and copying product names
- 🔒 **Privacy First**: No data collection, runs 100% locally in your browser
- 🆓 **100% Free**: Open source and free to use forever

![AliToDaraz Chrome Extension Screenshot](https://via.placeholder.com/800x400?text=AliToDaraz+Extension+Screenshot)
*AliToDaraz Sidebar showing price comparison between Alibaba and Daraz*

---

## ✨ Key Features

### 🔍 Visual Search (Primary)
Our revolutionary Visual Search technology finds products by image matching:
- Upload any product image from Alibaba
- AI-powered matching finds identical products on Daraz
- Works even when product titles are completely different
- No keyword guessing required!

### 🕵️ Hidden Background Processing
- Visual search runs invisibly in the background
- No annoying popup tabs or windows
- Seamless user experience

### ⚡ Instant Price Comparison
- View Daraz prices directly on the Alibaba product page
- Real-time price updates
- Side-by-side comparison in elegant sidebar

### 🇧🇩 Bangladesh Focused
- Optimized specifically for **Daraz Bangladesh** (daraz.com.bd)
- Local currency support (BDT/৳)
- Designed for Bangladeshi dropshippers and resellers

### 🔒 Privacy & Security
- **No data collection**: We don't track your browsing
- **No external servers**: Everything runs locally in your browser
- **No personal information**: No login required, no account needed
- **Open source**: Full transparency - see exactly what the code does

---

## 🚀 Installation

### Method 1: Chrome Web Store (Coming Soon)
The extension will be available on Chrome Web Store soon. Stay tuned!

### Method 2: Manual Installation (Developer Mode)
Since this is an open-source tool, you can install it manually:

1. **Download** the latest release: `ali-to-daraz-extension.zip` from the [Releases page](https://github.com/Ashiq3/alitodaraz/releases)
2. **Extract** the zip file to a folder on your computer
3. Open Chrome and navigate to `chrome://extensions`
4. Enable **Developer Mode** (toggle in top-right corner)
5. Click **Load Unpacked** button
6. Select the extracted folder
7. Done! You should see the **AD** icon in your Chrome toolbar

**Note**: You'll need to keep Developer Mode enabled to use the extension.

---

## 📖 How to Use

### Step-by-Step Guide

1. **Navigate** to any product page on [Alibaba.com](https://www.alibaba.com/)

2. **Look for the floating button** - You'll see a **"Compare on Daraz"** button at the bottom-right corner of the page

3. **Click the button** - The sidebar will slide open automatically

4. **Automatic Search** - The extension will:
   - Extract the product image from Alibaba
   - Perform Visual Search on Daraz using Google Lens AI
   - Display matching products with prices

5. **Compare Prices** - Review the results and verify your profit margins!

### Alternative: Right-Click Search
You can also right-click on any selected text and choose **"Compare on Daraz"** from the context menu.

---

## 🛠️ Development Setup

Want to contribute or customize the extension? Here's how to set up the project locally:

### Prerequisites

- **Node.js** v18 or higher
- **pnpm** package manager (recommended)
- **Git** for version control

### Installation Steps

```bash
# 1. Clone the repository
git clone https://github.com/Ashiq3/alitodaraz.git
cd alitodaraz/ali-to-daraz-extension

# 2. Install dependencies
pnpm install

# 3. Start development server
pnpm dev
# This starts Vite dev server with hot reload
```

### Build for Production

```bash
# Create production build
pnpm build

# This generates the 'dist' folder ready for Chrome extension deployment
```

### Run Tests

```bash
# Run unit tests
pnpm test

# Run end-to-end tests
pnpm test:e2e

# Run linter
pnpm lint
```

---

## 🏗️ Architecture

### Tech Stack

- **Frontend**: React 18 + Tailwind CSS 3
- **Build Tool**: Vite 5
- **Extension**: Chrome Manifest V3
- **Testing**: Vitest (unit) + Playwright (E2E)
- **Package Manager**: pnpm

### How It Works

1. **Content Script** (`content.js`): Injects floating button and sidebar iframe into Alibaba pages
2. **Background Script** (`background.js`): Handles Visual Search via Google Lens API and Daraz API calls
3. **Sidebar UI** (`Sidebar.jsx`): React-based floating panel for displaying comparison results
4. **Smart Parser** (`parser.js`): Extracts structured data from Daraz API responses
5. **Title Cleaner** (`cleaner.js`): Intelligently strips B2B jargon from Alibaba titles

---

## 🤝 Contributing

We welcome contributions! Please check out [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

### Quick Start for Contributors

1. **Fork** the repository
2. **Create** your feature branch: `git checkout -b feature/AmazingFeature`
3. **Commit** your changes: `git commit -m 'Add some AmazingFeature'`
4. **Push** to the branch: `git push origin feature/AmazingFeature`
5. **Open** a Pull Request

### Contribution Areas

- 🐛 **Bug fixes**
- ✨ **New features**
- 📝 **Documentation improvements**
- 🎨 **UI/UX enhancements**
- 🌐 **Internationalization** (support for other countries)
- 🧪 **Test coverage**

---

## 📊 Use Cases

### For Dropshippers
- Verify product availability on Daraz before ordering from Alibaba
- Calculate profit margins instantly
- Find trending products with price arbitrage opportunities

### For Online Resellers
- Compare wholesale vs retail prices
- Identify high-margin products
- Research market competition

### For Shoppers
- Find the best deals across platforms
- Verify if Daraz prices are fair compared to wholesale
- Discover similar products at better prices

---

## 🔍 SEO Keywords

`alibaba-daraz-price-comparison` `chrome-extension` `dropshipping-tool` `bangladesh-ecommerce` `visual-search` `price-tracker` `alibaba-scraper` `daraz-bangladesh` `product-comparison` `arbitrage-tool` `google-lens` `ecommerce-automation` `wholesale-price-checker`

---

## 🛡️ Privacy Policy

**Last Updated**: January 22, 2026

### What We Collect
- **Product Information**: When you use the extension on Alibaba.com, we temporarily read product titles and images from the current page to perform searches on Daraz.
- **No Personal Data**: We do NOT collect any personal information, login credentials, or browsing history.

### What We Don't Collect
- ❌ Personal identification information
- ❌ Email addresses or contact information
- ❌ Browsing history
- ❌ Keystrokes or form data
- ❌ Payment information
- ❌ Location data

### Data Storage
- **Local Only**: All data is stored locally in your browser using Chrome's storage API.
- **No External Servers**: We do not send any data to external servers owned by us.
- **Third-Party Services**: We use Google Lens for visual search. Please refer to [Google's Privacy Policy](https://policies.google.com/privacy) for their data practices.

For full details, see [PRIVACY_POLICY.md](ali-to-daraz-extension/PRIVACY_POLICY.md)

---

## 📄 License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for more information.

---

## 🙏 Acknowledgments

- Thanks to all contributors who have helped improve this project
- Special thanks to the open-source community
- Built with ❤️ for the Bangladesh dropshipping community

---

## 📞 Support & Contact

- 🐛 **Bug Reports**: [Open an Issue](https://github.com/Ashiq3/alitodaraz/issues)
- 💡 **Feature Requests**: [Open an Issue](https://github.com/Ashiq3/alitodaraz/issues)
- 📧 **General Inquiries**: Open an issue on GitHub
- ⭐ **Star this repo** if you find it helpful!

---

<div align="center">

**Made with ❤️ by [Ashiqe Bin Rahman](https://github.com/Ashiq3)**

[⭐ Star this project](https://github.com/Ashiq3/alitodaraz) • [🍴 Fork it](https://github.com/Ashiq3/alitodaraz/fork) • [🐛 Report Bug](https://github.com/Ashiq3/alitodaraz/issues)

</div>

---

**Disclaimer**: This project is not affiliated with Alibaba Group or Daraz Group. It is a third-party tool developed for educational and productivity purposes.

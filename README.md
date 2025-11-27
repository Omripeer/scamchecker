# Hebrew Phishing & Scam Website Checker
A simple, user-friendly, and free web application designed to help users, especially older adults and mentally disabled individuals, check if a website, phone number, or SMS message is potentially a phishing or scam. The interface is in Hebrew and English, built for maximum clarity and ease of use.

➡️ Live Demo Link (Replace this with your actual GitHub Pages URL after deploying!)

## 🌟 Project Purpose
The internet can be a dangerous place, with many fraudulent websites and scam messages trying to trick people into giving away personal information. This tool was created to provide a quick and easy first line of defense. Users can:
- Check URLs/websites against multiple security databases
- Verify phone numbers for spam/scam patterns
- Analyze SMS messages for suspicious content

The project is designed with accessibility in mind, featuring large text, high-contrast colors, and a simple, single-purpose interface. This is a **NON-PROFIT** project created to protect vulnerable populations from online scams.

## ✨ Features
 * 🛡️ **Multi-Source URL Safety Check**: 
   - Google Safe Browsing API - Checks against known malware, phishing, and unwanted software
   - PhishTank API - Community-driven phishing database (when CORS permits)
   - Local Pattern Analysis - Detects typosquatting, suspicious TLDs, and URL patterns
 * 📱 **Phone Number Spam Detection**:
   - Local pattern analysis for Israeli and international spam patterns
   - Premium/VoIP number detection
   - Known scam country code detection
   - Optional IPQualityScore API integration (free tier: 5,000/month)
 * 💬 **SMS/Message Analysis**: 
   - Enhanced keyword detection for Hebrew and English scam phrases
   - Common phishing pattern recognition
 * 📈 **Top 10 Searched Sites**: A live-updating list of the most frequently checked URLs
 * 🔢 **Visitor Counter**: Shows community engagement
 * 👴 **User-Friendly Design**: Clean, responsive, accessible interface with Tailwind CSS
 * 🌐 **Bilingual Support**: Hebrew and English interface
 * 📦 **Self-Contained**: Single index.html file for easy deployment

## 🛠️ Technology Stack
 * **Frontend**: HTML, Tailwind CSS
 * **Backend & Database**: Firebase (Firestore DB and Anonymous Authentication)
 * **Security APIs**:
   - Google Safe Browsing API V4 (free, unlimited for non-commercial use)
   - PhishTank API (free, community-driven)
   - Local heuristic analysis

## 🔌 API Information

### URL/Website Checking

1. **Google Safe Browsing API** (Primary)
   - **Cost**: Free for non-commercial use
   - **Limits**: 10,000 requests/day
   - **Documentation**: https://developers.google.com/safe-browsing
   - **Coverage**: Malware, phishing, unwanted software, potentially harmful applications

2. **PhishTank API** (Secondary)
   - **Cost**: Free
   - **Limits**: Unlimited for lookups
   - **Documentation**: https://www.phishtank.com/api_info.php
   - **Coverage**: Community-reported phishing sites

3. **Local Pattern Analysis**
   - Typosquatting detection (fake versions of popular domains)
   - Suspicious TLD detection (.tk, .ml, .xyz, etc.)
   - URL structure analysis

### Phone Number Checking

1. **Local Pattern Analysis** (Built-in)
   - Israeli premium number detection (1-900, 1-901, 1-902)
   - VoIP range detection (072, 073, 076-079)
   - International scam origin detection
   - Suspicious pattern detection

2. **IPQualityScore API** (Optional Enhancement)
   - **Cost**: Free tier with 5,000 requests/month
   - **Documentation**: https://www.ipqualityscore.com/documentation/phone-number-validation-api
   - **To Enable**: Set `window.IPQS_API_KEY = 'your-api-key';` before loading the page

## 🚀 Getting Started

1. Clone this repository
2. Open `index.html` in a browser, or deploy to GitHub Pages
3. (Optional) Configure your own API keys for enhanced functionality

### Optional API Key Configuration

To enable IPQualityScore phone number checking, add the following before the page loads:
```html
<script>
  window.IPQS_API_KEY = 'your-ipqualityscore-api-key';
</script>
```

## 📋 License
This project is open source and free to use for non-commercial purposes, especially for protecting vulnerable populations from online scams.

## 🤝 Contributing
Contributions are welcome! Please feel free to submit issues and pull requests to help improve protection for vulnerable users.

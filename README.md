# Webpage
Practice
# 👑 DYNASTY MERCANTILE

A regal furniture auction website built with HTML, CSS, JavaScript, and Firebase. This site allows users to browse throne-worthy listings, place real-time bids, and manage their royal profile.

---

## 🏗️ Project Structure


---

## 🚀 Setup Instructions

### 1. Preview Locally
- Open `pages/index.html` in your browser
- Ensure all links and images load correctly

### 2. Deploy Online
- Upload the full folder to [Netlify](https://netlify.com) or [GitHub Pages](https://pages.github.com)
- Set `index.html` as your homepage
- Connect your custom domain (e.g., dynastymercantile.com)

### 3. Firebase Integration
- Go to [Firebase Console](https://console.firebase.google.com)
- Create a new project: **DYNASTY MERCANTILE**
- Enable:
  - Authentication → Email/Password
  - Realtime Database → Start in test mode
- Copy your Firebase config and paste it into `auth.js` and `bidding.js`

### 4. Secure Your Database
In Firebase → Realtime Database → Rules:
```json
{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null"
  }
}

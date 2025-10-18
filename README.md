# mySahara Web Viewer

Beautiful, secure medical history viewer for QR code sharing.

## 🚀 Quick Deploy to Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/mysahara-web-viewer)

### Option 1: One-Click Deploy
1. Click the button above
2. Sign in to Vercel with GitHub
3. Deploy!

### Option 2: Manual Deploy
```bash
# Push to GitHub
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/mysahara-web-viewer.git
git push -u origin main

# Deploy on Vercel
# Go to vercel.com → Import Project → Select your repo
```

## ⚙️ Configuration

Before deploying, update your Supabase credentials in `index.html`:

```javascript
const SUPABASE_URL = 'https://your-project.supabase.co';
const SUPABASE_ANON_KEY = 'your-anon-key';
```

## 📝 Files

- `index.html` - Main viewer page
- `vercel.json` - Vercel configuration
- `.vercelignore` - Files to ignore during deployment

## 🔗 Usage

After deployment, your QR codes will link to:
```
https://your-site.vercel.app/view?code=SHARE_CODE
```

Update this URL in your Flutter app:
```dart
// lib/screens/share/qr_code_display_screen.dart
final shareUrl = 'https://your-site.vercel.app/view?code=${widget.share.shareCode}';
```

## 🎨 Features

- ✅ Beautiful, responsive UI
- ✅ Secure medical history display
- ✅ 10-minute expiry timer
- ✅ Mobile-friendly
- ✅ Fast loading (global CDN)

## 📖 Documentation

See `../VERCEL_DEPLOYMENT.md` for detailed deployment instructions.

## 🔒 Security

- HTTPS enforced
- Temporary links (10 min expiry)
- No data stored on viewer
- Secure headers configured

## 📄 License

Part of mySahara Health Application

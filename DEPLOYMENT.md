# GitHub Pages Deployment Instructions

## 🚀 Enable GitHub Pages

1. Go to your repository: https://github.com/sailendrakondapalli/NaveenBroTask_1
2. Click on **Settings** tab
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select **GitHub Actions**
5. The deployment will automatically trigger on the next push

## 📱 Your Live App URL

Once GitHub Pages is enabled, your app will be available at:
**https://sailendrakondapalli.github.io/NaveenBroTask_1**

## 🔄 Automatic Deployment

The GitHub Actions workflow is already set up to:
- Build your Expo app for web on every push to main
- Deploy the `dist` folder to GitHub Pages
- Your app will update automatically when you push changes

## 🛠️ Local Development & Deployment

```bash
# Build locally
npm run build:web

# Deploy (builds and reminds you to push)
npm run deploy

# Push to trigger GitHub Pages deployment
git add .
git commit -m "Update app"
git push
```

## ✅ Verification

After enabling GitHub Pages:
1. Check the **Actions** tab to see the deployment workflow
2. Visit your live URL to see the app
3. Any future pushes to main will automatically update the live site
# Render Deployment Guide

## 🚀 Deploy PowerStackHub to Render

Follow these steps to deploy your Expo web app to Render:

### 1. Create Render Account
- Go to [render.com](https://render.com)
- Sign up with your GitHub account

### 2. Create New Static Site
1. Click **"New +"** → **"Static Site"** (NOT Web Service)
2. Connect your GitHub repository: `sailendrakondapalli/NaveenBroTask_1`
3. Configure the deployment:

### 3. Deployment Settings
```
Name: powerstackhub (or your preferred name)
Branch: main
Root Directory: PowerStackHub
Build Command: npm ci && npx expo export --platform web
Publish Directory: dist
```

**Important**: Choose "Static Site" because:
- ✅ Your Expo app builds to static files
- ✅ Free tier available
- ✅ Fast CDN delivery
- ✅ Perfect for frontend-only apps

### 4. Environment Variables (Optional)
No environment variables needed for basic deployment.

### 5. Advanced Settings
- **Auto-Deploy**: Yes (deploys automatically on git push)
- **Pull Request Previews**: Enable for testing

## 🔧 Alternative: Manual Configuration

If you prefer manual setup instead of render.yaml:

### Build Command:
```bash
npm ci && npx expo export --platform web
```

### Publish Directory:
```
./dist
```

### Start Command:
```bash
# Not needed for static sites
```

## 🌐 Your Render URL
After deployment, your app will be available at:
`https://powerstackhub.onrender.com` (or your chosen name)

## 🔄 Automatic Deployments
- Every push to `main` branch triggers automatic deployment
- Build logs available in Render dashboard
- Deployment typically takes 2-3 minutes

## 🛠️ Local Testing
Before deploying, test your build locally:
```bash
npm run build:web
# Serve the dist folder to test
```

## 📊 Render vs GitHub Pages
| Feature | Render | GitHub Pages |
|---------|--------|--------------|
| Custom Domain | ✅ Free | ✅ Free |
| HTTPS | ✅ Auto | ✅ Auto |
| Build Time | ~2-3 min | ~1-2 min |
| Bandwidth | Generous | Generous |
| Deployment | Git push | Git push |

## 🔍 Troubleshooting
- Check build logs in Render dashboard
- Ensure `dist` folder is generated correctly
- Verify Node.js version compatibility (18.x recommended)
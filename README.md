# Edge Scanner - Payment Redirect Pages

This repository contains HTML redirect pages for the Edge Scanner mobile app's PayMongo payment integration.

## 🌐 **Live URL Structure**
Once deployed to Vercel, your URLs will be:
- `https://your-project-name.vercel.app/success` - Payment success redirect
- `https://your-project-name.vercel.app/failed` - Payment failure redirect

## 🚀 **Deploy to Vercel**

### **Option 1: Vercel CLI (Recommended)**
1. Install Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy:
   ```bash
   cd payment-redirects
   vercel
   ```

### **Option 2: GitHub + Vercel Dashboard**
1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository
5. Deploy!

### **Option 3: Drag & Drop**
1. Go to [vercel.com](https://vercel.com)
2. Drag the `payment-redirects` folder directly to the dashboard
3. Deploy instantly!

## 📱 **Update Your App**
After deployment, update your PaymentModal.js to use your live URLs:
```javascript
const redirectUrl = 'https://your-project-name.vercel.app/success';
const failedUrl = 'https://your-project-name.vercel.app/failed';
```

## 🔧 **Files Included**
- `index.html` - Landing page
- `success.html` - Payment success redirect
- `failed.html` - Payment failure redirect  
- `vercel.json` - Vercel routing configuration
- `README.md` - This documentation

## ⚡ **Features**
- ✅ Auto-redirect to mobile app after 2-3 seconds
- 🎨 Beautiful, responsive design
- 📱 Mobile-optimized
- 🔄 Fallback manual redirect button
- 🌐 HTTPS compliant for PayMongo 
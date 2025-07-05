# 🚗 FS RIDE - Professional Travel Billing System

A modern, responsive travel billing application with distance-based billing, invoice generation, client management, and expense tracking.

## ✨ Features

### Core Functionality
- **📋 Invoice Generation**: Professional invoices with PDF export
- **📏 Distance-Based Billing**: Automatic calculation (Distance × Rate/km × Trips)
- **👥 Client Management**: Complete customer database with GST details
- **💰 Expense Tracking**: Monitor travel-related costs with receipt uploads
- **📊 Dashboard Analytics**: Real-time statistics and insights
- **🌍 GPS Integration**: Distance calculation and route tracking

### Technical Features
- **🎨 Modern UI**: Responsive design with smooth animations
- **📱 Mobile-First**: Optimized for all device sizes
- **⚡ Fast Performance**: Optimized React components with lazy loading
- **🔒 Type Safety**: Full TypeScript implementation
- **💾 Local Storage**: Works offline with browser storage
- **📤 Export Functions**: PDF generation and data export

## 🚀 Quick Start (GitHub Pages)

### 1. Create Repository
```bash
# Create a new repository on GitHub
# Name: fs-ride-travel-billing (or your choice)
# Visibility: Public (required for free GitHub Pages)
```

### 2. Upload Code
- Download and extract the deployment package
- Upload all files to your GitHub repository
- Commit with message: "Deploy FS RIDE Travel Billing System"

### 3. Enable GitHub Pages
1. Go to **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **root**
4. Click **Save**

### 4. Access Your Site
- URL: `https://yourusername.github.io/repository-name`
- Deployment takes 5-10 minutes

## 💻 Local Development

### Prerequisites
- Node.js 18+ and npm
- Modern web browser

### Installation
```bash
# Clone your repository
git clone https://github.com/yourusername/fs-ride-travel-billing.git
cd fs-ride-travel-billing

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📁 Project Structure

```
fs-ride-travel-billing/
├── src/
│   ├── components/          # React components
│   │   ├── dashboard/       # Dashboard widgets
│   │   ├── layout/          # Header, sidebar, navigation
│   │   ├── modals/          # Invoice, client, expense modals
│   │   └── ui/              # Reusable UI components
│   ├── hooks/               # Custom React hooks
│   ├── lib/                 # Utilities and helpers
│   ├── pages/               # Page components
│   └── schema.ts            # Data types and validation
├── .github/workflows/       # GitHub Actions for deployment
├── public/                  # Static assets
└── dist/                    # Production build (generated)
```

## 🎯 Usage Guide

### Creating Invoices
1. Click **"New Invoice"** or use sidebar navigation
2. Select client from dropdown or create new
3. Choose billing type:
   - **Standard Items**: Quantity × Rate
   - **Distance-Based**: Distance × Rate/km × Trips
4. Add GST details (CGST, SGST, IGST)
5. Generate PDF and download

### Managing Clients
1. Navigate to **Clients** section
2. Add company details including GST information
3. Track all invoices and expenses per client
4. Edit or update client information anytime

### Expense Tracking
1. Go to **Expenses** section
2. Record travel costs with receipts
3. Categorize by client and trip
4. Track fuel, tolls, accommodation, etc.

### GPS Distance Calculation
1. Use **GPS Calculator** tool
2. Enter start and end locations
3. Get accurate distance measurements
4. Apply rates for automatic billing

## ⚙️ Configuration

### Customization Options
- **Company Details**: Update in header components
- **Theme Colors**: Modify in `src/index.css`
- **GST Rates**: Configure in invoice modal
- **Currency**: Set to ₹ (INR) by default

### Environment Variables (Optional)
```env
VITE_GOOGLE_MAPS_API_KEY=your_key_here
VITE_COMPANY_NAME="Your Company Name"
VITE_DEFAULT_GST_RATE=18
```

## 🌐 Deployment Options

### GitHub Pages (Free)
- Automatic deployment via GitHub Actions
- Custom domain support
- SSL/HTTPS included
- No server costs

### Alternative Platforms
- **Vercel**: Connect GitHub repo for auto-deployment
- **Netlify**: Drag-and-drop or Git integration
- **Surge.sh**: Simple static hosting
- **AWS S3**: Enterprise-grade hosting

## 📊 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Troubleshooting

### Common Issues

**Build Errors**
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
npm run build
```

**GitHub Pages Not Loading**
- Ensure repository is public
- Check GitHub Actions tab for build status
- Wait 10 minutes after first deployment
- Verify Pages settings in repository

**PDF Generation Issues**
- Ensure modern browser with JavaScript enabled
- Check browser console for errors
- Try downloading as image if PDF fails

## 📄 License

MIT License - feel free to use for personal or commercial projects.

## 🤝 Support

For technical issues:
1. Check browser console for errors
2. Verify all files uploaded correctly
3. Ensure GitHub Pages is properly configured
4. Check GitHub Actions for build failures

## 🎉 Credits

Built with modern web technologies:
- React 18 with TypeScript
- Tailwind CSS for styling
- Framer Motion for animations
- Radix UI for components
- jsPDF for document generation

---

**FS RIDE** - Professional Travel Billing Made Simple 🚗💼
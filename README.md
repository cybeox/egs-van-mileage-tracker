# 🚐 Van Mileage Tracker

A modern, mobile-first web application for tracking company van daily mileage with Google Sheets integration and comprehensive reporting features.

## ✨ Features

- **Daily Mileage Entry**: Record start/end mileage with automatic calculation
- **Flexible Start Points**: Home, Hotel, Office, Client Site, or custom locations
- **Multiple Fuel Entries**: Track multiple fuel purchases per day
- **Interactive Dashboard**: Weekly, monthly, and yearly analytics
- **Mobile Optimized**: Responsive design for on-the-go use
- **Export Options**: Excel, PDF, CSV, and Google Sheets sync
- **Visual Analytics**: Charts and statistics for mileage trends

## 🚀 Live Demo

Visit: [https://yourusername.github.io/van-mileage-tracker/](https://yourusername.github.io/van-mileage-tracker/)

## 📱 Screenshots

### Mobile Interface
- Clean, modern design optimized for mobile devices
- Three main tabs: Entry, Dashboard, History
- Touch-friendly controls and intuitive navigation

### Dashboard Analytics
- Real-time statistics (total miles, fuel costs, averages)
- Interactive charts showing mileage trends
- Period filtering (week/month/year)

## 🛠️ Setup Instructions

### Google Sheets Integration

1. **Create Google Cloud Project**
   - Go to [Google Cloud Console](https://console.cloud.google.com)
   - Create a new project or select existing one

2. **Enable Google Sheets API**
   - Navigate to "APIs & Services" → "Library"
   - Search and enable "Google Sheets API"

3. **Create API Credentials**
   - Go to "APIs & Services" → "Credentials"
   - Create API Key and restrict it:
     - Application restrictions: HTTP referrers
     - Add your domain: `yourdomain.github.io/*`
     - API restrictions: Google Sheets API only

4. **Prepare Your Google Sheet**
   - Create a new Google Sheet
   - Set sharing to "Anyone with the link can view"
   - Add headers: Date | Start Point | Start Mileage | End Mileage | Total Miles | Fuel Cost | Trip Summary
   - Copy the sheet ID from the URL

5. **Update Configuration**
   - Replace `GOOGLE_SHEETS_ID` and `GOOGLE_API_KEY` in the code
   - Deploy your changes

### Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/van-mileage-tracker.git
cd van-mileage-tracker

# Open index.html in your browser
# Or serve with a local server:
python -m http.server 8000
# Visit http://localhost:8000
```

### GitHub Pages Deployment

1. Fork or clone this repository
2. Update the Google Sheets configuration
3. Enable GitHub Pages in repository settings
4. Your app will be available at `https://yourusername.github.io/van-mileage-tracker/`

## 📊 Data Export Formats

- **Excel (.xlsx)**: Full data export with formatting
- **CSV**: Compatible with spreadsheet applications
- **PDF**: Formatted reports for printing/sharing
- **Google Sheets**: Real-time sync with cloud storage

## 🔧 Configuration

Update these variables in the JavaScript section:

```javascript
const GOOGLE_SHEETS_ID = 'your-sheet-id-here';
const GOOGLE_API_KEY = 'your-api-key-here';
```

## 🛡️ Security Notes

- API keys should be restricted to your domain only
- Google Sheets should have appropriate sharing permissions
- Consider using environment variables for sensitive data in production

## 📝 Usage

1. **Daily Entry**: Enter your daily mileage data including start point, mileage readings, and fuel costs
2. **Dashboard**: View analytics and trends for different time periods
3. **Export**: Download data in various formats or sync to Google Sheets
4. **History**: Review past entries and trip summaries

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🆘 Support

If you encounter any issues:
1. Check the browser console for error messages
2. Verify Google Sheets API configuration
3. Ensure proper sharing permissions on your Google Sheet
4. Create an issue in this repository

## 🔄 Updates

- **v1.0**: Initial release with full mileage tracking functionality
- Mobile-optimized interface with dashboard analytics
- Multiple export formats and Google Sheets integration

---

Made with ❤️ for efficient van mileage tracking

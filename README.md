# Care Compare Measure Timeline Dashboard

A comprehensive dashboard for tracking performance timelines across Care Compare, Star Ratings, and Leapfrog programs.

## Features

- **Live Data Integration**: Connects directly to Google Sheets for real-time updates
- **Timeline Visualization**: Gantt chart showing performance periods
- **Multi-Program Support**: 
  - Care Compare measures
  - CMS Star Ratings
  - Leapfrog Safety Grades
- **Manual Data Import**: Backup option for direct data paste
- **Responsive Design**: Works on desktop and mobile devices

## Live Demo

Visit: [https://YOUR-USERNAME.github.io/care-compare-dashboard/](https://YOUR-USERNAME.github.io/care-compare-dashboard/)

## Data Source

The dashboard pulls data from a Google Sheets spreadsheet containing:
- July 2025 Data Release measures
- Care Compare Website Only measures
- Star Ratings Measures
- Leapfrog Safety Grades

## Setup Instructions

### For Users
Simply visit the live demo link above. The dashboard will automatically load the latest data.

### For Developers

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR-USERNAME/care-compare-dashboard.git
   cd care-compare-dashboard
   ```

2. **Update the Google Sheets ID** (if using your own data)
   - Open `index.html`
   - Find `const SHEET_ID = '...'`
   - Replace with your Google Sheets ID

3. **Deploy Google Apps Script** (for API access)
   - Open [Google Apps Script](https://script.google.com)
   - Create a new project
   - Copy the script from `google-apps-script.js`
   - Deploy as Web App with "Anyone" access
   - Update the `GOOGLE_APPS_SCRIPT_URL` in `index.html`

4. **Deploy to GitHub Pages**
   - Push your changes to GitHub
   - Go to Settings → Pages
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)"
   - Save and wait for deployment

## Manual Data Import

If automatic connection fails:
1. Open your Google Sheet
2. Select all data (Ctrl+A)
3. Copy (Ctrl+C)
4. Click "Manual Data Import" in the dashboard
5. Paste and click "Import Data"

## Technologies Used

- HTML5/CSS3
- Vanilla JavaScript
- Google Apps Script
- Google Sheets API
- GitHub Pages

## Troubleshooting

### Data not loading?
1. Check browser console for errors (F12)
2. Verify Google Apps Script is deployed correctly
3. Ensure Google Sheet is shared publicly or with the script
4. Use Manual Data Import as fallback

### CORS errors?
- The dashboard must be served over HTTP/HTTPS (not file://)
- GitHub Pages automatically handles this correctly

## Contributing

Pull requests are welcome! For major changes, please open an issue first.

## License

MIT License - feel free to use this dashboard for your organization.

## Contact

For questions or support, please open an issue on GitHub.

---

Built with ❤️ for healthcare quality improvement
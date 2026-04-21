# The Wellness Project

A professional wellness poster and feedback collection system for our Team Wellbeing Initiative.

## 🌟 Overview

This project provides:
- Clean, professional wellness poster design
- Integrated feedback form (Monday.com)
- Mobile-responsive layout
- IBM Design Language compliant

## 🔗 Live Site

Once deployed, your site will be available at:
```
https://YOUR-USERNAME.github.io/wellness-project/
```

## ✨ Features

- ✅ Professional wellness poster with calming design
- ✅ Integrated Monday.com feedback form
- ✅ Anonymous feedback option
- ✅ Mobile-responsive
- ✅ IBM Plex Sans typography
- ✅ Accessible design
- ✅ Animated visual elements
- ✅ Privacy notice included

## 🛠️ Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with animations
- **Google Fonts** - IBM Plex Sans typography
- **Monday.com** - Form integration for feedback collection
- **GitHub Pages** - Free hosting

## 📦 Setup Instructions

### 1. Monday.com Setup (15 minutes)

1. Log into Monday.com
2. Create a new board: "Wellness Initiative Feedback"
3. Add columns: Name, Email, Feedback, Date, Status, Category, Priority
4. Create a Form view
5. Configure form fields (Name, Email, Feedback)
6. Get the form URL (looks like: `https://forms.monday.com/forms/abc123def456`)

### 2. Update index.html (2 minutes)

1. Open `index.html` in a text editor
2. Find line ~330 (search for `YOUR_MONDAY_FORM_URL_HERE`)
3. Replace with your Monday.com form URL
4. Save the file

### 3. Deploy to GitHub Pages (10 minutes)

1. Create a new GitHub repository named `wellness-project`
2. Upload all files from this folder
3. Go to Settings → Pages
4. Set Source to: Deploy from branch `main` / `/ (root)`
5. Wait 1-2 minutes for deployment
6. Visit your site at: `https://YOUR-USERNAME.github.io/wellness-project/`

## 📁 File Structure

```
wellness-project/
├── index.html          # Main HTML file with poster and form
├── README.md           # This file
├── .gitignore          # Git exclusions
└── SETUP_GUIDE.md      # Detailed setup instructions
```

## 🚀 Quick Start

**For immediate testing:**
1. Open `index.html` in your web browser
2. View the wellness poster
3. Note: Form won't work until Monday.com URL is added

**For production deployment:**
1. Follow Monday.com setup above
2. Update `index.html` with form URL
3. Deploy to GitHub Pages
4. Share the link with your team!

## 🔧 Customization

### Change Colors

Edit the CSS in `index.html`:

```css
/* Poster gradient (line ~95) */
background: linear-gradient(135deg, #e8f5e9 0%, #b3e5fc 50%, #f3e5f5 100%);

/* Primary button color (line ~177) */
background: #0f62fe;
```

### Change Text

Edit these sections in `index.html`:
- **Line 280:** Page title
- **Line 287:** Poster title
- **Line 288:** Tagline
- **Line 289:** Message
- **Line 312:** Feedback section heading

### Add Logo

1. Add your logo image to the folder
2. Insert in the header section:
```html
<img src="your-logo.png" alt="Logo" style="max-width: 200px;">
```

## 📊 Viewing Feedback

All feedback submissions will appear in your Monday.com board:

1. Log into Monday.com
2. Navigate to "Wellness Initiative Feedback" board
3. View submissions in real-time
4. Use Status column to track progress
5. Assign feedback to team members
6. Export to Excel for analysis

## 🔒 Privacy & Security

- Anonymous submissions supported (leave name/email blank)
- Data stored securely in Monday.com
- GDPR compliant
- SOC 2 Type II certified
- IBM-approved tool

## 📱 Mobile Support

The site is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones
- All modern browsers

## 🐛 Troubleshooting

### Form not showing?
- Check Monday.com form URL is correct
- Ensure form is set to "Public" in Monday.com
- Try the button link option instead of iframe
- Clear browser cache

### Site not updating?
- Wait 2-3 minutes after GitHub commit
- Hard refresh browser (Ctrl+F5 or Cmd+Shift+R)
- Check GitHub Actions tab for build status

### Submissions not appearing?
- Verify form URL is correct
- Test form directly (visit Monday.com form URL)
- Check Monday.com board permissions

## 📈 Success Metrics

Track these metrics after launch:
- **Page views** (GitHub Insights)
- **Form submissions** (Monday.com)
- **Response rate** (submissions / team size)
- **Feedback themes** (categorize in Monday.com)
- **Implementation time** (track in Status column)

## 🤝 Contributing

This is an internal ISDL project. For updates or improvements:
1. Create a branch
2. Make your changes
3. Test thoroughly
4. Submit for review

## 📞 Support

For questions or issues:
- Check `SETUP_GUIDE.md` for detailed instructions
- Review troubleshooting section above
- Contact: ISDL Design and Content Team

## 📄 License

Internal use only - ISDL Team Wellbeing Initiative

---

**Created by:** ISDL Design and Content Team  
**Last Updated:** April 2026  
**Version:** 1.0
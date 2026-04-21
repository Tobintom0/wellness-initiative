# Setup Guide - The Wellness Project

Complete step-by-step instructions for deploying your wellness poster with Monday.com integration.

## 📋 Prerequisites

- GitHub account (free) - https://github.com
- Monday.com account (free tier available) - https://monday.com
- Text editor (VS Code, Notepad++, or any editor)
- Web browser (Chrome, Firefox, Safari, or Edge)

**Time Required:** ~30 minutes total

---

## Step 1: Set Up Monday.com Form (15 minutes)

### 1.1 Create Board

1. Log into Monday.com
2. Click **"+ Add"** → **"New board"**
3. Name: **"Wellness Initiative Feedback"**
4. Choose: **"Blank board"**
5. Click **"Create board"**

### 1.2 Add Columns

Click **"+ Add Column"** and create these columns:

| Column Name | Type | Configuration |
|-------------|------|---------------|
| Name | Text | Default |
| Email | Email | Default |
| Feedback | Long Text | Enable rich text |
| Submission Date | Date | Auto-fill creation date |
| Status | Status | Labels: New, Reviewed, In Progress, Implemented |
| Category | Dropdown | Options: Design, Programs, Activities, Mental Health, Physical Wellness, Other |
| Priority | Priority | Default (Low, Medium, High, Critical) |
| Assigned To | People | Default |

### 1.3 Create Form View

1. Click **"+ Add View"** (top of board)
2. Select **"Form"**
3. Name: **"Wellness Feedback Form"**
4. Click **"Create"**

### 1.4 Configure Form

**Form Settings:**
1. Click **gear icon** (Form settings)
2. **Form name:** "Share Your Ideas & Opinions"
3. **Description:** "Help us shape the Team Wellbeing Initiative"
4. **Thank you message:** "Thank you for your feedback! Your ideas will help us create a healthier, happier workplace."

**Configure Fields:**

For each field, click to edit:

**Name:**
- Label: "Your Name (Optional)"
- Description: "Leave blank for anonymous feedback"
- Required: ❌ No
- Show: ✅ Yes

**Email:**
- Label: "Your Email (Optional)"
- Description: "Only if you'd like us to follow up"
- Required: ❌ No
- Show: ✅ Yes

**Feedback:**
- Label: "Your Ideas & Opinions"
- Description: "Share your thoughts, ideas, and suggestions"
- Required: ✅ Yes
- Show: ✅ Yes

**Hide these fields** (for internal use only):
- Submission Date
- Status
- Category
- Priority
- Assigned To

### 1.5 Customize Appearance

1. Click **"Customize"** tab
2. **Theme color:** Blue (#0f62fe)
3. **Button text:** "Submit Feedback"
4. **Cover image:** Optional (upload wellness poster image)

### 1.6 Get Form URL

1. Click **"Share"** button (top right)
2. Click **"Copy link"**
3. **Save this URL** - it looks like:
   ```
   https://forms.monday.com/forms/abc123def456ghi789
   ```

✅ **Monday.com setup complete!**

---

## Step 2: Update index.html (5 minutes)

### 2.1 Open index.html

1. Navigate to the `wellness-project` folder
2. Open `index.html` in your text editor

### 2.2 Find the Form Section

1. Press `Ctrl+F` (or `Cmd+F` on Mac)
2. Search for: `YOUR_MONDAY_FORM_URL_HERE`
3. You'll find it around line 330

### 2.3 Replace with Your URL

**Before:**
```html
<iframe 
    class="monday-form-embed"
    src="YOUR_MONDAY_FORM_URL_HERE"
    width="100%"
    height="800"
    frameborder="0">
</iframe>
```

**After:**
```html
<iframe 
    class="monday-form-embed"
    src="https://forms.monday.com/forms/abc123def456ghi789"
    width="100%"
    height="800"
    frameborder="0">
</iframe>
```

### 2.4 Save the File

- Press `Ctrl+S` (or `Cmd+S` on Mac)
- Close the editor

✅ **index.html updated!**

---

## Step 3: Upload to GitHub (10 minutes)

### 3.1 Create GitHub Repository

1. Go to https://github.com
2. Sign in (or create account if needed)
3. Click **"+"** icon (top right) → **"New repository"**

**Repository Settings:**
- **Name:** `wellness-project`
- **Description:** "Team Wellbeing Initiative - Wellness Poster and Feedback"
- **Visibility:** 
  - ✅ **Public** (anyone can view)
  - OR **Private** (only you and invited collaborators)
- **Initialize:**
  - ❌ Don't add README (we have our own)
  - ❌ Don't add .gitignore (we have our own)
  - ❌ Don't add license

4. Click **"Create repository"**

### 3.2 Upload Files

**Method 1: Web Interface (Easiest)**

1. On the repository page, click **"uploading an existing file"** link
2. Drag and drop ALL files from `wellness-project` folder:
   - `index.html`
   - `README.md`
   - `.gitignore`
   - `SETUP_GUIDE.md`
3. Add commit message: "Initial commit - wellness poster with Monday.com"
4. Click **"Commit changes"**

**Method 2: Git Command Line** (if you prefer)

```bash
# Navigate to wellness-project folder
cd path/to/wellness-project

# Initialize Git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - wellness poster with Monday.com"

# Add remote (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/wellness-project.git

# Push to GitHub
git branch -M main
git push -u origin main
```

✅ **Files uploaded to GitHub!**

---

## Step 4: Enable GitHub Pages (5 minutes)

### 4.1 Go to Settings

1. In your repository, click **"Settings"** tab
2. Scroll down left sidebar
3. Click **"Pages"**

### 4.2 Configure Pages

**Source:**
- **Deploy from a branch**

**Branch:**
- Select: **`main`**
- Folder: **`/ (root)`**

Click **"Save"**

### 4.3 Wait for Deployment

- GitHub will build your site (1-2 minutes)
- Refresh the page
- You'll see: **"Your site is live at https://YOUR-USERNAME.github.io/wellness-project/"**

### 4.4 Visit Your Site

Click the URL or visit:
```
https://YOUR-USERNAME.github.io/wellness-project/
```

✅ **Site is live!**

---

## Step 5: Test Everything (5 minutes)

### 5.1 Test on Desktop

1. Visit your GitHub Pages URL
2. Check wellness poster displays correctly
3. Scroll to feedback section
4. Verify Monday.com form is embedded
5. Fill out test feedback
6. Submit

### 5.2 Check Monday.com

1. Go to Monday.com
2. Open "Wellness Initiative Feedback" board
3. Verify your test submission appears
4. Check all fields populated correctly

### 5.3 Test on Mobile

1. Open site on your phone
2. Check responsive design
3. Test form submission
4. Verify submission in Monday.com

### 5.4 Test Anonymous Submission

1. Fill out form
2. Leave Name and Email blank
3. Submit
4. Check Monday.com - should show "Anonymous"

✅ **All tests passed!**

---

## Step 6: Share with Team (5 minutes)

### 6.1 Prepare Announcement

**Email Subject:** 🌱 Share Your Ideas for The Wellness Project

**Email Body:**
```
Hi Team,

We're excited to launch The Wellness Project - our new Team Wellbeing Initiative!

We'd love to hear your ideas and opinions. Please take 2-3 minutes to:

1. View the wellness poster
2. Share your thoughts and suggestions

👉 https://YOUR-USERNAME.github.io/wellness-project/

Your feedback can be anonymous - just leave the name/email fields blank.

All ideas welcome! We're looking for:
✨ Suggestions for wellbeing programs
✨ Ideas for team activities
✨ Feedback on the poster design
✨ Any other thoughts

Thank you for helping us create a healthier, happier workplace!

Best regards,
ISDL Design and Content Team
```

### 6.2 Share via Multiple Channels

- ✅ Send email to team
- ✅ Post in Slack/Teams
- ✅ Add to team calendar
- ✅ Include in newsletter
- ✅ Pin in team chat

✅ **Launch complete!**

---

## Troubleshooting

### Problem: Form not showing

**Solutions:**
1. Check Monday.com form URL is correct in `index.html`
2. Ensure form is set to "Public" in Monday.com
3. Try opening form URL directly in browser
4. Check browser console for errors (F12)
5. Try the button link option instead of iframe

### Problem: GitHub Pages not updating

**Solutions:**
1. Wait 2-3 minutes after commit
2. Hard refresh: `Ctrl+F5` (Windows) or `Cmd+Shift+R` (Mac)
3. Check GitHub Actions tab for build status
4. Clear browser cache
5. Try incognito/private browsing mode

### Problem: Submissions not in Monday.com

**Solutions:**
1. Verify form URL matches in both places
2. Check Monday.com board permissions
3. Test form directly (visit Monday.com form URL)
4. Check if form is still active
5. Look in Monday.com trash/archive

### Problem: Mobile display issues

**Solutions:**
1. The CSS is responsive - try different devices
2. Check viewport meta tag is present
3. Test in browser dev tools (F12 → Device toolbar)
4. Try different mobile browsers
5. Check for JavaScript errors

---

## Maintenance

### Update Content

1. Go to GitHub repository
2. Click `index.html`
3. Click pencil icon (Edit)
4. Make changes
5. Commit changes
6. Wait 1-2 minutes for redeployment

### Update Monday.com Form

1. Edit form in Monday.com
2. Changes apply immediately
3. No GitHub update needed

### View Analytics

**GitHub:**
- Repository → Insights → Traffic
- See page views and visitors

**Monday.com:**
- Board → Dashboard view
- Create charts for submissions
- Filter by date, category, status

---

## Next Steps

After successful deployment:

1. ✅ Monitor submissions daily
2. ✅ Respond to feedback within 48 hours
3. ✅ Categorize feedback in Monday.com
4. ✅ Update Status as you review
5. ✅ Assign action items to team
6. ✅ Share summary with team weekly
7. ✅ Implement top ideas
8. ✅ Close the feedback loop

---

## Support

Need help?
- Review this guide
- Check troubleshooting section
- Contact: ISDL Design and Content Team

---

**Setup Complete! 🎉**

Your wellness poster is now live and collecting feedback!
# Quick Form Creation Guide

## ✅ What's Already Done

Your Monday.com board columns are ready:
- ✅ Email column created
- ✅ Feedback column created  
- ✅ Category column created
- ✅ Priority column created

**Board URL:** https://ibm.monday.com/boards/18409572978

---

## 🚀 Create the Form (2 Minutes)

### Step 1: Open Your Board
Click this link: https://ibm.monday.com/boards/18409572978

### Step 2: Add Form View
1. Look for **"+ Add View"** button (top of board, near Main Table)
2. Click it
3. Select **"Form"** from the dropdown
4. Name it: **"Wellness Feedback Form"**
5. Click **"Add"**

### Step 3: Configure Form Fields
The form builder will open. Add these fields by clicking the **"+ Add question"** button:

**Question 1:**
- Select column: **Name**
- Question text: "Your Name (Optional)"
- Toggle OFF "Required"

**Question 2:**
- Select column: **Email**
- Question text: "Email Address (Optional)"
- Toggle OFF "Required"

**Question 3:**
- Select column: **Feedback** (Long Text)
- Question text: "Share Your Thoughts"
- Toggle ON "Required" ✅

**Question 4:**
- Select column: **Category**
- Question text: "Feedback Type (Optional)"
- Toggle OFF "Required"

### Step 4: Customize Welcome Screen
1. Click **"Welcome screen"** tab
2. Title: **"The Wellness Project"**
3. Description: 
   ```
   We're building a wellness initiative and want YOUR input!
   Share ideas and feedback to help shape programs that support your wellbeing.
   
   Responses are anonymous unless you provide your name/email.
   ```

### Step 5: Customize Thank You Screen
1. Click **"Thank you screen"** tab
2. Message:
   ```
   Thank you for your feedback! 🌟
   
   Your input helps us create wellness programs that truly matter.
   
   - ISDL Design and Content Team
   ```

### Step 6: Get Form URL
1. Click **"Share"** button (top right)
2. Copy the **"Public link"**
3. It looks like: `https://forms.monday.com/forms/abc123xyz456`
4. **SAVE THIS URL!**

---

## 🔧 Update index.html

Open `index.html` and find this section (around line 330):

```html
<iframe 
    class="monday-form-embed"
    src="YOUR_MONDAY_FORM_URL_HERE"
    width="100%"
    height="800"
    frameborder="0">
</iframe>
```

Replace `YOUR_MONDAY_FORM_URL_HERE` with your form URL:

```html
<iframe 
    class="monday-form-embed"
    src="https://forms.monday.com/forms/YOUR-ACTUAL-FORM-ID"
    width="100%"
    height="800"
    frameborder="0">
</iframe>
```

Save the file!

---

## ✅ Done!

Now you can:
1. Upload all files to GitHub
2. Enable GitHub Pages
3. Share the live URL with your team

**Total time:** 2 minutes to create form + 10 minutes to deploy = 12 minutes! 🎉
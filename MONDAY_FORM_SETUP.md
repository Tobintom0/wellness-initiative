# Monday.com Form Setup Guide

## ✅ Board Structure Created

Your Monday.com board is now configured with the following columns:

### Current Board Structure

**Board URL:** https://ibm.monday.com/boards/18409572978  
**Board Name:** Wellness Initiative Feedback

#### Columns Created:

1. **Name** (Text) - Default column - For respondent's name (optional)
2. **Person** (People) - Default column - For assigning feedback to team members
3. **Status** (Status) - Default column - Labels: Working on it, Done, Stuck, On Hold
4. **Date** (Date) - Default column - For submission date tracking
5. **Email** (Email) - ✅ Just created (ID: `email_mm2mdxsx`) - For optional email follow-up
6. **Feedback** (Long Text) - ✅ Just created (ID: `long_text_mm2m3fgd`) - Main feedback field (required)
7. **Category** (Dropdown) - ✅ Just created (ID: `dropdown_mm2mv05j`) - Options: Design Feedback, Program Ideas, Activity Suggestions, General Comments, Question
8. **Priority** (Status) - ✅ Just created (ID: `color_mm2m2met`) - Levels: Low, Medium, High, Critical

---

## 📋 Create the Form (5 Steps)

### Step 1: Access Form Builder
1. Go to: https://ibm.monday.com/boards/18409572978
2. Click **"+ Add View"** button
3. Select **"Form"**
4. Name it: "Wellness Feedback Form"

### Step 2: Add Form Fields

**Field 1: Name (Optional)**
- Column: Name
- Label: "Your Name (Optional)"
- Help text: "You can submit anonymously"
- Required: ❌ No

**Field 2: Email (Optional)**
- Column: Email
- Label: "Email Address (Optional)"
- Help text: "Only if you'd like follow-up"
- Required: ❌ No

**Field 3: Feedback (Required)**
- Column: Feedback
- Label: "Share Your Thoughts"
- Help text: "What would you like to see in our wellness initiative?"
- Required: ✅ Yes

**Field 4: Category (Optional)**
- Column: Category
- Label: "Feedback Type (Optional)"
- Required: ❌ No

### Step 3: Customize Appearance

**Form Title:** "The Wellness Project - Share Your Ideas"

**Description:**
```
We're building a wellness initiative for our team and we want YOUR input! 
Share your ideas, suggestions, and feedback to help shape programs that 
truly support your wellbeing.

Your responses are anonymous unless you choose to provide your name/email.
```

**Thank You Message:**
```
Thank you for your feedback! 🌟

Your input helps us create wellness programs that truly matter.
We'll review all submissions and share updates soon.

- ISDL Design and Content Team
```

### Step 4: Configure Settings
1. Click **"Form Settings"** (gear icon)
2. Enable:
   - ✅ Allow multiple submissions
   - ✅ Show progress bar
   - ❌ Require login (for anonymous submissions)

### Step 5: Get Form URL
1. Click **"Share"** button
2. Copy **Public Form Link**
3. URL format: `https://forms.monday.com/forms/[unique-id]`
4. **Save this URL!**

---

## 🔧 Update index.html

Find line ~330 and replace:

**Before:**
```html
src="YOUR_MONDAY_FORM_URL_HERE"
```

**After:**
```html
src="https://forms.monday.com/forms/YOUR-ACTUAL-FORM-ID"
```

---

## 🧪 Test Before Deploying

1. Open form URL in browser
2. Submit test entry (anonymous)
3. Check board for submission
4. Delete test entry
5. Verify form displays in index.html

---

## 📊 Managing Feedback

### Workflow
1. **New:** Status = "Working on it", Assign reviewer, Set priority
2. **Review:** Analyze, add notes, tag related items
3. **Done:** Mark complete, note implementation
4. **On Hold:** Add reason, revisit later

### Useful Views
- **By Category:** Group by Category column
- **By Priority:** Group by Priority column
- **Timeline:** Group by Date column

---

## 🔒 Privacy

- Name/Email optional = anonymous submissions
- No login required
- Only board members see submissions
- Follow IBM data privacy guidelines

---

## 🆘 Troubleshooting

**Form not displaying?**
- Verify URL is correct
- Check form is "Public"
- Clear browser cache

**Submissions not appearing?**
- Refresh board view
- Verify correct board
- Check form settings

**Form size issues?**
- Adjust iframe height (600-1000px)
- Test on mobile

---

## ✨ Launch Checklist

- [ ] Board columns created ✅
- [ ] Form created in Monday.com
- [ ] Form fields configured
- [ ] Form appearance customized
- [ ] Form URL copied
- [ ] index.html updated
- [ ] Test submission successful
- [ ] Test submission deleted
- [ ] Ready to deploy!

**Next:** Upload to GitHub following SETUP_GUIDE.md
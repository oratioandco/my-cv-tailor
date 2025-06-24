# My CV Tailor System

## 🚀 Quick Start

### New User? Start Here:
```bash
@setup.mdc
```
**This guided setup walks you through everything conversationally - no need to read documentation first!**

### Already Set Up? Quick Workflow:
For each job application: `@analyze-job-posting.mdc` → `@verify-experience.mdc` → `@generate-cv.mdc`

---

### Manual Setup (Alternative):
If you prefer to set up manually:
1. **PDF CV**: Drop `cv.pdf` in `input/` folder
2. **LinkedIn Export**: Save LinkedIn profile as `linkedin.pdf` in `input/` folder  
3. **LinkedIn Data**: Download LinkedIn data and extract to `input/linkedin-data/`
4. **Manual Text**: Paste CV content into `start-here.md`
5. **Document Attachment**: Attach CV file directly to conversation

Then run `@import-initial-cv.mdc` (one-time setup)

## 📋 Complete Workflow

### First Time Setup
```bash
# Recommended: Guided conversational setup
@setup.mdc

# Alternative: Manual import (if you prefer to set up yourself)
@import-initial-cv.mdc
```

### For Each Job Application
```bash
# 1. Analyze the job posting
@analyze-job-posting.mdc

# 2. Verify experience gaps (if needed)
@verify-experience.mdc

# 3. Generate customized CV
@generate-cv.mdc

# 4. Generate cover letter (optional)
@generate-cover-letter.mdc
```

## 🎯 Key Features

### ✅ **Safety-First**
- Never embellishes experience
- All claims are verified
- Protects your professional reputation
- Interview-ready content

### 🔧 **Smart Customization**
- Analyzes job requirements
- Selects relevant experiences
- Optimizes for ATS systems
- Matches company culture

### 📊 **Learning System**
- Improves with each application
- Builds verified experience database
- Tracks successful patterns
- Reduces future setup time

### 🎨 **Professional Output**
- Interactive HTML with editing
- Print-ready PDFs
- ATS-compatible DOCX files
- Multiple style options

## 📁 File Structure

```
my-cv-tailor/
├── input/                     # Multiple CV input options
│   ├── cv.pdf                # Drop your PDF CV here
│   ├── linkedin.pdf          # LinkedIn profile PDF export
│   ├── linkedin-data/        # LinkedIn data download (CSV files)
│   └── README.md             # Input format instructions
├── start-here.md              # Manual text input option
├── rules/                     # AI processing rules (.mdc files)
│   ├── import-initial-cv.mdc  # Multi-format import with auto-detection
│   ├── analyze-job-posting.mdc
│   ├── verify-experience.mdc
│   ├── generate-cv.mdc
│   └── generate-cover-letter.mdc
├── data/                      # Your structured information
│   ├── personal-info.md
│   ├── initial-cv-raw.md      # Original CV preserved
│   ├── experiences/           # One file per job
│   ├── skills/               # Categorized skills
│   ├── education/            # Education history
│   ├── awards/               # Recognition
│   └── verification-log/     # What's been verified
├── templates/                 # HTML/CSS templates
│   └── cv-template.html
└── outputs/                   # Generated CVs and cover letters
    ├── cv/
    └── cover-letters/
```

## 🛠️ Commands Reference

| Command | Purpose | When to Use |
|---------|---------|-------------|
| `@setup.mdc` | **Guided conversational setup** | **First time users - start here!** |
| `@import-initial-cv.mdc` | Import CV (auto-detects format) | Manual setup - supports PDF, LinkedIn, text |
| `@analyze-job-posting.mdc` | Analyze job requirements | For each new job |
| `@verify-experience.mdc` | Verify experience claims | When gaps identified |
| `@generate-cv.mdc` | Create customized CV | After verification complete |
| `@generate-cover-letter.mdc` | Create cover letter | Optional, after CV |

## 🔍 How Job Analysis Works

1. **Paste job posting** or provide URL
2. **Requirements extraction**: Must-have vs nice-to-have
3. **Fit calculation**: Honest percentage match
4. **Gap identification**: What needs verification
5. **Keyword extraction**: For ATS optimization

Example output:
```
📊 Job Analysis: GitLab - Senior Product Designer
Fit Score: 85% ⭐⭐⭐⭐

✅ Strong Matches (6):
- Enterprise B2B software design
- Technical interface design
- Admin tool development

❓ Need Verification (3):
- GitLab platform experience
- CI/CD workflow knowledge
- Remote team leadership

❌ Gaps Identified (2):
- DevOps tool design
- Open source contribution
```

## 📥 Input Format Support

The system supports multiple CV input formats with automatic detection:

### 📄 PDF CV Import
- **File**: Drop `cv.pdf` in `input/` folder
- **Best for**: Traditional CVs from Word, Google Docs, etc.
- **Processing**: Extracts text and parses as standard CV format

### 💼 LinkedIn Profile Import

#### Option A: LinkedIn PDF Export
- **File**: Save LinkedIn profile as `linkedin.pdf` in `input/` folder
- **How to get**: LinkedIn profile → "More" → "Save to PDF"
- **Processing**: Handles LinkedIn's unique structure and formatting

#### Option B: LinkedIn Data Download (Recommended)
- **Files**: Extract LinkedIn data to `input/linkedin-data/` folder
- **How to get**: LinkedIn Settings → "Get a copy of your data"
- **Processing**: Most accurate - uses structured CSV data
- **Includes**: Complete profile, hidden details, precise dates

### ✏️ Manual Text Input
- **File**: Paste content in `start-here.md`
- **Best for**: Quick setup or non-standard formats
- **Processing**: Traditional text parsing

### 📎 Document Attachments
- **Method**: Attach CV file directly in Cursor/Claude Code
- **Supported**: PDF, DOCX, TXT files
- **Processing**: Automatic format detection and parsing

### 🔍 Auto-Detection Process
1. System checks `input/` folder for files
2. Detects format (PDF CV vs LinkedIn vs CSV data)
3. Applies format-specific parsing logic
4. Falls back to `start-here.md` if no files found
5. Creates same structured output regardless of input format

### 📊 LinkedIn-Specific Features
- **Narrative Conversion**: Transforms LinkedIn's paragraph style to CV bullet points
- **Skills Processing**: Extracts skill names, removes endorsement counts
- **Date Standardization**: Converts LinkedIn date formats to CV standards
- **Section Mapping**: Maps "About" to Summary, "Accomplishments" to multiple sections
- **Content Cleanup**: Removes social elements, maintains professional tone

## 🔒 Safety Principles

### Never
- ❌ Adds unverified information
- ❌ Embellishes responsibilities  
- ❌ Extends employment dates
- ❌ Creates fictional achievements

### Always  
- ✅ Uses only verified information
- ✅ Maintains honest representation
- ✅ Provides accurate dates
- ✅ Ensures interview defensibility

## 🎨 Output Options

### Interactive HTML CV
- **Live editing**: Click any text to modify
- **Style options**: Modern, Tech, Corporate themes
- **Auto-save**: Changes preserved automatically
- **Export ready**: PDF/DOCX generation

### Professional PDF
- **ATS optimized**: Clean, parseable format
- **Print ready**: Professional appearance
- **Consistent**: Matches your template style

### DOCX Format
- **Maximum compatibility**: Works with all ATS systems
- **Editable**: Minor tweaks possible
- **Standard**: Industry-expected format

## 💡 Pro Tips

1. **First import is crucial** - Include everything, even minor experience
2. **Be honest in verification** - System protects you from over-promising  
3. **Use HTML editor** - Make final tweaks with live preview
4. **Save multiple versions** - Different roles need different positioning
5. **Export early** - Always have submission-ready files

## 🚨 Common Mistakes to Avoid

- Don't rush the verification process
- Don't skip job analysis for "similar" roles
- Don't edit the raw data files manually
- Don't use unverified claims in interviews
- Don't forget to export final PDFs

## 📈 System Learning

Each application improves the system:
- **Verified experiences** become reusable assets
- **Successful keywords** get tracked and recommended
- **Industry patterns** improve future analysis
- **Time efficiency** increases with each use

## 🔧 Troubleshooting

### "No matches found"
- Check if CV was properly imported
- Ensure job analysis completed
- Verify data files exist in `/data/`

### "Verification needed"  
- Run `@verify-experience.mdc`
- Answer questions honestly and specifically
- Don't skip verification steps

### "Export failed"
- Check HTML template exists
- Ensure all placeholders filled
- Try different browser for PDF export

## 🎯 Next Steps

### New Users:
1. **Run guided setup**: `@setup.mdc` (takes 10-15 minutes)
2. **Find target job**: Copy job posting text or URL  
3. **Generate first CV**: Follow the workflow above
4. **Refine over time**: System improves with each use

### Alternative (Manual Setup):
1. **Choose input method**: PDF upload, LinkedIn export, or manual text
2. **Prepare your data**: See `input/README.md` for detailed instructions  
3. **Run import**: `@import-initial-cv.mdc` (auto-detects your format)

### Quick Start by Format:
- **New Users**: Just run `@setup.mdc` - it handles everything conversationally
- **PDF Users**: Drop `cv.pdf` in `input/` folder → run `@import-initial-cv.mdc`
- **LinkedIn Users**: Save profile as PDF or download data → run `@import-initial-cv.mdc`
- **Text Users**: Paste CV in `start-here.md` → run `@import-initial-cv.mdc`

---

## ✅ Production Ready

The My CV Tailor system is **complete and ready to use**! All components are implemented and tested:

- ✅ **Conversational Setup** - Guided onboarding via `@setup.mdc`
- ✅ **Multi-Format Import** - PDF, LinkedIn, text input support
- ✅ **Smart Job Analysis** - Automatic fit scoring and gap identification  
- ✅ **Experience Verification** - Safety-first validation system
- ✅ **HTML Generation** - Real CVs and cover letters with inline editing
- ✅ **PDF Export** - Browser-based, ATS-compatible output
- ✅ **Complete Documentation** - Ready for immediate use

## 🚀 Get Started Now

1. **Run**: `@setup.mdc` - 15-minute guided setup
2. **Find a job** - Copy any job posting
3. **Generate CV** - Follow the conversational workflow
4. **Export PDF** - Professional, ready-to-submit documents

See `EXAMPLE-WORKFLOW.md` for a complete walkthrough.

---

**Ready to revolutionize your job applications?** This system transforms CV customization from a 2-hour manual chore into a 10-minute guided conversation that produces better, more accurate results every time.
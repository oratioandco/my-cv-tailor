# Example Complete Workflow

## Test the My CV Tailor System

This example walks through the entire process from setup to PDF export.

## Step 1: Initial Setup

**Run**: `@setup.mdc`

The system will guide you through:
- Choosing your CV input method (PDF, LinkedIn, or text)
- Importing your CV data
- Setting your preferences
- Creating your professional profile

## Step 2: Job Application Workflow

### Example Job Posting
Let's say you want to apply for this role:

**"Senior Product Designer at GitLab"**
```
We're looking for a Senior Product Designer to join our team. You'll design complex developer tools and admin interfaces for our DevOps platform.

Requirements:
- 5+ years product design experience
- Experience with B2B/enterprise software
- Strong understanding of developer workflows
- Proficiency in Figma and design systems
- Experience with data visualization
- Understanding of technical interfaces

Nice to have:
- Remote team experience
- Open source contribution
- DevOps platform knowledge
```

### Analysis & Generation Process

1. **Analyze the Job**: `@analyze-job-posting.mdc`
   - Paste the job description above
   - System calculates your fit score
   - Identifies gaps and strengths

2. **Verify Experience**: `@verify-experience.mdc`
   - System asks targeted questions about missing/unclear experience
   - You provide specific examples and context
   - All responses are verified and documented

3. **Generate CV**: `@generate-cv.mdc`
   - System creates customized HTML CV
   - Opens automatically in your browser
   - Ready for editing and PDF export

4. **Generate Cover Letter**: `@generate-cover-letter.mdc` (optional)
   - Creates matching cover letter
   - Same editing and export capabilities

## Step 3: Final Review & Export

### In the Browser
1. **Review Content**: Check that everything is accurate and relevant
2. **Edit if Needed**: Enable editing mode to make final adjustments
3. **Try Different Styles**: Use toolbar to test Modern/Tech/Corporate themes
4. **Export PDF**: `Ctrl+P` → Save as PDF

### File Output
You'll have:
- `GitLab-Senior-Product-Designer-2024-01-15.html` (interactive CV)
- `GitLab-Senior-Product-Designer-CoverLetter-2024-01-15.html` (if generated)
- Plus PDF exports ready for submission

## Expected Results

### What the System Does
✅ **Analyzes job fit** - Shows you're 85% match for GitLab role  
✅ **Identifies strengths** - Emphasizes your B2B/enterprise experience  
✅ **Addresses gaps** - Asks about DevOps knowledge, handles honestly  
✅ **Customizes content** - Highlights data visualization and technical interface work  
✅ **Optimizes for ATS** - Includes relevant keywords naturally  
✅ **Creates professional documents** - Ready-to-submit CV and cover letter  

### What You Get
📄 **Accurate CV**: Only verified, interview-defensible content  
🎯 **Highly Targeted**: Specifically customized for the GitLab role  
💼 **Professional Quality**: Industry-standard formatting and design  
⚡ **Time Efficient**: 15-20 minutes vs 2+ hours manual customization  
🔒 **Reputation Safe**: No embellishments or false claims  

## Workflow Summary

```
User Input → Job Analysis → Experience Verification → Document Generation → Browser Editing → PDF Export
     ↓             ↓               ↓                    ↓                 ↓             ↓
   Job URL    Fit Score &    Targeted Questions    Customized HTML    Final Polish    Ready to Submit
            Gap Analysis     & Verification       with Real Data                          PDF
```

## Time Investment
- **First Setup**: 15-20 minutes (one-time only)
- **Each Application**: 10-15 minutes
- **Future Applications**: 5-10 minutes (system learns)

## Success Metrics
- **Accuracy**: 100% verifiable claims
- **Relevance**: 85%+ match for suitable roles
- **Efficiency**: 80% time savings vs manual process
- **Quality**: Professional, ATS-optimized output
- **Learning**: Improves with each application

Ready to revolutionize your job application process? Start with `@setup.mdc`!
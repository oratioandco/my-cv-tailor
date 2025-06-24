# CV Template Instructions

## How to Generate HTML CVs

The `cv-template.html` file uses simple bracket placeholders that should be replaced with actual content when generating a CV.

## Placeholder System

### Basic Information
- `[FULL_NAME]` → User's full name from personal-info.md
- `[PROFESSIONAL_TITLE]` → Customized title for target role
- `[EMAIL]` → Email address
- `[PHONE]` → Phone number  
- `[LOCATION]` → City, Country
- `[PROFESSIONAL_SUMMARY]` → Customized summary paragraph

### Conditional Sections
- `[LINKEDIN_SECTION]` → Only include if LinkedIn URL exists:
  ```html
  <div class="editable" contenteditable="false" data-field="linkedin">
      <span>💼</span> linkedin.com/in/username
  </div>
  ```
- `[PORTFOLIO_SECTION]` → Only include if portfolio URL exists:
  ```html
  <div class="editable" contenteditable="false" data-field="portfolio">
      <span>🌐</span> portfolio-url.com
  </div>
  ```

### Experience Entries
Replace `[EXPERIENCE_ENTRIES]` with:
```html
<div class="experience-entry">
    <div class="experience-header">
        <div>
            <span class="job-title editable" contenteditable="false" data-field="job-title-0">Senior Product Designer</span>
            <span> at </span>
            <span class="company editable" contenteditable="false" data-field="company-0">Datameer</span>
        </div>
        <div class="date-range editable" contenteditable="false" data-field="dates-0">
            January 2020 - Present
        </div>
    </div>
    <div class="job-description">
        <ul class="editable" contenteditable="false" data-field="description-0">
            <li>Led design of enterprise data visualization platform used by Fortune 500 companies</li>
            <li>Increased user engagement by 40% through intuitive interface redesign</li>
            <li>Collaborated with engineering teams to implement complex technical interfaces</li>
        </ul>
    </div>
</div>
```

### Skills Categories
Replace `[SKILLS_CATEGORIES]` with:
```html
<div class="skill-category">
    <h4 class="editable" contenteditable="false" data-field="skill-category-0">Design Tools</h4>
    <div class="skill-list editable" contenteditable="false" data-field="skills-0">
        Figma, Sketch, Adobe Creative Suite, Principle, InVision
    </div>
</div>
<div class="skill-category">
    <h4 class="editable" contenteditable="false" data-field="skill-category-1">Technical Skills</h4>
    <div class="skill-list editable" contenteditable="false" data-field="skills-1">
        HTML/CSS, JavaScript, React, Design Systems, API Design
    </div>
</div>
```

### Education Entries
Replace `[EDUCATION_ENTRIES]` with:
```html
<div class="experience-entry">
    <div class="experience-header">
        <div>
            <span class="job-title editable" contenteditable="false" data-field="degree-0">Bachelor of Design</span>
        </div>
        <div class="date-range editable" contenteditable="false" data-field="edu-dates-0">
            2015 - 2019
        </div>
    </div>
    <div class="editable" contenteditable="false" data-field="school-0" style="color: #3498db; font-weight: 600;">
        University of Applied Sciences
    </div>
    <div class="editable" contenteditable="false" data-field="edu-details-0" style="font-size: 12px; color: #666; margin-top: 5px;">
        Major: Interactive Design, Minor: Computer Science
    </div>
</div>
```

### Optional Sections
Only include if data exists:

**Awards Section:**
Replace `[AWARDS_SECTION]` with:
```html
<div class="section">
    <div class="section-title">Awards & Recognition</div>
    <div class="editable" contenteditable="false" data-field="award-0" style="margin-bottom: 8px;">
        <strong>Design Excellence Award</strong> - Tech Conference 2023 (2023)
    </div>
</div>
```

**Projects Section:**
Replace `[PROJECTS_SECTION]` with:
```html
<div class="section">
    <div class="section-title">Notable Projects</div>
    <div class="experience-entry">
        <div class="experience-header">
            <div>
                <span class="job-title editable" contenteditable="false" data-field="project-title-0">Enterprise Dashboard Redesign</span>
            </div>
            <div class="date-range editable" contenteditable="false" data-field="project-date-0">2023</div>
        </div>
        <div class="editable" contenteditable="false" data-field="project-desc-0" style="font-size: 12px; color: #666; margin-top: 5px;">
            Led complete redesign of data analytics dashboard, resulting in 60% improvement in user task completion rates.
        </div>
    </div>
</div>
```

## Generation Process

1. **Read template**: Load `cv-template.html`
2. **Read user data**: Parse all markdown files in `/data/` folder
3. **Select content**: Choose relevant experiences based on job analysis
4. **Replace placeholders**: Use simple string replacement
5. **Save file**: Write complete HTML to `/outputs/cv/`
6. **Open in browser**: Use system command to open file

## File Naming Convention
`{company}-{role}-{date}.html`

Example: `gitlab-senior-product-designer-2024-01-15.html`

This creates a complete, functional HTML CV that opens immediately in the browser with all editing capabilities intact.
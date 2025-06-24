# PDF Export Guide

## Browser-Based PDF Generation

The CV Builder system uses your browser's built-in PDF generation for maximum compatibility and simplicity.

## How to Export PDF

### Quick Method
1. **Generate your CV** using the CV Builder system
2. **Open the HTML file** in your browser (system does this automatically)
3. **Press `Ctrl+P` (Windows/Linux) or `Cmd+P` (Mac)**
4. **Choose "Save as PDF"** in the destination dropdown
5. **Click "Save"**

### Detailed Steps

#### Step 1: Generate CV
When you run `@generate-cv.mdc`, the system creates an HTML file and opens it in your browser automatically.

#### Step 2: Review & Edit
- Use the toolbar to enable editing if needed
- Make final adjustments to content
- Try different style themes (Modern/Tech/Corporate)
- Ensure everything looks professional

#### Step 3: Export to PDF
1. **Open Print Dialog**:
   - **Windows/Linux**: `Ctrl+P`
   - **Mac**: `Cmd+P`
   - **Or**: Click browser menu → Print

2. **Configure Print Settings**:
   - **Destination**: Choose "Save as PDF"
   - **Layout**: Portrait (should be default)
   - **Paper Size**: A4 (or Letter for US)
   - **Margins**: Default or Minimum
   - **Scale**: 100% (adjust if content doesn't fit)

3. **Advanced Options** (if needed):
   - **Background graphics**: Enable (to keep colors/styling)
   - **Headers and footers**: Disable
   - **Page ranges**: All pages

4. **Save**:
   - Choose filename: `{YourName}-{Company}-{Role}-CV.pdf`
   - Select save location
   - Click "Save"

## PDF Quality Tips

### For Best Results:
✅ **Use Chrome or Edge** - Best PDF generation quality  
✅ **Enable background graphics** - Preserves styling  
✅ **Check print preview** - Ensure content fits properly  
✅ **Use 100% scale** - Maintains professional appearance  
✅ **Disable headers/footers** - Clean, professional look  

### Avoid:
❌ Safari - Sometimes has formatting issues with complex layouts  
❌ Firefox - May not preserve all styling elements  
❌ Scaling below 85% - Text becomes too small  
❌ Adding browser headers/footers - Looks unprofessional  

## Browser-Specific Instructions

### Google Chrome (Recommended)
1. `Ctrl/Cmd+P`
2. Destination: "Save as PDF"
3. More settings → Background graphics: ✅
4. Save

### Microsoft Edge
1. `Ctrl/Cmd+P`
2. Destination: "Microsoft Print to PDF"
3. More settings → Background graphics: ✅
4. Print

### Firefox
1. `Ctrl/Cmd+P`
2. Destination: "Save to PDF"
3. Print backgrounds: ✅ (in Page Setup)
4. Save

## Troubleshooting

### Content Cut Off
- **Solution**: Reduce scale to 90-95% or enable "Fit to page"
- **Check**: Margins are set to "Default" or "Minimum"

### Missing Colors/Styling
- **Solution**: Enable "Background graphics" or "Print backgrounds"
- **Alternative**: Use Chrome for most reliable styling

### Multiple Pages When Expecting One
- **Check**: Content length - may need to remove some sections
- **Solution**: Adjust scale or content to fit on desired pages

### Fonts Look Different
- **Normal**: PDF fonts may vary slightly from browser display
- **Solution**: Use standard fonts (Arial, which is system default)

## File Naming Convention

**Recommended Format**: `FirstName-LastName-Company-Role-CV.pdf`

**Examples**:
- `John-Smith-Google-ProductManager-CV.pdf`
- `Sarah-Johnson-Microsoft-SoftwareEngineer-CV.pdf`
- `Alex-Brown-Startup-UXDesigner-CV.pdf`

## ATS Compatibility

PDFs generated this way are ATS-friendly because:
✅ **Text is selectable** (not images)  
✅ **Standard fonts** used throughout  
✅ **Clean structure** with proper headings  
✅ **No complex graphics** or layouts  
✅ **Reasonable file size** (typically under 1MB)  

## Cover Letters

The same process works for cover letters:
1. Generate cover letter HTML
2. Open in browser
3. `Ctrl/Cmd+P` → Save as PDF
4. Use naming: `FirstName-LastName-Company-Role-CoverLetter.pdf`

## Alternative: Print to Physical Printer

If you need a hard copy:
1. Follow same steps but choose your printer instead of "Save as PDF"
2. Use high-quality paper for professional appearance
3. Print in color if your styling includes colored elements

This browser-based approach ensures your PDFs are always high-quality, ATS-compatible, and generated locally without requiring external services or complex software installations.
# Update Guide for My CV Tailor

## Safe Update Process

My CV Tailor is designed to preserve your personal data during updates. Your CV information, generated documents, and preferences are stored separately from system files.

## What Gets Updated vs. What's Preserved

### ✅ **Preserved During Updates (Your Personal Data)**
- `/data/` - Your structured CV information
- `/outputs/` - Your generated CVs and cover letters  
- `/input/` - Your uploaded CV files
- `start-here.md` - Your manual CV input (if used)

### 🔄 **Updated During Updates (System Files)**
- `/rules/` - AI processing rules (.mdc files)
- `/templates/` - HTML/CSS templates
- Documentation files (README.md, guides, etc.)
- `.github/` - Issue templates and community files

## How to Update

### Option 1: Simple Git Update (Recommended)
```bash
# Navigate to your My CV Tailor folder
cd my-cv-tailor

# Fetch latest changes
git fetch origin

# Update to latest version
git pull origin main
```

**That's it!** Your personal data is automatically preserved.

### Option 2: Manual Backup (Extra Safe)
If you want extra peace of mind:

```bash
# 1. Backup your personal data
cp -r data/ data_backup_$(date +%Y%m%d)/
cp -r outputs/ outputs_backup_$(date +%Y%m%d)/
cp -r input/ input_backup_$(date +%Y%m%d)/

# 2. Update system files
git pull origin main

# 3. Verify everything works
@setup.mdc  # Test the system
```

## Folder Rename (One-Time)

If you're updating from the old "CV Builder" version, rename your folder:

```bash
# From your parent directory (e.g., StudioProjects/)
mv my-custom-cv my-cv-tailor
cd my-cv-tailor
```

## What's Protected by .gitignore

The `.gitignore` file ensures these personal items are never committed:

- All files in `/data/` (except templates)
- All files in `/outputs/` 
- All files in `/input/` (except README.md)
- Your `start-here.md` if you've customized it
- System files like .DS_Store, IDE settings

## Version Compatibility

### Template Updates
- New CV templates are added without breaking existing ones
- Your generated CVs continue to work with new template features
- Style improvements apply automatically

### Rule Updates  
- AI processing rules improve over time
- Your existing data works with updated rules
- New features are additive, not breaking

### Data Format
- Your `/data/` folder format is stable and forward-compatible
- New fields may be added but existing data is preserved
- Migration scripts are provided for major format changes (rare)

## Troubleshooting Updates

### "Git Pull Failed" 
If you get conflicts during `git pull`:

```bash
# Check what's conflicting
git status

# If it's user data files (shouldn't happen with .gitignore):
git stash push -m "user data backup"
git pull origin main
git stash pop
```

### "Missing Dependencies"
If new features require additional setup:
- Check CHANGELOG.md for update notes
- Re-run `@setup.mdc` to configure new features
- Updates are designed to be backward compatible

### "Data Migration Required"
For major version updates (rare):
- Backup your data first (see Option 2 above)
- Follow migration instructions in CHANGELOG.md
- Migration scripts preserve all your existing information

## Best Practices

1. **Update Regularly**: Get bug fixes and new features
2. **Test After Updates**: Run `@setup.mdc` or generate a test CV
3. **Keep Backups**: Though automatic, periodic backups are wise
4. **Read Changelogs**: Check what's new in each update

## Emergency Data Recovery

If something goes wrong:

```bash
# Your data should still be in the folder
ls data/     # Check your CV data
ls outputs/  # Check your generated CVs
ls input/    # Check your uploaded files

# Restore from backup if needed
cp -r data_backup_YYYYMMDD/* data/
```

## Getting Help

- 📖 Check CHANGELOG.md for update details
- 🐛 Report issues via GitHub issue templates  
- ❓ Ask questions in GitHub Discussions
- 🔄 Rollback: `git checkout <previous-version-tag>`

---

**Remember**: My CV Tailor updates improve the system while keeping your personal career data safe and private. Updates only enhance functionality - your CV information remains yours and stays local.
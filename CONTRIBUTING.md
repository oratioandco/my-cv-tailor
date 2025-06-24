# Contributing to My CV Tailor

Thank you for your interest in contributing to My CV Tailor! This project aims to create the best AI-powered CV generation system that prioritizes accuracy, privacy, and user control.

## 🎯 Project Vision

My CV Tailor is a **safety-first, local-only** CV generation system that:
- Never hallucinates or makes up information about users
- Learns and improves over time through verified user interactions
- Works completely offline with any AI assistant that has file system access
- Prioritizes user privacy and control over their professional data

## 🚀 Quick Start for Contributors

### Prerequisites
- An AI assistant with file system access (Cursor, Claude Code, etc.)
- Basic understanding of markdown and HTML
- Familiarity with conversational AI workflows

### Getting Started
1. Fork the repository
2. Clone your fork locally
3. Test the system by running `@setup.mdc` in your AI assistant
4. Review the [task list](tasks/tasks-prd-cv-builder-open-source.md) for contribution opportunities

## 🤝 How to Contribute

### 1. Bug Reports
- Use the bug report template when creating issues
- Include your operating system and AI assistant details
- Provide steps to reproduce the issue
- Share relevant error messages or unexpected behavior

### 2. Feature Requests
- Check existing issues to avoid duplicates
- Use the feature request template
- Explain the problem your feature would solve
- Consider how it aligns with our safety-first philosophy

### 3. Documentation Improvements
- Fix typos, clarify instructions, add examples
- Update documentation when features change
- Translate documentation (following our style guide)

### 4. Template Contributions
- Create new CV/cover letter templates
- Follow our template standards (see below)
- Test templates across different browsers and PDF exports
- Ensure ATS compatibility

### 5. Code Contributions
- Follow the existing .mdc rule structure
- Maintain the safety-first approach (no hallucination)
- Update relevant documentation
- Test across multiple AI platforms if possible

## 📋 Template Contribution Standards

### CV Templates
- **HTML Structure**: Use semantic HTML elements for ATS compatibility
- **CSS Styling**: Inline CSS only for portability
- **Print Optimization**: Must render properly when printed to PDF
- **Responsive Design**: Should work on different screen sizes
- **Accessibility**: Follow WCAG guidelines for screen readers

### Template Checklist
- [ ] Uses placeholder system `[PLACEHOLDER_NAME]` for content
- [ ] Includes interactive editing toolbar
- [ ] Supports multiple themes (Modern, Tech, Corporate)
- [ ] Tests clean in Chrome print-to-PDF
- [ ] ATS-friendly structure (no complex graphics or tables)
- [ ] Professional appearance and typography
- [ ] Auto-save functionality works
- [ ] Keyboard navigation supported

### Testing Your Template
1. Generate a CV using your template
2. Test inline editing functionality
3. Export to PDF using browser print function
4. Verify ATS compatibility (text selectable, proper structure)
5. Test in different browsers (Chrome, Firefox, Safari, Edge)

## 🛡️ Safety & Quality Guidelines

### Safety-First Principles
- **Never assume or generate content** not explicitly provided by users
- **Always verify information** through targeted questions
- **Maintain transparency** about what data is verified vs. unverified
- **Protect user privacy** - all processing happens locally
- **Preserve accuracy** - every claim must be interview-defensible

### Code Quality Standards
- **Clear Documentation**: Every .mdc rule should have clear instructions
- **Error Handling**: Gracefully handle missing files or malformed data
- **User Feedback**: Provide clear status updates and guidance
- **Testing**: Verify functionality across different platforms
- **Backwards Compatibility**: Don't break existing user data

## 🏗️ Development Workflow

### For .mdc Rule Development
1. **Study existing rules** in the `/rules` directory
2. **Follow the conversational pattern** established in `setup.mdc`
3. **Test thoroughly** with different input scenarios
4. **Document any new placeholders** or data requirements
5. **Update template instructions** if needed

### For Template Development
1. **Start with existing template** as a base
2. **Test with sample data** before submitting
3. **Verify PDF export quality** across browsers
4. **Check ATS compatibility** using online ATS testing tools
5. **Document any special requirements** or features

### Pull Request Process
1. **Create a feature branch** from main
2. **Make your changes** following our standards
3. **Test thoroughly** across different scenarios
4. **Update documentation** as needed
5. **Submit pull request** using our template
6. **Respond to feedback** and iterate as needed

## 🔍 AI Platform Compatibility

### Supported Platforms
- **Cursor**: Primary development platform
- **Claude Code**: Full compatibility
- **Other AI Assistants**: Any with file system read/write access

### Platform Testing
When contributing features that might affect platform compatibility:
- Test with multiple AI assistants if possible
- Document any platform-specific requirements
- Report compatibility issues in your PR description
- Consider graceful degradation for limited platforms

## 📊 Metrics & Success

### What We Track
- **User Adoption**: GitHub stars, forks, clones
- **Community Health**: Issue response time, contribution volume
- **Quality Metrics**: Bug reports, user feedback
- **Template Usage**: Downloads and adoption of community templates

### How You Can Help
- **Share your success stories** using My CV Tailor
- **Report metrics** on template performance and user feedback
- **Suggest improvements** based on real-world usage
- **Help other users** in issues and discussions

## 📝 Documentation Style Guide

### Writing Style
- **Clear and concise** - assume users are tech-savvy but new to My CV Tailor
- **Step-by-step instructions** with concrete examples
- **Safety reminders** about accuracy and verification
- **Troubleshooting sections** for common issues

### Markdown Conventions
- Use consistent heading levels
- Include code blocks for file names and commands
- Add emojis sparingly for visual organization
- Link to relevant sections and external resources

## 🏷️ Issue Labels

### Priority Labels
- `priority: high` - Critical bugs or security issues
- `priority: medium` - Feature requests or minor bugs
- `priority: low` - Documentation or nice-to-have improvements

### Type Labels
- `type: bug` - Something isn't working correctly
- `type: feature` - New functionality request
- `type: documentation` - Documentation improvements
- `type: template` - CV/cover letter template related
- `type: platform` - AI platform compatibility

### Status Labels
- `status: needs-info` - Waiting for more information
- `status: in-progress` - Someone is working on this
- `status: ready-for-review` - Ready for maintainer review

## 📞 Getting Help

### Where to Ask Questions
- **GitHub Issues**: Bug reports and feature requests
- **GitHub Discussions**: General questions and community chat
- **Documentation**: Check README and example workflows first

### Response Expectations
- **Bug reports**: Within 48 hours
- **Feature requests**: Within 1 week
- **Pull requests**: Within 1 week for initial review
- **Questions**: Community-driven, best effort response

## 🎉 Recognition

### Contributors
All contributors are recognized in our README and release notes. We value:
- **Code contributions** of any size
- **Documentation improvements** and translations
- **Bug reports** with clear reproduction steps
- **Template contributions** that expand user options
- **Community support** helping other users

### Maintainer Path
Regular contributors who demonstrate:
- Understanding of our safety-first philosophy
- Quality contributions across multiple areas
- Helpful community engagement
- Platform testing and compatibility work

May be invited to become maintainers with repository access.

## 📄 License

By contributing to My CV Tailor, you agree that your contributions will be licensed under the same MIT License that covers the project.

---

**Thank you for helping make My CV Tailor the best AI-powered CV generation system available!** 

Your contributions help job seekers worldwide create accurate, professional CVs while maintaining complete control over their personal data.
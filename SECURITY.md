# Security Policy

## Security Philosophy

My CV Tailor is designed with security and privacy as core principles. The system processes sensitive professional and career information, so we take security seriously.

### Core Security Principles

1. **Local-Only Processing**: All CV generation happens locally on your machine
2. **No Cloud Dependencies**: No data is ever sent to external servers or APIs
3. **User Control**: You maintain complete control over your professional data
4. **Transparency**: All processing is visible and auditable through file system changes
5. **Privacy by Design**: Personal information never leaves your local environment

## Supported Versions

We provide security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | ✅ Yes             |
| < 1.0   | ❌ No (development versions) |

## Security Model

### Data Processing
- **Input**: CV data imported from user-provided files (PDF, LinkedIn exports, text)
- **Processing**: Local AI assistant reads/writes files in project directory
- **Storage**: All data stored in local markdown files on user's machine
- **Output**: HTML and PDF files generated locally for user

### Threat Model

**What We Protect Against:**
- Accidental data exposure through cloud services
- Unauthorized access to career information
- Data persistence in AI model training
- Information leakage through external APIs

**What We Don't Protect Against:**
- Local machine compromise (malware, physical access)
- AI assistant security vulnerabilities
- User sharing of generated files
- Browser security when viewing generated CVs

### Data Flow Security

```
User Input → Local AI Assistant → Local File System → Generated CV
    ↓              ↓                     ↓              ↓
No Upload    No Cloud API      Local Storage    User Control
```

## Privacy Considerations

### Personal Information Handling
- **Name, Contact Info**: Stored in local `personal-info.md` file
- **Career History**: Individual files per experience in `experiences/` folder
- **Skills & Education**: Categorized in local markdown files
- **Job Applications**: Analysis stored locally in `jobs/` folder

### AI Assistant Integration
- My CV Tailor uses your AI assistant's existing security model
- No additional data collection beyond standard file operations
- Processing happens within your AI assistant's security context
- No special permissions or network access required

### File System Security
- Uses standard file read/write operations
- Respects your operating system's file permissions
- Creates files only in the project directory
- No system-level changes or installations required

## Reporting Security Vulnerabilities

### How to Report

If you discover a security vulnerability in My CV Tailor, please report it responsibly:

1. **DO NOT** create a public GitHub issue for security vulnerabilities
2. **DO** email the maintainers directly at [security contact - to be added in repository settings]
3. **DO** provide detailed information about the vulnerability
4. **DO** give us reasonable time to address the issue before public disclosure

### What to Include

When reporting a security vulnerability, please include:

- **Description**: Clear description of the vulnerability
- **Impact**: What data or functionality could be affected
- **Reproduction**: Steps to reproduce the issue
- **Environment**: AI platform, operating system, browser details
- **Severity**: Your assessment of the risk level

### Response Process

1. **Acknowledgment**: We'll acknowledge receipt within 24 hours
2. **Assessment**: We'll assess the vulnerability and determine severity
3. **Fix Development**: We'll develop and test a fix
4. **Disclosure**: We'll coordinate disclosure timing with you
5. **Release**: We'll release a security update with appropriate credit

### Security Response Timeline

- **Critical vulnerabilities**: Fix within 48 hours
- **High severity**: Fix within 1 week
- **Medium severity**: Fix within 2 weeks
- **Low severity**: Fix in next regular release

## Security Best Practices for Users

### System Security
- **Keep your AI assistant updated** to the latest version
- **Use updated browsers** for HTML/PDF functionality
- **Maintain OS security** with regular updates and antivirus
- **Secure your machine** with appropriate access controls

### Data Protection
- **Backup your CV data** regularly (the entire `my-cv-tailor/` folder)
- **Use version control** (Git) to track changes to your professional data
- **Secure your generated files** when sharing (remove sensitive info if needed)
- **Control file sharing** - be mindful of what CV versions you share

### AI Assistant Security
- **Understand your AI assistant's data policy** regarding local files
- **Review file permissions** granted to your AI assistant
- **Monitor file system changes** during CV generation
- **Use trusted AI platforms** with established security practices

## Common Security Questions

### Q: Does My CV Tailor send my data anywhere?
**A:** No. My CV Tailor processes everything locally. Your CV data never leaves your machine.

### Q: Can my AI assistant see my CV data?
**A:** Yes, but only locally. Your AI assistant reads your CV files to generate customized versions, but this happens entirely on your machine.

### Q: Are generated CVs secure?
**A:** Generated HTML/PDF files are standard documents. Secure them like any other important document on your computer.

### Q: What about browser security when editing CVs?
**A:** The HTML CVs use standard browser security features. Use updated browsers and standard web security practices.

### Q: Can I audit what My CV Tailor does?
**A:** Yes. All processing is visible through file system changes. You can review all `.mdc` rules and generated files.

## Security Updates

### Notification Methods
Security updates will be communicated through:
- GitHub Security Advisories
- Release notes in CHANGELOG.md
- Repository README updates
- GitHub repository watch notifications

### Update Process
1. **Assessment**: We evaluate all reported security issues
2. **Development**: Security fixes are developed and tested
3. **Release**: Updates are released with clear security advisory
4. **Communication**: Community is notified through multiple channels

## Compliance & Standards

### Industry Alignment
- Follows OWASP guidelines for secure software development
- Implements privacy-by-design principles
- Aligns with data minimization best practices
- Supports user control and transparency requirements

### Regulatory Considerations
- **GDPR Compliance**: Local processing supports data subject rights
- **CCPA Compliance**: User control meets privacy requirements  
- **Industry Standards**: Professional data handling aligns with HR and recruiting standards

## Contact Information

### Security Contact
- **Primary**: [Security email to be configured in repository settings]
- **Backup**: GitHub repository maintainers
- **Emergency**: Create a private security advisory on GitHub

### Community Security
- **General Questions**: Use the question issue template
- **Public Discussions**: GitHub Discussions (for non-sensitive topics)
- **Documentation Issues**: Regular GitHub issues

---

**Remember**: My CV Tailor's security is built on local processing and user control. Keep your system secure, and My CV Tailor will help protect your professional information while generating excellent job application materials.
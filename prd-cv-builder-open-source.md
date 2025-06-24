# Product Requirements Document: My CV Tailor - Open Source

## Introduction/Overview

My CV Tailor is an AI-powered, conversational CV generation system designed for tech-savvy job seekers using AI coding assistants. Unlike traditional CV tools that rely on templates or AI systems that hallucinate content, My CV Tailor creates a private, local, self-learning system that verifies user experience and generates highly customized CVs and cover letters for each job application.

The system transforms CV customization from a 2-hour manual process into a 10-15 minute guided conversation while maintaining complete accuracy and building a reusable knowledge base that improves over time.

**Core Problem Solved:** Job seekers waste hours manually customizing CVs for each application, often struggling with relevance, accuracy, and ATS optimization, while existing AI tools risk generating false information that could damage professional reputation.

## Goals

1. **Accuracy First:** Enable users to create 100% verified, interview-defensible CVs with zero false claims
2. **Efficiency:** Reduce CV customization time from 2+ hours to 10-15 minutes per application
3. **Learning System:** Build a personal knowledge base that improves with each job application
4. **Professional Quality:** Generate ATS-optimized, professionally formatted documents
5. **Open Source Adoption:** Achieve 1,000+ GitHub stars and 500+ forks within 6 months
6. **Community Growth:** Enable template contributions and platform integrations
7. **Self-Contained:** Provide completely local, private solution requiring no external services

## User Stories

### Primary User: Tech-Savvy Job Seeker
- **As a software engineer using Cursor,** I want to import my CV data once and generate customized versions for each job application, so that I can apply to more positions with higher quality submissions
- **As a product manager using Claude Code,** I want the system to analyze job postings and identify experience gaps, so that I can honestly assess my fit and prepare better applications
- **As a designer changing career focus,** I want to verify my transferable skills through targeted questions, so that I can confidently represent my qualifications without overselling
- **As a senior professional,** I want my CV system to learn from each application, so that future customizations become faster and more accurate

### Secondary User: Career-Focused Individual
- **As someone applying to multiple roles,** I want to track which experiences and skills are most effective, so that I can optimize my application strategy
- **As a job seeker concerned about AI accuracy,** I want every CV claim to be traceable to verified information, so that I never get caught misrepresenting my experience in interviews

## Functional Requirements

### Core System Requirements
1. **Conversational Setup:** System must provide guided onboarding via `@setup.mdc` rule that walks users through CV import and preference configuration
2. **Multi-Format Import:** System must support CV import from PDF files, LinkedIn exports, LinkedIn data downloads, and manual text input
3. **Data Verification:** System must ask targeted questions to verify user experience and never generate unverified claims
4. **Job Analysis:** System must analyze job postings from text or URLs and calculate honest fit scores with gap identification
5. **Content Customization:** System must select relevant experiences and customize language based on job requirements and company culture
6. **HTML Generation:** System must create interactive HTML files with inline editing capabilities and real user data
7. **PDF Export:** System must enable professional PDF generation through browser print functionality
8. **Cover Letter Generation:** System must create matching cover letters with same editing and export capabilities

### Data Management Requirements
9. **Structured Storage:** System must organize user data in individual markdown files (one per experience, skill category, education entry)
10. **Version Control:** System must preserve original CV data while tracking modifications and verifications
11. **Preference Storage:** System must remember user preferences for CV style, content depth, and targeting approach
12. **Learning Capability:** System must improve recommendations based on successful application patterns

### Safety & Accuracy Requirements
13. **No Hallucination:** System must never add information not explicitly provided by the user
14. **Verification Tracking:** System must log which claims have been verified and which need clarification
15. **Honest Assessment:** System must provide accurate job fit scores even when revealing significant gaps
16. **Interview Defensibility:** System must ensure every CV claim can be confidently discussed in interviews

### Technical Requirements
17. **File System Integration:** System must work with any AI tool that can read/write local files
18. **Markdown-Based:** System must use .md files for data storage and .mdc files for AI processing rules
19. **Template System:** System must use simple placeholder replacement for HTML generation
20. **Cross-Platform:** System must work on Windows, macOS, and Linux with any modern browser
21. **Offline Capable:** Generated HTML/CSS files must work without internet connectivity

### User Experience Requirements
22. **Progressive Enhancement:** First setup takes 15-20 minutes, subsequent applications take 5-10 minutes
23. **Error Recovery:** System must gracefully handle file reading errors and provide clear guidance
24. **Multi-Style Support:** System must offer Modern, Tech, and Corporate CV styling options
25. **ATS Optimization:** Generated documents must be ATS-compatible with proper structure and keywords

## Non-Goals (Out of Scope)

1. **Web Application:** This is not a SaaS platform or web service
2. **Cloud Storage:** No cloud sync or remote data storage capabilities
3. **Social Features:** No sharing, collaboration, or social networking features
4. **Job Board Integration:** No direct integration with job posting platforms
5. **Interview Preparation:** No interview question generation or coaching features
6. **Salary Negotiation:** No compensation analysis or negotiation guidance
7. **Portfolio Management:** No project portfolio or work sample management
8. **Team/Enterprise Features:** No multi-user or organization-level capabilities
9. **Mobile App:** Desktop/laptop only, no mobile application
10. **Real-time Collaboration:** No simultaneous multi-user editing

## Design Considerations

### User Interface
- **Conversational Flow:** Primary interaction through AI chat with clear step-by-step guidance
- **HTML Templates:** Clean, professional layouts optimized for both screen viewing and PDF printing
- **Inline Editing:** Browser-based editing with live preview and auto-save functionality
- **Multiple Themes:** Switchable styling options (Modern, Tech, Corporate) without content changes

### File Organization
- **Modular Structure:** Each experience, skill, and qualification in separate files for maximum flexibility
- **Clear Naming:** Intuitive file names and folder structure for easy manual navigation
- **Template Separation:** HTML templates separate from content for easy customization

### Accessibility
- **Screen Reader Compatible:** Proper HTML structure and semantic elements
- **High Contrast:** Readable color schemes that work in print and on screen
- **Keyboard Navigation:** Full functionality without requiring mouse interaction

## Technical Considerations

### AI Platform Compatibility
- **Rule-Based System:** Uses .mdc files that can be read by any AI with file system access
- **Cursor Optimization:** Leverages Cursor's document attachment and file management features
- **Claude Code Integration:** Works seamlessly with Claude Code's local file capabilities
- **Extensible Design:** Architecture supports additional AI platforms with minimal modification

### File System Requirements
- **Read/Write Access:** AI must be able to create, modify, and organize files in project directory
- **HTML Generation:** AI must be able to create complete HTML files and open them in browser
- **Data Persistence:** User data and preferences stored locally in structured markdown files

### Performance Considerations
- **Local Processing:** All operations happen locally for maximum speed and privacy
- **Incremental Updates:** Only modified sections need regeneration, not entire CV
- **Efficient Templates:** Simple string replacement avoids complex rendering engines

## Success Metrics

### Adoption Metrics
- **GitHub Stars:** 1,000+ within 6 months of public release
- **Repository Forks:** 500+ indicating active community interest
- **Clone Count:** 5,000+ downloads showing actual usage
- **Issue Engagement:** Active community participation in bug reports and feature requests

### Quality Metrics
- **User Retention:** Users generating multiple CVs (indicating system value)
- **Template Contributions:** Community-submitted templates and improvements
- **Documentation Quality:** Low ratio of support issues to total users
- **Success Stories:** User testimonials about job application success

### Technical Metrics
- **Cross-Platform Compatibility:** Confirmed working on Windows, macOS, Linux
- **AI Platform Support:** Compatibility with Cursor, Claude Code, and potential others
- **Error Rate:** Low incidence of setup or generation failures
- **Performance:** Sub-30-second CV generation times

## Open Questions

1. **Licensing:** Should this use MIT, Apache 2.0, or another open source license?
2. **Contribution Guidelines:** What standards should community contributions meet?
3. **Template Standards:** Should there be specific requirements for community-submitted templates?
4. **Internationalization:** Should initial release support multiple languages or start English-only?
5. **AI Model Requirements:** Any minimum capability requirements for compatible AI models?
6. **Version Control Integration:** Should the system integrate with Git for tracking CV evolution?
7. **Privacy Documentation:** What privacy guarantees should be explicitly documented?
8. **Commercial Use:** Any restrictions on commercial use or derivative products?

## Implementation Priority

### Phase 1: Core Release (Immediate)
- All existing functionality working and documented
- Comprehensive README with setup instructions
- Example workflow and templates
- Basic issue templates and contribution guidelines

### Phase 2: Community Building (Month 2-3)
- Enhanced documentation and video tutorials
- Community template submission process
- Additional AI platform testing and compatibility
- User feedback integration

### Phase 3: Ecosystem Growth (Month 4-6)
- Community-contributed templates and themes
- Additional language support
- Advanced customization options
- Integration guides for other AI platforms

This PRD serves as the foundation for releasing CV Builder as a valuable open-source tool that empowers job seekers while building a strong developer community around intelligent, privacy-focused career tools.
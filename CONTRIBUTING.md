# Contributing to Nudg

Thank you for your interest in contributing to Nudg! We're building a healthcare platform to improve medication adherence and patient outcomes, and we welcome contributions from developers, healthcare professionals, designers, and community members.

---

## 🎯 Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

---

## ❓ Questions or Need Help?

- 📧 Email: developers@nudg.com
- 💬 Discussions: [GitHub Discussions](https://github.com/abdirzakali/Nudg/discussions)
- 🐛 Issues: [GitHub Issues](https://github.com/abdirzakali/Nudg/issues)

---

## 🚀 Getting Started

1. **Fork** the repository
2. **Clone** your fork: `git clone https://github.com/YOUR_USERNAME/Nudg.git`
3. **Create a branch** for your feature: `git checkout -b feature/your-feature-name`
4. **Follow** our development setup in [SETUP.md](./SETUP.md)
5. **Make** your changes
6. **Test** your changes thoroughly
7. **Commit** with clear, descriptive messages
8. **Push** to your fork
9. **Submit** a pull request to the main repository

---

## 📋 Types of Contributions

### 🐛 Bug Reports
- Check [existing issues](https://github.com/abdirzakali/Nudg/issues) first to avoid duplicates
- Include:
  - Clear description of the bug
  - Steps to reproduce
  - Expected vs actual behavior
  - Screenshots/logs if applicable
  - Your environment (OS, browser, app version)

### ✨ Feature Requests
- Describe the use case and problem it solves
- Explain the expected behavior
- Provide mockups or examples if helpful
- Consider healthcare compliance implications

### 📝 Documentation
- Grammar/clarity improvements
- Setup guide enhancements
- API documentation updates
- User guide contributions

### 💻 Code Contributions
- Bug fixes
- Performance improvements
- New features (check with maintainers first!)
- Refactoring and code quality improvements

### 🎨 Design Contributions
- UI/UX improvements
- Accessibility enhancements (WCAG 2.1 AA minimum)
- Design system updates
- User research insights

---

## 🏥 Healthcare-Specific Guidelines

Since Nudg handles sensitive health data, all contributions must consider:

### Security
- Never commit API keys, credentials, or tokens
- Use environment variables for secrets
- Follow HIPAA encryption requirements
- Sanitize all user inputs

### Privacy
- Don't add unnecessary data collection
- Implement data minimization principles
- Include privacy impact assessments for new features
- Honor user consent and preferences

### Clinical Accuracy
- GLP-1 medication information must be evidence-based
- Consult medical literature for feature design
- Include disclaimers where appropriate
- Work with healthcare advisors for clinical features

### Accessibility
- Ensure WCAG 2.1 AA compliance minimum
- Test with screen readers
- Support keyboard navigation
- Consider users with low health literacy

---

## 💻 Development Standards

### Code Style
- Follow project-specific linters and formatters
- Run `npm run lint` or `python -m flake8` before committing
- Write clear, commented code
- Use meaningful variable/function names

### Testing
- Write tests for new features (minimum 80% coverage)
- Run existing test suite before submitting PR: `npm run test`
- Include both unit and integration tests
- Test on multiple devices/browsers (if frontend)

### Commit Messages
```
[TYPE] Short description (50 chars max)

Detailed explanation (if needed):
- Why the change was made
- What problem it solves
- Any relevant issues/PRs

Fixes: #123
Related: #456
```

**Types:** feat, fix, docs, style, refactor, test, chore, perf

Example:
```
feat: Add calendar invite generation for dose increases

- Generate Google Calendar invites 7 days before scheduled dose increase
- Support Outlook and Apple Calendar via CalDAV standard
- Include medication details and side effect tips in invite description

Fixes: #89
```

### Branching Strategy
- `main` - production-ready code
- `develop` - staging/integration branch
- `feature/` - new features
- `fix/` - bug fixes
- `docs/` - documentation updates
- `chore/` - maintenance tasks

---

## 🔄 Pull Request Process

1. **Update** documentation if needed (README, API docs, etc.)
2. **Add** tests and ensure all pass
3. **Follow** code style guidelines
4. **Fill out** the PR template completely
5. **Link** related issues
6. **Request** review from maintainers
7. **Address** feedback and requested changes
8. **Ensure** CI/CD checks pass

### PR Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Related Issues
Fixes #(issue number)

## Testing
Describe how you tested this change

## Healthcare/Privacy Considerations
Any impact on data security, privacy, or clinical accuracy?

## Checklist
- [ ] My code follows the style guidelines
- [ ] I have performed a self-review
- [ ] I have commented my code, particularly in complex areas
- [ ] I have updated relevant documentation
- [ ] My changes generate no new warnings
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] New and existing unit tests pass locally with my changes
- [ ] Any dependent changes have been merged and published
```

---

## ✅ Review Process

1. **Automated Checks**
   - CI/CD pipeline runs (tests, linting, security scans)
   - Code coverage maintained or improved
   - All checks must pass

2. **Code Review**
   - At least 1 maintainer review required
   - Healthcare/privacy review for sensitive changes
   - Constructive feedback provided
   - Changes requested addressed before merge

3. **Approval & Merge**
   - PR approved by maintainers
   - All conversations resolved
   - Branch up-to-date with main
   - Squash-merge to main

---

## 🔒 Security Guidelines

### What NOT to Commit
- API keys, tokens, or credentials
- Private keys or certificates
- Database passwords
- User PII or PHI
- Third-party secrets

### Security Best Practices
- Always use HTTPS for external APIs
- Validate and sanitize all inputs
- Use parameterized queries to prevent SQL injection
- Implement rate limiting on endpoints
- Log security events (without logging sensitive data)
- Report vulnerabilities responsibly (see [SECURITY.md](./SECURITY.md))

---

## 📚 Documentation Standards

When updating documentation:

### README Sections
- Keep current and accurate
- Include examples where helpful
- Update roadmap with completed items
- Link to detailed guides

### Setup & Installation
- Step-by-step instructions
- Include all prerequisites
- Troubleshooting section
- Example `.env` files (without secrets)

### API Documentation
- Clear endpoint descriptions
- Request/response examples
- Error codes and meanings
- Authentication requirements

### Code Comments
- Explain the "why", not the "what"
- Use for complex algorithms
- Link to related issues/docs
- Keep comments current with code changes

---

## 🎓 Getting Help

### Resources
- [Setup Guide](./SETUP.md)
- [API Documentation](./API.md)
- [Architecture Overview](./ARCHITECTURE.md)
- [GLP-1 Medication Guide](./docs/glp1-guide.md)

### Learning About GLP-1
- [GLP-1 Receptor Agonists - FDA](https://www.fda.gov/...)
- [ADA Standards of Care](https://diabetes.org/...)
- Patient resources and forums

### Project Maintainers
- @abdirzakali (Lead)
- See [MAINTAINERS.md](./MAINTAINERS.md) for team members

---

## 📊 Recognition

Contributors are recognized:
- In repository via Git history
- In [CONTRIBUTORS.md](./CONTRIBUTORS.md)
- In release notes for significant contributions
- Monthly contributor spotlight

---

## 📜 Legal

By contributing, you agree that:
- Your contributions will be licensed under the same license as the project (MIT)
- You have the right to contribute the code
- You grant the project maintainers the right to use your contributions

---

## 🙏 Thank You!

Thank you for contributing to Nudg. Together, we're improving medication adherence and health outcomes for millions of patients.

**Questions?** Reach out to developers@nudg.com


# Contributing to Executive Dashboard

Thank you for your interest in contributing to the Executive Dashboard! This document provides guidelines and information for contributors.

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic knowledge of HTML, CSS, and JavaScript
- Git for version control

### Development Setup
1. Fork the repository on GitHub
2. Clone your fork locally:
   ```bash
   git clone https://github.com/yourusername/exec-dashboard.git
   cd exec-dashboard
   ```
3. Open `index.html` in your browser to start developing
4. Make changes and refresh the browser to see results

## 📝 How to Contribute

### Reporting Issues
- Use the GitHub Issues tab
- Provide a clear description of the problem
- Include steps to reproduce the issue
- Add screenshots if helpful
- Mention your browser and operating system

### Suggesting Features
- Open a GitHub Issue with the "feature request" label
- Describe the feature and its benefits
- Explain how it fits with the project's goals
- Consider implementation complexity

### Code Contributions

#### 1. Choose an Issue
- Look for issues labeled "good first issue" for beginners
- Comment on the issue to let others know you're working on it
- Ask questions if anything is unclear

#### 2. Development Process
- Create a new branch for your feature:
  ```bash
  git checkout -b feature/your-feature-name
  ```
- Make your changes in small, logical commits
- Test your changes thoroughly in multiple browsers
- Follow the existing code style and patterns

#### 3. Testing Your Changes
- Open `index.html` in multiple browsers
- Test all existing functionality still works
- Test your new feature thoroughly
- Try importing/exporting configurations
- Check mobile responsiveness

#### 4. Submitting Changes
- Commit your changes with clear messages:
  ```bash
  git commit -m "Add feature: brief description"
  ```
- Push to your fork:
  ```bash
  git push origin feature/your-feature-name
  ```
- Open a Pull Request on GitHub
- Describe what your changes do and why
- Reference any related issues

## 🎨 Code Style Guidelines

### HTML
- Use semantic HTML5 elements
- Maintain proper indentation (2 spaces)
- Add comments for complex sections
- Keep accessibility in mind

### CSS
- Use the existing CSS structure within the `<style>` tag
- Follow BEM-like naming conventions
- Group related styles together
- Add comments for complex styling

### JavaScript
- Use descriptive variable and function names
- Add comments for complex logic
- Follow the existing function organization
- Maintain the modular structure

## 📊 Architecture Overview

### File Structure
```
exec-dashboard/
├── index.html                    # Main application file
├── default-dashboard-config.json # Default configuration
├── README.md                     # Documentation
├── LICENSE                       # MIT license
└── CONTRIBUTING.md              # This file
```

### Code Organization (within index.html)
- **HTML Structure**: Layout and form elements
- **CSS Styles**: All styling in `<style>` section
- **JavaScript Modules**:
  - Global data storage (`expenses`, `initiatives`)
  - Expense management functions
  - Initiative management functions  
  - Chart generation and updates
  - JSON export/import functionality
  - localStorage persistence

### Key Functions to Understand
- `updateChart()`: Regenerates the capital burn and roadmap visualization
- `renderExpenses()` / `renderInitiatives()`: Update the data tables
- `exportToJson()` / `loadDashboardData()`: Handle data persistence
- `autoSave()`: Automatic localStorage backup

## 🔧 Common Tasks

### Adding a New Expense Field
1. Add the field to the expense object structure
2. Update `renderExpenses()` to display the field
3. Update `updateExpense()` to handle changes
4. Update the JSON export format if needed

### Adding a New Chart Type
1. Study the existing Chart.js configuration
2. Add new dataset to the `datasets` array
3. Update chart options if needed
4. Test with various data scenarios

### Improving Mobile Experience
1. Focus on the CSS media queries
2. Test on actual mobile devices
3. Consider touch interaction improvements
4. Optimize table layouts for small screens

## 🧪 Testing Guidelines

### Browser Testing
Test in at least these browsers:
- Chrome (latest)
- Firefox (latest)
- Safari (if on Mac)
- Edge (latest)

### Feature Testing Checklist
- [ ] All existing functionality works
- [ ] New feature works as expected
- [ ] Data persists correctly (localStorage)
- [ ] Export/import still works
- [ ] Charts render properly
- [ ] Mobile layout is acceptable
- [ ] No JavaScript errors in console

### Data Scenarios to Test
- Empty configuration
- Single expense/initiative
- Many expenses/initiatives  
- Very large numbers
- Very long time periods
- Edge cases (negative numbers, etc.)

## 📋 Pull Request Guidelines

### Before Submitting
- [ ] Code follows existing style
- [ ] All features tested in multiple browsers
- [ ] No console errors
- [ ] Documentation updated if needed
- [ ] Commit messages are clear

### PR Description Should Include
- Summary of changes
- Why the change is beneficial
- Screenshots if UI changes
- Testing steps performed
- Any breaking changes

### Review Process
1. Automated checks (if any) must pass
2. Manual review by maintainers
3. Feedback addressed and changes made
4. Final approval and merge

## 🏷️ Labels and Issues

### Issue Labels
- `bug`: Something isn't working
- `enhancement`: New feature or improvement
- `documentation`: Documentation improvements
- `good first issue`: Good for newcomers
- `help wanted`: Looking for contributors

### Priority Levels
- `priority: high`: Critical fixes or important features
- `priority: medium`: Normal improvements
- `priority: low`: Nice-to-have enhancements

## 🤔 Questions?

If you have questions:
1. Check existing issues and discussions
2. Ask in a GitHub Discussion
3. Comment on relevant issues
4. Reach out to maintainers

## 📜 Code of Conduct

Please be respectful and constructive in all interactions. This project welcomes contributors of all skill levels and backgrounds.

Thank you for contributing to making this tool better for everyone! 🎉
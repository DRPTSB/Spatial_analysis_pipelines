# Contributing to Spatial Analysis Pipelines

Thank you for your interest in contributing to this repository! We welcome contributions from the community to help make spatial data analysis more accessible.

## 📋 Table of Contents

- [Ways to Contribute](#ways-to-contribute)
- [Getting Started](#getting-started)
- [Contribution Guidelines](#contribution-guidelines)
- [Tutorial Format](#tutorial-format)
- [Code of Conduct](#code-of-conduct)

---

## Ways to Contribute

### 📝 Content Contributions
- **New Tutorials**: Step-by-step guides for spatial analysis techniques
- **Best Practices**: Documented guidelines and recommendations
- **Code Examples**: Working code snippets and notebooks
- **Bug Reports**: Issues with existing content or code

### 🔍 Review Contributions
- **Proofread**: Fix typos and improve clarity
- **Technical Review**: Verify code and methods are accurate
- **Accessibility**: Ensure content is beginner-friendly

### 💬 Community Contributions
- **Answer Questions**: Help others in Discussions
- **Share Feedback**: Suggest improvements
- **Test Tutorials**: Report issues with instructions

---

## Getting Started

### Prerequisites
- GitHub account
- Basic knowledge of Markdown
- Familiarity with spatial analysis (for technical contributions)

### Setting Up

1. **Fork the Repository**
   ```bash
   # Clone your fork
   git clone https://github.com/YOUR-USERNAME/Spatial_analysis_pipelines.git
   cd Spatial_analysis_pipelines
   ```

2. **Create a Branch**
   ```bash
   git checkout -b feature/your-contribution-name
   ```

3. **Make Your Changes**
   - Add/edit files following our guidelines
   - Test any code examples

4. **Submit a Pull Request**
   ```bash
   git add .
   git commit -m "Add: Brief description of your contribution"
   git push origin feature/your-contribution-name
   ```
   Then open a Pull Request on GitHub.

---

## Contribution Guidelines

### General Principles
- Keep content **clear and accessible**
- Include **working code examples**
- Provide **context and rationale**
- Link to **relevant resources**
- Test all code before submitting

### File Organization
```
tutorials/
├── [platform]/
│   ├── README.md           # Overview and navigation
│   ├── getting-started.md  # Introduction tutorial
│   ├── [topic].md          # Specific tutorials
│   └── images/             # Tutorial images
```

### Naming Conventions
- Use lowercase with hyphens: `my-tutorial.md`
- Be descriptive but concise
- Use consistent naming across platforms

### Writing Style
- Use active voice
- Write for an international audience
- Define acronyms on first use
- Include prerequisites for each tutorial

---

## Tutorial Format

Use this template for new tutorials:

```markdown
# Tutorial Title

## Overview
Brief description of what this tutorial covers.

## Prerequisites
- Required software and versions
- Required knowledge or previous tutorials
- Required data (with download links)

## Learning Objectives
By the end of this tutorial, you will be able to:
- Objective 1
- Objective 2
- Objective 3

## Tutorial Content

### Step 1: Title
Explanation and code...

### Step 2: Title
Explanation and code...

## Common Issues
- Issue 1: Solution
- Issue 2: Solution

## Summary
Key takeaways from this tutorial.

## Next Steps
- Link to related tutorials
- Suggested further reading

## References
- Citation 1
- Citation 2
```

### Code Blocks

Always specify the language for syntax highlighting:

````markdown
```python
import scanpy as sc
adata = sc.read_h5ad("data.h5ad")
```

```r
library(Seurat)
obj <- readRDS("data.rds")
```
````

### Images
- Store in `images/` subdirectory
- Use descriptive filenames
- Include alt text for accessibility
- Keep file sizes reasonable (<1MB)

---

## Pull Request Process

1. **Title Format**: `[Platform] Brief description`
   - Example: `[Xenium] Add cell segmentation tutorial`

2. **Description Template**:
   ```markdown
   ## Summary
   What does this PR add/change?

   ## Type of Contribution
   - [ ] New tutorial
   - [ ] Update to existing content
   - [ ] Bug fix
   - [ ] Documentation improvement
   - [ ] Other (describe)

   ## Checklist
   - [ ] Follows style guidelines
   - [ ] Code has been tested
   - [ ] Links have been verified
   - [ ] Images are properly sized
   ```

3. **Review Process**:
   - A maintainer will review your PR
   - Address any feedback
   - Once approved, it will be merged

---

## Code of Conduct

All contributors must follow our [Code of Conduct](CODE_OF_CONDUCT.md). We are committed to providing a welcoming and inclusive environment.

---

## Questions?

- Open a [Discussion](../../discussions) for general questions
- Open an [Issue](../../issues) for bugs or specific problems
- Tag maintainers for urgent matters

---

Thank you for contributing to better spatial data analysis! 🔬✨

---
title: Best Practices
description: Recommended workflows and best practices for working effectively in the ADRF
order: 11
lastUpdated: 2026-03-31
---

# Best Practices

Following these best practices will help you work more efficiently in the ADRF and make your research more reproducible and maintainable.

> [!TIP]
> Check out the [Redshift Querying Guide](../advanced/redshift-querying-guide.md) for detailed instructions on how to how to access sensitive data stored in structured strorage in AWS Redshift.

## Key Principles

### Code Organization
- Structure your project logically
- Use meaningful file and folder names
- Keep related files together

### Documentation
- Comment your code clearly
- Maintain README files
- Document data sources and transformations

### Version Control
- Commit changes regularly
- Write descriptive commit messages
- Use branches for experimental work

### Reproducibility
- Make your analysis reproducible
- Document dependencies
- Use relative paths

### Storage Use
- **Avoid saving copies of raw data tables**. Instead, write code to **access data**. For detailed instructions on how to access data in structed data storage, please see the ADRF's [Redshift Querying Guide](../advanced/redshift-querying-guide.md)
- Organize folders in a way that makes sense for your particular project. For example, you might have folders for a particular analysis or sub-projects. Dates on file names can be helpful for version control.
- Keep tabs on how much storage you are using compared to the allocated amount of storage.

<!--

## Topics Covered

This section provides detailed guidance on:
- File and folder organization strategies
- Notebook documentation standards
- Code commenting best practices
- Version control workflows
- Collaboration guidelines

## Benefits

Following these practices will:
- Make your work easier to understand and maintain
- Facilitate collaboration with team members
- Speed up the export and disclosure review process
- Improve research reproducibility

-->


<br>

---
# Support & Navigation

**Need help?**
- Email: support@coleridgeinitiative.org
- Hours: Monday-Friday, 9 AM - 5 PM ET

**Navigation**
- ⬅️ [Back to Home](../README.md)
# Code Review Guidelines
This repository contains code guide lines helps you to understand what needs to follow.

## Pre-Pull Request Checklist: Streamline Your Code Reviews

This guide outlines essential pre-pull request (PR) checks to enhance code readability, maintain consistency, and expedite the review process. By following these practices, you'll contribute cleaner, more efficient code and reduce the need for extensive reviewer comments.

### I. Code Formatting and Readability

**Format Code Consistently:** Utilize the built-in formatting options in your **Visual Studio (VS) IDE**. 

For entire documents: ```Edit -> Advanced -> Format Document. For code selections: Edit -> Advanced -> Format Selection.```

**Code Cleanup:** Leverage automated code cleanup features (```Tools -> Options -> Text Editor -> Code Cleanup```). 
Customize or use the default settings to automatically format and remove unused elements (namespaces, etc.) upon saving.

### II. Code Quality and Maintainability

**Spell-check:** Double-check variable, method, and property names to ensure accuracy.
**Unused Variables/Objects:** Eliminate any references to variables or objects that are no longer required.
**Constructor Injection Order: **Maintain consistency in the order when injecting services into your constructor.

### III. Clear Code Comments and Documentation

**TODO Comments:** Use clear and concise //TODO comments to indicate areas requiring future attention. 
Follow a convention like ```// TODO: [PBI/Bug/Defect]#Number - Brief description of the change.```

**Complex Method Insights: **If a method is particularly intricate, consider adding summary comments that provide context for reviewers or even future reference by yourself.

### IV. Efficient Code Practices

**Minimize Hardcoded Values:** Avoid directly embedding hardcoded values within your code, especially if they recur across multiple locations. 
Instead, centralize such values in constants or enums for improved maintainability.

**Break Down Large PRs:** Refrain from submitting PRs encompassing massive amounts of logic. Smaller, focused PRs are easier to understand and review.

### V. Unit Testing

**Include Unit Tests: **Strive to add unit test methods along with your code, even if they haven't reached full functionality yet. This promotes a test-driven development (TDD) approach and facilitates future code maintenance.

### VI. Coding Conventions

**Naming Conventions: **Familiarize yourself and adhere to the established naming conventions for fields, properties, methods, and classes within your project.

### VII. Maintainable and Object-Oriented Code

**Parameter Reduction:** If a method accepts a large number of parameters, consider creating a model class to encapsulate those parameters and enhance code readability.

### VIII. Pre-Push Validation

**Clean and Build:** Clean your solution/project and ensure a successful build.
**Run Unit Tests:** Execute your unit test projects to verify that all existing and newly added tests pass successfully.
**Local Validation:** Thoroughly test your changes within your local environment.

#### **As a Reviewer, Consider:**

**Code Functionality:** Can the code effectively accomplish the intended task? Is it implemented in the optimal way, or could it benefit from refactoring?
**Impact Analysis:** Does this code modification potentially affect other parts of the codebase?
**Code Clarity:** Is the code easy to understand for reviewers and future developers?

By adopting these pre-PR checks, you'll significantly contribute to a clean, well-structured, and maintainable codebase, fostering a productive and collaborative development environment.

### Reference links:
[Code Review from NDC Conferences](https://www.youtube.com/watch?v=VuG4QhA89es&t=121s)

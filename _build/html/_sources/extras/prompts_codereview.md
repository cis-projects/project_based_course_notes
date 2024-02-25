# Reviewing Your Code

As part of enhancing your skills in software engineering, it's crucial to learn how to effectively review code. Not only does this practice help in identifying potential defects, but it also contributes to the overall quality of the software development process. In this guide, we introduce a structured approach to code review using ChatGPT, leveraging a research-informed prompt that focuses on various aspects of code quality.

## The Code Review Prompt

When requesting ChatGPT to review your software code, use the following structured prompt to guide the analysis. This prompt is designed to cover a comprehensive checklist that addresses common areas where defects may occur in software code. By following this prompt, you can ensure a thorough review that touches on critical components of code quality.

```markdown
Please evaluate the {code} below.
Use the following checklist to guide your analysis:
   1. Documentation Defects:
       a. Naming: Assess the quality of software element names.
       b. Comment: Analyze the quality and accuracy of code comments.
   2. Visual Representation Defects:
       a. Bracket Usage: Identify any issues with incorrect or missing brackets.
       b. Indentation: Check for incorrect indentation that affects readability.
       c. Long Line: Point out any long code statements that hinder readability.
   3. Structure Defects:
       a. Dead Code: Find any code statements that serve no meaningful purpose.
       b. Duplication: Identify duplicate code statements that can be refactored.
   4. New Functionality:
       a. Use Standard Method: Determine if a standardized approach should be used for single-purpose code statements.
   5. Resource Defects:
       a. Variable Initialization: Identify variables that are uninitialized or incorrectly initialized.
       b. Memory Management: Evaluate the program's memory usage and management.
   6. Check Defects:
       a. Check User Input: Analyze the validity of user input and its handling.
   7. Interface Defects:
       a. Parameter: Detect incorrect or missing parameters when calling functions or libraries.
   8. Logic Defects:
       a. Compute: Identify incorrect logic during system execution.
       b. Performance: Evaluate the efficiency of the algorithm used.
Provide your feedback in a numbered list for each category. At the end of your answer, summarize the recommended changes to improve the quality of the code provided.
```

## How to Use the Prompt

1. **Prepare Your Code**: Before using the prompt, ensure your code is ready for review. This might involve commenting your code adequately and ensuring it's in a format that ChatGPT can understand.
   
2. **Customise the Prompt**: Replace `{code}` with the actual code you wish to review. If the code is lengthy, consider breaking it down into smaller segments to focus on specific parts of the code for each review session.

3. **Analyse ChatGPT's Feedback**: Once you receive the analysis, go through each point carefully. ChatGPT will categorise its feedback based on the checklist provided in the prompt, making it easier to identify areas for improvement. **Remember, do not accept received feedback as correct. Carefully criticise and reflect on received feeback**.

4. **Implement Recommendations That Makes Sense for You**: Use ChatGPT's feedback to make informed decisions on improving your code. **Ideally, you and your team review received feedback together**. You are in control of these decisions. This might involve refactoring parts of the code, improving documentation, or optimising logic and performance. Or, this might also include that you ignore received feedback (in case it's not correct or appropriate).

5. **Iterate**: Code review is an iterative process. You may wish to refine your code based on feedback and run it through the review process again to ensure all potential issues are addressed.


## How to Run an Automated Code Review Using Generative AI?

Below are links to some our recently developed GenAI-powered Code Review Scripts (GitHub Action):

- **ChatGPT Pull Request Review Action**: [https://github.com/agogear/chatgpt-pr-review/](https://github.com/agogear/chatgpt-pr-review/)
  - A GitHub Action that helps you with code reviews.
- **AI-powered peer review process: An approach to enhance computer science students’ engagement with code review in industry-based subjects (2023 ASCILITE Paper)**: [https://publications.ascilite.org/index.php/APUB/article/download/482/557/](https://publications.ascilite.org/index.php/APUB/article/download/482/557/)


## Conclusion

Utilising ChatGPT for code review with this structured approach can significantly enhance the quality of your software projects. By systematically addressing each category in the checklist, you can identify and rectify common defects, leading to more robust, efficient, and maintainable code.

Remember, the goal of this exercise is not only to improve the specific piece of code under review but also to cultivate a mindset of continuous improvement and attention to detail that is essential in software engineering.
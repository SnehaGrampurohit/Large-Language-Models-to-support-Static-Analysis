# Large-Language-Models-to-support-Static-Analysis

Static analysis is a fundamental technique in software engineering, used to analyse source code without executing it. It helps identify potential defects, security vulnerabilities, and design issues in software systems. This process typically relies on examining the code's structure and interactions to predict and prevent issues during development. Large language models, such as GPT-3.5, are advanced artificial intelligence systems that have shown remarkable abilities in natural language understanding and generation. These models have the potential to transform various fields, including static analysis. Currently, the field of static analysis faces several challenges. Traditional static analysis tools  often struggle with complex codebases and languages, producing high rates of false positives and negatives. This can hinder the efficiency and effectiveness of the analysis process. Moreover, keeping these tools up to date with ever-evolving programming languages and frameworks is a daunting task. Using large language models to support static analysis can revolutionise this landscape. These models can enhance the accuracy of defect detection and code comprehension. They can assist developers in understanding code written in different programming languages, recognising common coding patterns, and identifying potential vulnerabilities more effectively. Furthermore, large language models can also aid in code summarisation, documentation generation, and refactoring suggestions, ultimately improving the overall software development process. The integration of these models into static analysis tools has the potential to mitigate the challenges faced by developers and researchers alike.

A software vulnerability scanner checks for SQL Injections in a project and exports the result to a Static Analysis Results Interchange Format (SARIF) file
- understand and query the results reported by the static analysis tool with the aid of a chatbot

example :
Dialog 1
Human: How many vulnerabilities are in my project?
Bot: Provides the number and type of vulnerabilities in the SARIF file

Dialog 2
Human: Is there a vulnerability in the <<classname>> class? (user provides the name of a class, for example, SqlInjectionLesson10)
Bot: Gives the location of the vulnerability and uses the text from the message (see SARIF file) to provide more details about the vulnerability

Task #1: ChatBot
For this task, use a chatbot library of your choice, for example, AIML (Java), ChatterBot (Python), or other
libraries to create a chatbot that allows users to ask the questions in the section above. The Chatbot
should provide answers to the questions using the information described in Task #2.

Task #2: Static Analysis Results Processing
The SARIF file provided is the output from a taint analysis tool called SecuCheck. The results in the SARIF
file are CWE89 SQL Injection vulnerabilities detected in the Webgoat project. Perform the following two
tasks in a Java or Python project:

- Implement a solution to parse the SARIF file.
- Implement queries that can obtain the information needed to respond to the user’s questions (the number and type of vulnerabilities, as well as whether a vulnerability is in a specific class)
- Integrate the chatbot with the queries used to process the SARIF file, such that a user can
- Type the question and get the correct answers.

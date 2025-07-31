# Guidelines for Data Storytelling Lab Workshops
#### Authored by: John Lauermann, School of Information, Pratt Institute
#### Last updated: July 2025

Thank you for agreeing to lead a workshop -- and develop a tutorial -- for the Data Storytelling Lab! This repository provides a basic template for use when preparing your workshop materials. 




## The basic structure
While the specific content and organization is entirely up to you, we as that your tutorial repository include some standard elements. These elements support replicability for faculty who may want to teach with your materials, and facilitate learning comprehension for students who may be exploring on their own. 

Each repository should include:
- a `readme.md` file that identifies learning outcomes and explains the structure of the workshop
- one or more code templates, written with literate programming best practices and annotated for step-by-step explanation
- replication data if relevant
- information on reproducibility



## readme
The markdown document will be the first document that a user reads when encountering your tutorial. Thus it needs to perform several kinds of interpretive work for explaining what the tutorial does, how to replicate the process, and why the tools used are relevant and useful. 

Relevant content might include: 
- an abstract that explains the overall purpose of the workshop and summarizes the most important skills a student will learn
- one or more student learning outcomes, achievable in the context of a 90 minute workshop
- a clear statement on how to replicate the workflow
- a bibliography of relevant resources for further learning

Potentially useful reading:

Cone, M (2025) "Basic Syntax for Markdown", _The Markdown Guide_, https://www.markdownguide.org/basic-syntax/

Pratt Institute Center for Teaching and Learning, "Lesson Planning Frameworks", _The Art and Architecture of Teaching and Learning: A Course Design Resource Hub_, https://prattctl.org/course-design/



## Code templates
The specific structure and content of your code templates will of course vary based on the languages used and the nature of the workflow. But please be sure to integrate literate programming and data science pedagogy best practices throughout. Those best practices include:
- Clearly indicate the order in which a student should proceed, for example by numbering files sequentially
- Use descriptive and easy-to-understand names for folders, files, functions, and variables
- Annotate each section of the code to explain what is happening and how it fits within the workflow
- Explain common shorthand that you may know but a student might not (e.g., `df` usually means data frame, `pd` is a common alias for `pandas`)

Potentially useful reading: 

[Candela, G. et al. (2023). An approach to assess the quality of Jupyter projects published by GLAM institutions. Journal of the Association for Information Science and Technology, 74(13), 1550–1564.](https://drive.google.com/file/d/1HB40Aga9brU7U5nJS1EBwwfIWBYooMOX/view?usp=sharing)

[Trisovic, Ana, et al. (2022) A large-scale study on research code quality and execution. Scientific Data 9: 60](https://drive.google.com/file/d/137ig_nDWtXIVwsFRoDvxZgDV1TV8oAXf/view?usp=sharing)



## Replication materials
Your repository should include all necessary information for a student to reproduce the workflow. This could mean including a folder with relevant replication data. Or it could mean providing other clear guildeines for accessing data, such as using API calls to ingest data directly into a code template. However you decide to structure this, please keep in mind the following best practices:
- Include a 'how to replicate this' paragraph somewhere in the repostitory, for example in the `readme.md`
- Use APIs when relevant to reduce the raw data needing storage. If you do, please be sure to clearly explain how to use the API in the code template (including where to obtain keys or tokens, and how to configure and customize the query)
- Use relative path structures and project-oriented workflows whenever possible (e.g., building relative paths with 'here' in R, rather than less replicable tools like `setwd()`
- Include documentation on versions and dependencies. For example, this could mean adding a `requirements.txt` file for Python workflows, or adding relevant installations into an R script such as ``` if (!require(dplyr)) install.packages("dplyr") ```
  

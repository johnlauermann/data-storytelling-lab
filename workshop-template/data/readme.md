# Ideas for replication materials

Your repository should include relevant information for a student to reproduce the workflow. This could mean including a folder with relevant replication data. Or it could mean providing other clear guildeines for accessing data, such as using API calls to ingest data directly into a code template. However you decide to structure this, please keep in mind the following best practices:
- Include a 'how to replicate this' paragraph somewhere in the repostitory, for example in the `readme.md`
- Use APIs when relevant to reduce the raw data needing organization and storage. Please be sure to clearly explain how to use the API in the code template (including how to obtain keys, and how to configure the query)
- Use relative path structures and project-oriented workflows when possible (e.g., building relative paths with 'here' in R, rather than less replicable tools like `setwd()`
- Include documentation on versions and dependencies. For example, this could mean adding a `requirements.txt` file for Python workflows, or adding relevant installations into an R script such as
 ```console
 if (!require(dplyr)) install.packages("dplyr")
```

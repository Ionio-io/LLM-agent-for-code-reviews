# LLM agent for code review automation using crewAI

An autonomous agent created using [crewAI](https://www.crewai.io/) and [Langchain](https://www.langchain.com/) to automate your code review workflow

### [Read the blog!](https://www.ionio.ai/blog/how-to-build-llm-agent-to-automate-your-code-review-workflow-using-crewai)

## 👀 Sneak peek

<div style="position: relative; padding-bottom: 56.25%; height: 0;"><iframe src="https://www.loom.com/embed/3d31233572f04c2fac1478df9475ca28?sid=0fd4251f-49fa-4bce-b3d8-57db44180a0a" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

## 🤔 How it works?

### 1. Get the Tree Structure of Repo

The agent will first get the tree structure of given github repository and then for every file, it will create full paths for that file from tree structure

### 2. Get the File Content

From the given file path, it will then use github API to get the file content

### 3. Review the File

Once it gets the file content, it will review the given file and make changes in code if needed.

### 4. Add the Review in Notion Document

The review will be added in notion document using notion API client.

## ⚒️ Architecture

![](https://assets-global.website-files.com/62528d398a42420e66390ef9/65e82541a4d0a90120a3bfc6_image5.png)

## 🚀 Getting started

### Prerequisites

- Python and anaconda installed on your machine
- OpenAI api key
- Github Personal Access Token (PAT)
- Notion api key

### How to run?

- Clone the repository
- Create a file called `constants.py` in same folder and store all of your api keys like this

```
OPENAI_API_KEY = <key_here>
GITHUB_SECRET_KEY = <key_here>
NOTION_API_KEY = <key_here>
```

- Open any jupyter notebook from repository and import the `constants.py` file in it
- Select your existing python environment or create one using anaconda
- Run the code

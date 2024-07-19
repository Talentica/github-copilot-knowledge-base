# GitHub Copilot VS Code Settings

## Installation
- Install Visual Studio Code (VS Code) from the official website.
- Install the GitHub Copilot and Copilot Chat extension from the VS Code marketplace.
  	- Link : (https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)
    - Reference : (https://www.geeksforgeeks.org/how-to-install-github-copilot-on-vscode/)
- Sign in with your GitHub account and enable Copilot in your editor.


## Basic Usage
-	Open a new or existing file in VS Code.
-	Start typing your code or a comment describing what you want to achieve.
-	GitHub Copilot will suggest code snippets based on your input.
-	Press Tab to accept a suggestion or Esc to dismiss it.

## More features of copilot extension:
To get the most out of GitHub Copilot, it's important to understand how to leverage its capabilities effectively. Here are some strategies:

### Copilot extension options:
Select code snippet, right click and take appropriate action from copilot extension options.
Actions like Explain code, Generate UT, etc can be taken.

### Use Slash Commands

To perform any copilot operation on a single or multiple lines, first select the lines and click on the yellow bulb and perform your desired operation.

- Open inline chat
![4b74b77c-a3a7-4db9-9d9c-b7b631740644](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/bd5c3d4b-e2ac-4966-bc3f-0ae09d107a92)

- Open Copilot chat to explain a code file
![0fcd61d7-9ea5-4334-8b2f-1788d856aa8c](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/ddd7b539-9d82-4b0d-8f9b-dcb4d93f54e5)

- Open Copilot chat to fix a selected code
![99f09a99-61f2-47f1-95e5-999e64b79546](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/29ae6d45-b962-4f6e-a3d3-355740b4ad0f)

![image](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/de094908-4a79-4dde-85d3-b87871a35852)

### To ignore secret files from copilot use below settings.
.vscode/settings.json add below config.

```
  "files.associations": {
    ".env*": "dotenv"
  },
  "github.copilot.enable": {
    "*": true,
    "dotenv": false
  }
```
  

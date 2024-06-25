# Contributing to ZHCET Code Oasis

Thank you for considering contributing to our projects! We appreciate your efforts and want to make the contribution process smooth and effective for everyone involved. Here are our contribution guidelines.

## Reporting Issues

All issues should be reported according to the issue templates provided in the `ISSUE_TEMPLATE` folder. This helps us understand the context and severity of the issue quickly and ensures we can address it appropriately.

---

## Workflow for Contributing

1. **Clone the Project**:
    ```bash
    git clone https://github.com/your-repo/project.git
    cd project
    ```

2. **Set Upstream for Main/Master**:
    ```bash
    git remote add upstream https://github.com/original-repo/project.git
    ```

3. **Sync Your Fork**:
    - Before working on any new feature, ensure your master branch is up-to-date with the upstream master.
    ```bash
    git pull upstream master
    ```

4. **Create a New Branch**:
    - Branch names should follow the format `feat/<feature>/<sub_feature>`, `fix/...`, `refactor/...`, or `init/...`.
    ```bash
    git checkout -b feat/new-feature/sub-feature
    ```

5. **Make Your Changes**:
    - Make the necessary code changes and commits.

6. **Push to Your Fork**:
    ```bash
    git push origin feat/new-feature/sub-feature
    ```

7. **Open a Pull Request**:
    - Navigate to the original repository and open a pull request to the master branch of the project repository.

---

## Writing Commit Messages

Clear, concise commit messages are crucial for maintaining a readable project history.
Use the following format for commit messages:
```
feat(<feature>) : <Changes_description>
```

### Follow this format
**Type** | **Description** |
--- | --- |
feat | Use for new features |
fix  | Use for bug fixes |
refactor | Use for refactoring changes |
init | Use for initial changes or new environments |

#### Example Commit Messages:
* feat(user-auth): add JWT authentication
* fix(api): resolve data fetch issue
* refactor(utils): optimize calculation functions

--- 

## Writing a Pull Request (PR)

When writing a PR, ensure it is clear and follows the PR template provided in PULL_REQUEST_TEMPLATE.md. 
### Here’s the format to follow:
* Describe the PR: Provide a detailed description of the PR and the problem it solves.
* Changes Made: Describe the changes made in this PR.
* How to Test: Include steps on how to test the changes.
* Relevant Issues/PRs: Reference any related issues or PRs.
* Screenshots: Add any relevant screenshots to demonstrate the changes.

#### Example PR
```
## Describe the PR
This PR adds JWT authentication to enhance the security of user sessions. This involves creating new middleware and updating the login route.

## Changes Made
- Implemented JWT authentication for user login.

## How to Test
1. Pull the latest changes.
2. Run the application.
3. Use Postman to test the login route with valid credentials.
4. Check for the JWT token in the response.

## Relevant Issues/PRs
- Fixes #123

## Screenshots
![JWT Authentication](path/to/screenshot.png)
```
--- 
# KODEGO GitHub Demo Day 6 (06/17/23)
## Contents

[Prerequisite](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#prerequisite)

[Git VS GitHub](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#git-vs-github)

[HTTP vs SSH](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#http-vs-ssh)

[Local Repository VS Cloud Repository](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#local-repository-vs-cloud-repository)

[When to use Git Init and Git Clone](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#when-to-use-git-init-and-git-clone)

[Common Git Command](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#common-git-command)

[Personal Access Token](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#personal-access-token)

[Getting Started](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#getting-started)

[Pushing Code to a Git Repository](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#pushing-code-to-a-git-repository)

[Documentation](https://github.com/HexeCalibre/my-test-repo/blob/master/README.MD#documentation)

## Prerequisite
Install Git(Powershell) or Git Bash(Linux)

[Git](https://git-scm.com/)

Git Bash
```bash
sudo apt install git
```

[Learn more about Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)

[Create Github Account](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home)

[Learn more about Singing up](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account)

## Git VS GitHub

Git and GitHub are two closely related but distinct tools used in software development for version control and collaboration. While they are often used together, it's important to understand the differences between them.

**Git** is a distributed version control system designed to track changes in source code during software development. It allows developers to create branches, make changes, and merge those changes back into the main codebase. Git provides a command-line interface and a set of commands that enable efficient version control, including creating repositories, committing changes, and resolving conflicts.

**GitHub** is a web-based platform that provides hosting services for Git repositories. It adds a layer of functionality on top of Git, making it easier to collaborate with others and manage projects. GitHub offers a graphical user interface (GUI) that simplifies tasks like creating and managing repositories, visualizing code history, and facilitating collaboration through features like pull requests and code reviews.

In summary, Git is the underlying technology that handles version control, while GitHub is a platform built around Git that provides additional features and a user-friendly interface.

[Learn more about GitHub](https://docs.github.com/en/get-started/quickstart/hello-world)

## HTTP vs SSH

When it comes to interacting with remote repositories, Git offers two primary protocols: HTTP and SSH.

- **HTTP**: This protocol allows read and write access to the remote repository, but it requires authentication for write access. It is relatively easier to set up and use, making it suitable for public repositories or scenarios where write access is not required.

- **SSH**: This protocol provides secure access to the remote repository using SSH keys for authentication. It allows both read and write access to the repository and is commonly used in situations where secure access is necessary, such as private repositories.

[Learn more about Authenticating with GitHub from Git](https://docs.github.com/en/get-started/quickstart/set-up-git#authenticating-with-github-from-git)

## Local Repository VS Cloud Repository

When working with version control systems like Git, you have the option to use either a local repository or a cloud repository. Here's a breakdown of the key differences:

**Local Repository:**
- A local repository is stored on your local machine or a local server.
- It resides within your local file system and is not accessible to others unless explicitly shared.
- You have full control over the repository and can perform all Git operations locally.
- Local repositories are typically used for individual development or small team collaborations where all members have direct access to the same file system.

**Cloud Repository:**
- A cloud repository is hosted on a remote server, usually provided by a platform like GitHub, GitLab, or Bitbucket.
- It is accessible over the internet, allowing multiple users to collaborate on the same repository simultaneously.
- Cloud repositories provide additional features like issue tracking, pull requests, and team collaboration tools.
- They offer remote backups and easy sharing of code with others.
- Cloud repositories are commonly used for open-source projects, large team collaborations, and remote development workflows.

In summary, while a local repository provides direct control and privacy, a cloud repository offers collaboration features, accessibility, and remote backups. The choice between the two depends on the nature of the project, team size, and preferred workflow.

[Learn more about Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories)

## When to use Git Init and Git Clone
Both `git init` and `git clone` are important Git commands, but they are used in different scenarios:

- `git init`: This command is used when you want to initialize a new Git repository in an existing local directory. It is typically used when you want to start tracking changes in a project from scratch.

[Learn more about git init](https://git-scm.com/docs/git-init)

- `git clone`: This command is used when you want to create a local copy of an existing remote repository. It is commonly used when you want to collaborate on an existing project or when you want to work with a codebase that is already hosted on a remote Git repository.
  
[Learn more about Cloning Repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

## Common Git Command
| Git Command | Function |
| --- | --- |
| `git init` | Initializes a new Git repository |
| `git clone` | Creates a local copy of a remote repository |
| `git add [file]` | Adds a specific file to the staging area |
| `git add .` | Adds all modified and new files to the staging area |
| `git commit -m "Commit message"` | Records changes to the local repository |
| `git status` | Displays the current state of the repository |
| `git branch` | Lists all branches in the repository |
| `git checkout [branch_name]` | Switches to a different branch |
| `git merge [branch_name]` | Combines changes from one branch into the current branch |
| `git pull` | Fetches and merges changes from a remote repository to the current branch |
| `git push` | Pushes changes from the local repository to a remote repository |

[Learn more about Git Commands](https://git-scm.com/docs)

## Authentication
### Personal Access Token

A Personal Access Token (PAT) is a security mechanism used for authentication in Git. It serves as an alternative to passwords when accessing Git repositories, providing an additional layer of security.
#### How to Generate PAT

To generate a Personal Access Token, follow these steps:

1. Go to your Git provider's settings or account settings page.
2. Look for the section related to Personal Access Tokens.
3. Generate a new token and provide a name for identification.
4. Select the desired scopes or permissions for the token.
5. Generate the token and make sure to save it securely.

[Learn more about PAT](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

### SSH Key
#### What is an SSH Key?

SSH keys are a pair of cryptographic keys used for secure communication and authentication between a client and a server. The key pair consists of a private key and a public key.

#### Why Use SSH Keys?

- Enhanced Security: SSH keys provide stronger security than passwords, eliminating the risk of password-based attacks.
- Convenience: SSH keys allow for passwordless authentication, saving time and facilitating automation.
- Simplified Authentication: Configure the public key on the server once, and any device with the private key can authenticate.
- Scalability: Use the same SSH key pair across multiple machines, simplifying key management.

#### Generating SSH Keys

1. Open a terminal or command prompt.
2. Execute the following command to generate the key pair:

   ```shell
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   //Replace "your_email@example.com" with your actual email address.
   ```

#### Using SSH Keys

1. Copy the public key (id_rsa.pub) to the remote server's ~/.ssh/authorized_keys file.

2. Connect to the remote server using SSH by executing the following command:
   
```bash
ssh username@server_ip
//Replace username with your username on the remote server and server_ip with the IP address or domain name of the server.
```

3. Enter the passphrase if applicable.

SSH keys provide secure and convenient authentication for remote servers. Handle your private key with care, regularly update and rotate your keys for better security.

Remember to refer to additional resources and SSH documentation for advanced configurations and use cases.

[Learn more about SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
## Getting Started
### How to Setup Using `git config`

The `gitconfig` command is used to configure Git settings on your local machine. It allows you to set various options such as your name, email, and preferred text editor.

To configure Git settings on your local machine using `git config`, follow these steps:

1. Open a terminal or command prompt.
2. Set your name by executing the following command:

```bash
git config --global user.name "Your Name"
//Replace "Your Name" with your actual name.
```

3. Set your email address by executing the following command:

```bash
git config --global user.email "your.email@example.com"
//Replace "your.email@example.com" with your actual email address.
```

4. Set your preferred text editor by executing the following command:

```bash
git config --global core.editor "your-editor"
Replace "your-editor" with the name of your preferred text editor (e.g., "vim", "nano", "code").
```

5. (Optional) Set other configurations such as aliases, colors, or default branch names according to your preference.

These configurations will be applied globally, meaning they will be used for all your Git repositories on the local machine.

Feel free to explore the Git documentation and additional resources for more information on `git config` and its various options.

[Learn more about Git Config](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
### Setup Remote

To set up a remote repository in Git, you can use the following commands:

```shell
git remote add [remote_name] [repository_url]  # Links your local repository to a remote repository
git remote remove [remote_name]               # Removes the specified remote repository
git remote -v
```
## Pushing Code to a Git Repository

To push your code changes to a Git repository, follow these steps:

1. Stage your changes by adding them to the staging area using the command:
```bash
   git add .
   //This command adds all modified and new files to the staging area.
```

2. Commit your changes with a descriptive commit message using the command:
```bash
git commit -m "Your commit message"
//Replace "Your commit message" with a brief and meaningful description of the changes you made.
```

3. Push your changes to the remote repository using the command:
```bash
git push <remote> <branch>
//Replace <remote> with the name of the remote repository you want to push to, and <branch> with the branch name you want to push.
```
Example:
```bash
git push origin main
or
git push origin master
//This command pushes your committed changes to the remote repository named "origin" in the "main" or "master" branch
//Note: Always check the branch name first.
```
4. Enter your authentication credentials if prompted.
5. Wait for the push to complete. Once finished, your code changes will be available in the remote repository.

Make sure you have the necessary permissions and the correct remote repository URL configured.

Remember to pull any changes from the remote repository before pushing to avoid conflicts.

Feel free to explore the Git documentation and additional resources for more advanced usage and Git workflows.

[Learn more about git remote](https://git-scm.com/docs/git-remote)

## Conflict in GitHub

When collaborating with others on a project using GitHub, conflicts can occur when multiple people make changes to the same file or code at the same time. A conflict happens when Git is unable to automatically merge the changes and requires manual intervention to resolve the differences.

### Identifying a Conflict

Conflicts are typically identified when you attempt to merge or pull changes from a remote repository into your local repository. Git will notify you if there are conflicts and provide information about the affected files.

### Resolving a Conflict

To resolve a conflict in GitHub, follow these steps:

1. **Pull the Latest Changes**: Before resolving conflicts, make sure you have the latest changes from the remote repository. Use the command `git pull origin branch-name` to fetch and merge the changes.

2. **Identify the Conflicting Files**: Git will highlight the conflicting files and mark the conflicting lines within those files. Open the conflicted file(s) in a text editor or an integrated development environment (IDE).

3. **Locate and Edit the Conflict**: Inside the conflicted file, Git will mark the conflicting lines with special characters like `<<<<<<<`, `=======`, and `>>>>>>>`. These markers separate the conflicting changes made by different contributors.

4. **Resolve the Conflict**: Review the conflicting changes and decide which changes to keep or modify. Remove the conflict markers and edit the code to create a resolution that integrates both sets of changes appropriately.

5. **Save and Commit the Changes**: Once you've resolved the conflict, save the file and stage it for commit using the command `git add path/to/file`. Repeat this step for all conflicted files.

6. **Commit the Changes**: Finally, create a new commit with a meaningful message to document the conflict resolution. Use the command `git commit -m "Resolved conflict in file-name"`.

7. **Push the Changes**: After committing the changes, push the resolved conflict to the remote repository using `git push origin branch-name`.

## Communication and Collaboration

It's essential to communicate with other contributors involved in the conflict to ensure a smooth resolution. Discussing the changes and reaching a consensus can help prevent future conflicts and improve collaboration.

By following these steps and maintaining effective communication, you can successfully resolve conflicts in GitHub and ensure the integrity of your collaborative project.

## Documentation
### What is Documentation?

Documentation refers to the process of capturing and recording information about a software project, system, or process. It involves creating written, visual, or interactive materials that provide details and instructions on how to understand, use, maintain, and troubleshoot the software or system.

Documentation can include various artifacts such as:

- **User Manuals:** Guides that help end-users understand and use the software effectively.
- **Technical Guides:** Detailed instructions and explanations for developers and system administrators.
- **API Documentation:** Documentation specifically for application programming interfaces (APIs), providing information on how to interact with the software components.
- **Code Comments:** In-line comments within the source code, explaining the purpose and functionality of different code sections.
- **Tutorials and Examples:** Step-by-step instructions and code samples to help users learn and implement specific functionalities.
- **Troubleshooting Guides:** Documentation that assists in identifying and resolving common issues and errors.

### Why is Documentation Important?

Documentation plays a crucial role in software development and maintenance for the following reasons:

1. **Knowledge Transfer:** Documentation ensures that knowledge about the software or system is preserved and can be shared with others, such as new team members or stakeholders. It helps onboard new developers, reduces dependencies on specific individuals, and facilitates collaboration.

2. **Improved Usability:** Well-documented software is easier to understand and use. Users can refer to documentation to learn how to interact with the software, reducing the learning curve and improving user experience.

3. **Maintenance and Troubleshooting:** Documentation provides insights into the inner workings of the software, making it easier to maintain, debug, and troubleshoot issues. It helps developers understand the system's architecture, dependencies, and expected behavior.

4. **Consistency and Standardization:** Documentation promotes consistency and standardization in code, processes, and practices. It establishes guidelines and best practices that enable teams to work cohesively and maintain a high level of quality.

5. **Support and Collaboration:** Documentation facilitates support by providing resources for users and developers to find solutions to common problems. It encourages collaboration by providing a central reference for all team members to understand the software and work together effectively.

By investing time and effort into creating comprehensive and up-to-date documentation, software projects can become more accessible, maintainable, and scalable.

Remember, good documentation is concise, clear, organized, and regularly updated to reflect changes in the software or system.


[README Template](https://gist.github.com/DomPizzie/7a5ff55ffa9081f2de27c315f5018afc)

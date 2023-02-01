# GitHub Repository Standard :chicken:

Welcome to the GitHub Repository Standard repo. In this repo, you will be guided through how each repository should be set up, how to track progress, assiging roles, and all the other necessary coverage of project management.

TLDR: Skip ahead to the Setting Up A Project to get started.

TLDR P2: If you'd like, you can clone this repo and start using it out of the box to setup your project. While this is a quick method, it is recommended that your read the rest of this so that all standards are followed.

# Goals :soccer:

The following criteria must be described in each project README.md file in the root of the repository: 

- Define clear project goals and objectives.
- Use a branching strategy for version control.
- CI/CD through GitHub actions (if used)
  - Describe where configuration files are, how they are to be used, etc
- Describe contribution details (ex. is a pull requests needed? Do contributors need to create code on a different branch? Do developers need to fork the repo?)

The responsibility of the repo owner is the following tasks:

- Establish Milestones for each project
  - Milestones can be created in any GitHub project. They can be created and found under:
    - Pull Requests > Milestones
  - Under each milestone, a set of issues will be created before hand
  - When issues are closed, progress can be tracked through GitHub's burndown chart
  - Admins of the repo can assign each issue related to each milestone to a developer within the organization
- Assign clear roles and responsibilities to team members.
  - Similiarly to before, those managing the milestone of a project will assign developers to each issue in each milestone.
- Document all code, processes, and decisions.
  - Documentation of code should be followed under respective linting standards. For a Python3 project for example, the user could use Pylint to lint their code, which forces users to document each function they create which describes the parameters of a function, what the function returns, how it works, etc. All code written should be easy to understand, and well documented. Any documentation that pertains to the project that must be kept in a seperate folder can be placed in:
    - project root > documentation
- Testing
  - Software must be properly tested before pushed, but code is safe guarded by CI/CD which allows for mistakes. To ensure that the code passes the proper tests, lint code and run test cases on code before pushing. 
- Use pull requests for code review and collaboration.
  - Admins of each repository must ensure that pull requests are reviewed before merge to the main branch.
- Regularly merge code and maintain a clean repository.
- Track and manage issues and project milestones.
- Use project boards and agile methodologies as necessary.
- Keep all team members informed and up to date.


# Naming convention :pencil:

All repositories should follow **PascalCase** naming convention. For example, if your project relates to an Ethiopia dashboard, the repository name should be "EthiopiaDashboard". In case of acronyms or third-party standards that cannot be avoided, the acronym should still be in uppercase while following the PascalCase naming convention. For example, if the repository contains the acronym "TEV", the name should be "TEVDashboard".

# Setting Up A Project :star:

To start, clone this repo and begin to edit the following files:

- .gitignore
  - Typical files to be include in a .gitignore are ones that are unnecessary for the project, and allow the repo size to become reduced. Here are a few examples:
    - .DS_Store
    - node_modules
    - __pycache__  
<br/>
- .github/workflows
  - This is where all GitHub workflows are found and where CI/CD can be specified. The following workflows must be created:
    - Linting process
      - Cleans up your code
    - Testing process
      - Tests your code
  - If either of these are not passed on push, then the build will fail. Progress of a pushed workflow can be tracked at:
    - Actions > All Workflows
<br/>
  
- README.md
  - Your README.md file should specify everything mentioned in the Goals section.


# Project Management Structure :building:

All tasks should be managed under a milestone. To create these tasks, an issue must be created, and then placed into the milestone. Once the issue is created, 




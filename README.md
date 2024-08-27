# greenwood-library-website
This project focused on improving the current Greenwood Community Library website by incorporating a "Book Reviews" section and updating the "Events" page to captured forthcoming events. The project emulated a collaborative effort between two developers, Morgan and Jamie, who each played distinct roles in various components of the project.

## Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Setup Instructions](#setup-instructions)
- [Branch Workflow](#branch-workflow)
  - [Morgan's Contribution: Adding Book Reviews](#morgans-contribution-adding-book-reviews)
  - [Jamie's Contribution: Updating Events Page](#jamies-contribution-updating-events-page)
- [Testing and Validation](#testing-and-validation)
- [Contributor Guidelines](#contributor-guidelines)
- [Final Outcome](#final-outcome)

## Project Overview

The Greenwood Community Library website originally featured fundamental sections such as Home, About Us, Events, and Contact Us. The objective of this project was to:

- Add a "Book Reviews" section to the website.
- Update the "Events" page with new community events.

The project replicated the cooperative efforts of two contributors utilizing Git and GitHub to efficiently manage modifications and integrate them.

## Objectives

- Practice cloning a repository and working with branches in Git.
- Gain experience in staging, committing, and pushing changes from multiple developers.
- Create pull requests and merge them after resolving any potential conflicts.

## Setup Instructions

1. **Create a Repository on GitHub:**
   - Repository Name: `greenwood-library-website`
   - Initialized with a `README.md` file.
   ![Setup github repo](./img/01.png)

   - Clone the repository to your local machine using:

     Copy the repo http link
    ![copy repo http link](./img/02.png)
   ```bash
     git clone https://github.com/kanmyng/greenwood-library-website.git
     ```

    - Open `Git Bash`, navigate to the desire directory created and clone the remote repo to your local system.
    ![clone repo to local machine](./img/03.png).

    - Navigate to the directory
    ![confirmation and navigate to the directory](./img/04.png)

2. **Initial Setup:**
   - On the `main` branch, create the following files using a code editor such as Visual Studio Code:
     - `home.html`
     - `about_us.html`
     - `events.html`
     - `contact_us.html`

     To open the project in Visual Studio editor, type `code .` in the Git Bash. This will automatically open the project in VS Code editor.
     ![open project in VS Code editor](./img/05.png)

     Project opened in VS Code editor
     ![Project display in VS Code editor](./img/06.png)
    
    - Creation of files in the main branch
    ![creation of files in the main branch](./img/07.png)

   - Add some placeholder content to each of these files.

   - `Home.html` content
   ![Add content to home.html](./img/08.png)

    - `About_us.html` content
   ![Add content to about_us.html](./img/09.png)

   - `Event.html` content
   ![Add content to event.html](./img/10.png)

   - Contact_us.html` content
   ![Add content to contact_us.html](./img/11.png)

   - Stage, commit, and push these changes to the `main` branch:
     ```bash
     git add .
     git commit -m "Initial setup with basic web pages"
     git push origin main
     ```

    - Staging and committing files, and pushing to main the main branch
   ![Stage, commit, and push changes](./img/12.png)

## Branch Workflow

### Morgan's Contribution: Adding Book Reviews

1. **Create a Branch for Morgan:**
   - Create and switch to a new branch named `add-book-reviews`:

        ```bash
     git checkout -b add-book-reviews
     ```
      ![creating and switching to add-book-reviews](./img/13.png)

2. **Add Book Reviews Section:**
   - Create a new file `book_reviews.html` for the "Book Reviews" section.
    ![creat book_reviews.html file](./img/14.png)

   - Add some placeholder text to the file.
    ![add content to book_reviews.html file](./img/15.png)

   - Stage, commit, and push the changes to GitHub:

     ```bash
     git add book_reviews.html
     git commit -m "Add book reviews section"
     git push origin add-book-reviews
     ```

     ![Stage, commit, and push](./img/16.png)

3. **Create Pull Request:**
   - On GitHub, create a Pull Request (PR) from the `add-book-reviews` branch to the `main` branch.
   ![Compare and pull request](./img/17.png)

   - Create PR
   ![create PR](./img/18.png)

4. **Merge Morgan's Work:**
   - Review and merge the PR into the `main` branch.
  ![review and merge PR to main branch](./img/19.png)

### Jamie's Contribution: Updating Events Page

1. **Create a Branch for Jamie:**
   - Create and switch to a new branch named `update-events`:

     ```bash
     git checkout -b update-events
     ```

       ![creating and switching to update-events](./img/20.png)

2. **Update Events Page:**
   - Update the `events.html` file with new community events.
      ![Jamie updating events.html](./img/21.png)

   - Stage, commit, and push the changes to GitHub:
     ```bash
     git add events.html
     git commit -m "Update events page with new community events"
     git push origin update-events
     ```
     ![Stage, commit, and push](./img/22.png)

3. **Pull Latest Changes:**
   - Before raising a PR, pull the latest changes from the `main` branch:

     ![Compare and pull request](./img/23.png)

    - Create PR
      ![create PR](./img/24.png)
      review and merge PR to main branch
      ![review and merge PR to main branch](./img/25.png)

     ```bash
     git checkout main
     git pull origin main
     git checkout update-events
     git merge main
     ```
    - Switch to main branch, pull origin main. Switch to update-events and merge to main
     ![review and merge PR to main branch](./img/26.png)

  ### Resolve any conflicts if necessary and then create a PR:
    - Resolve Conflicts: Manually resolve any conflicts with the main branch and conduct tests to confirm that all functionalities operate correctly.

    - Create PR: Submit a pull request (PR) to integrate your modifications into the main branch, accompanied by a concise summary of the changes and their intended objectives.
        
  ### Review and merge the PR into the `main` branch.
    - Review: Team members review the pull request (PR), and give their feedback or approval.

    - Merge: Once approved, merge the PR into the main branch using an appropriate strategy (merge commit, squash, or rebase). After merging, verify that everything works correctly and delete the feature branch if needed.

## Testing and Validation

To guarantee the reliability of the workflow, adhere to the following testing and validation procedures:

1. **Manual Testing:**
   - Access each `.html` file using a web browser and confirm that the content is displayed correctly.
   - Examine the navigation across various pages to ensure that all links function properly.
   - Check that the "Book Reviews" and "Events" sections feature the most current content.

2. **Code Review:**
   - Ensure that all modifications to the code are evaluated by at least one additional contributor prior to merging.
   - Utilize GitHub's integrated code review features to provide feedback and recommendations..

## Contributor Guidelines

If you wish to contribute to this project, please follow these guidelines:

1. **Fork the Repository:**
   - Initiate your own fork of the repository on GitHub.

2. **Create a Feature Branch:**
   - Always establish a new branch for your feature or bug fix.

3. **Write Descriptive Commit Messages:**
   - Employ comprehensive commit messages that clarify the changes made and the rationale behind them.

4. **Submit a Pull Request:**
   - After finalizing your changes, submit a pull request and request a review from another contributor.

5. **Review and Testing:**
   - Assess the existing code for potential enhancements.
   - Conduct thorough testing of your changes before submission.


### Open any of the .html files in a web browser to view the pages.
  1. Identify .html Files: Utilize File Explorer or Finder, or access your code editor to locate your .html files.

  2. Access in Browser: Right-click on the file and select "Open with" followed by your preferred web browser, or alternatively, drag and drop the file into an active browser window.

  3. Visit Greenwood Library Website: Type the website URL into the address bar of your browser to access the Greenwood Library page and examine its offerings.
   ![Open greenwood library website in browser](./img/27.png)

  ## Final Outcome

Following the integration of contributions from both Morgan and Jamie, the Greenwood Community Library website has been enhanced to feature a new "Book Reviews" section, along with an updated "Events" page that showcases the most recent community happenings.
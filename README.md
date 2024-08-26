# Webex Samples Template

This is the Webex Samples repo template, which must be used for all code contributions. 

Using templates varies from directly forking a repo. The commit history is cleaned, and there is no link to the original repository. This will give your new repository all the framework needed but without the history or link to other repos. It will be easier to track your changes, and your work will not be tied to the repository’s other forks. 

To use this template, [follow these directions to create your new repo from the template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template). Add your project code to the new repo. Then, reach out to Adam Weeks(adweeks) or Ashton Jordan (ashjorda) to have your new repo added to this Github Organization. All newly created repos are set to private by default. Once all Github actions have passed, and your repo is complete, contact to Adam or Ashton for review to make the repo Public. 

This template repo also contains a sample README, that outlines sections you should include in your README to help properly describe the repo's contents. 

## Usage

1. **Clone the repository**: First, clone this repository to your local machine using `git clone git@github.com:WebexSamples/Webex-Samples-Template.git`.

2. **Install dependencies**: Install prettier/autopep8 as per the below instructions under "GitHub Actions" section

## Github Actions

This template uses GitHub Actions workflow to enforce commonly accepted coding practices across various file formats. We use [Prettier](https://prettier.io), and [AutoPep8](https://pypi.org/project/autopep8/) for these linting workflows. These workflows run on every pull request. And before merging is allowed, these workflows must pass. During these workflow checks, none of your code will be modified. These checks are commonly focused on spacing and proper tabbing.  


## Installing Prettier via npm (Local Machine)

**Note: Prettier documentation link: (https://prettier.io/docs/en/install.html)**

To format your code locally, run the following:

1. Install prettier
```bash
npm install --save-dev --save-exact prettier
```

2. Checking what changes prettier would like to make on  all the files within your repo. Before writing them:
```bash
npx prettier . --check
```

3. To write the proposed changes, to ensure the prettier workflow passes. Use the following command:
```bash
npx prettier . --write
```

## Installing AutoPep8 via pip (Local Machine)

**Note: Autopep8 Documentation: (https://pypi.org/project/autopep8/)**

To format your code locally, run the following:

1. Install autopep8
```bash
pip install --upgrade autopep8
```

2. Checking what changes prettier would like to make on  all the files within your repo. Before writing them:
```bash
autopep8 -r --diff --aggressive --aggressive .
```

3. To write the proposed changes, to ensure the prettier workflow passes. Use the following command:
```bash
autopep8 -r -i --aggressive --aggressive .
```

Made with <3 by the Webex Developer Relations Team at Cisco

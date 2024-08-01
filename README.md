# Webex Samples Template

This is the Webex Samples repo template, which must be used for all code contributions. To use this template, clone it using a new branch. And add your project code to the repo. Then create a PR to have your new repo added to this Github Organization. All newly created repo's are set to private by default. Once all Github actions have passed, and your repo is complete. Reach out to Adam Weeks(adweeks) or Ashton Jordan (ashjorda) for review, before making the repo Public. 

This template repo also contains a sample README, that outlines sections you should include in your README to help properly describe the repo's contents. 

## Usage

1. **Clone the repository**: First, clone this repository to your local machine using `git clone git@github.com:WebexSamples/Webex-Samples-Template.git`.

2. **Install dependencies**: Install prettier/autopep8 as per the below instructions under "Github Actions" section

## Github Actions

This template uses GitHub Actions workflow to enforce commmonly accepted coding practices across varios repo file formats. We use Prettier, and AutoPep8 for these linting workflows. These workflows run on every pull request. And before merging is allowed, these workfloes must pass. In conjunction with these workflow checks, none of your actual code is modified. These checks are commonly focued on spacing, and proper tabbing.  


## Installing Prettier via npm (Local Machine)

**Note: Autopep8 documentation link: (https://prettier.io/docs/en/install.html)**

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

Made with <3 by the Webex Developer Evangelism Team at Cisco

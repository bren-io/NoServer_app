# Serverless Web App

A basic guide to the structure of components in a Serverless framework, using AWS, and eventually Flask.

## Installation

Some pre-requirements for the system you intend to deploy from

```
 - git
 - python / pip
 - serverless
 - aws
```

Note that serverless can be installed using node.js and npm. I choose to install the binary for simplicity since this tech stack won't be utilizing node.js.
Also don't forget to setup your git and aws credentials, you can see their documentation for the location of the config files.
As well insure that serverless and aws are configured in your shell path environment

To start, walk through severless (sls) setup by calling. See their documentation for developing in their framework OR old_README.md contains instructions

```sls```

Then in your project directory, clone this repo with a name, create a virtual environment, and install the packages using pip

```
git clone <HTTP/SSH/CLI> <name>		# For me I like to use src as the name since I usually name the sls project the application name
cd <name>
git remote remove origin		# Dereferences this repo because you should have your own! Follow githubs steps when creating a repo through the web or follow what I included in here
git init
git add .
git commit -m "first commit"
git remote add origin <your_repo_url>
git branch -M main
git push -u origin main
python -m venv venv
source venv/bin/activate
```

Note that individual lambda functions will have their own requirements.txt and serverless should handle this
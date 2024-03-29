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

To start, walk through severless (sls) setup by calling. See their documentation for developing in their framework OR when you choose a template sls will create a README.md and serverless.yml files.

```sls```

Simply download the .zip of this repo and unzip it into your sls application. Then follow githubs setup for creating a new repository. If you are developing remotely, you can invoke curl commands to download the .zip or follow these steps I provided below

```
cd <sls app>
git clone --depth 1 <HTTP/SSH/CLI> <repo>		# For me I like to use src as the name since I usually name the sls project the application name
cd <repo>
rm -rf .git				# remember this is a template for you! Follow githubs steps when creating a new repository
python -m venv venv			# create your venv
source venv/bin/activate		# activate before installing dependencies!
```

Note that individual lambda functions will have their own requirements.txt and serverless should handle this
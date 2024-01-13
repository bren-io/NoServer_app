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

To start, walk through severless (sls) setup by calling

```sls```

See their documentation for developing in their framework OR old_README.md contains instructions

Then in your project directory, create a virtual environment and install the packages using pip

```
python -m venv venv
source venv/bin/activate
```

Note that individual lambda functions will have their own requirements.txt and serverless should handle this
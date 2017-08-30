# EC2-Json
Generic JSON script with Comments
requires Python and aws-cli

Step 1: Download aws-cli package

Build Status https://coveralls.io/repos/aws/aws-cli/badge.png
This package provides a unified command line interface to Amazon Web Services.

The aws-cli package works on Python versions:

2.6.5 and greater
2.7.x and greater
3.3.x and greater
3.4.x and greater
3.5.x and greater
Step 2: Install aws-cli

The easiest way to install aws-cli is to use pip:

$ pip install awscli
or, if you are not installing in a virtualenv:

$ sudo pip install awscli
If you have the aws-cli installed and want to upgrade to the latest version you can run:

$ pip install --upgrade awscli
Step 3: Run the script

MUST EDIT ec2-generator.json with details specific to your AWS account and configuration. Be sure to remove all comments from JSON file before running.

From the local directory where your ec2-generator.json file is stored, execute the following:

"To launch a regular instance rather than spot instance, execute the following":

$ aws ec2 run-instances --launch-specification file://ec2-run-script-template.json
Additional configuration options and commands

Please see: https://docs.aws.amazon.com/cli/latest/reference/ec2/

## Buld an AWS AMI Image Using Packer

#### Steps to Run

- An AWS Account with IAM Pragmatic access.
  _If you don't know how to create an IAM user with Pragmatic Access, you can learn do so [here]()_

- Install Packer from [here](https://www.packer.io/downloads)

- Clone the repostiory

- Create a `variable.json` file like this and replace with your IAM credentials amd AMI

  `{`
  `"description": "myWebServer",`
  `"access_key": "Your access key here",`
  `"secret_key": "Your Secret key here",`
  `"source_ami": "Preferred AMI here"`
  `}`

- Make sure to include the ` variable.json` file in your `.gitignore` file as it contains confidential credentials.

- Next, run `setup.sh` to start the build process.

- When build is complete, you can check the `out.json` to see details about the image.

- You can check out your custom Image on your AWS Dashboard under AMI Images in EC2 section..

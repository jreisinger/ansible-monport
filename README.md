## About

Create a virtual servers in AWS and deploy [App::Monport](https://metacpan.org/pod/App::Monport) into it.

## Setup

1) Remove keypair from AWS and private key from ~/.ssh


2) Set environment variables

    export AWS_ACCESS_KEY_ID='AK123'
    export AWS_SECRET_ACCESS_KEY='abc123'
    export GITHUB_TOKEN='ab12'  # for adding ssh public key

3) C3eck *CHECK ME* sections in `main.yml`.

If you do not wish to use private DNS (route53), VPC variable is not
needed and can be removed

Before running playbook, you will need to install and configure `boto`.

## Run

    ansible-playbook main.yml

## Connect

    ssh -i ~/.ssh/ansible-demo ubuntu@<public_ip>

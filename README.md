## About

Create a virtual servers in AWS and deploy App::Monport into it.

## Setup

Check *CHECK ME* sections in `main.yml`.

If you do not wish to use private DNS (route53), VPC variable is not
needed and can be removed

Before running playbook, you will need to install and configure `boto`.

## Run

    export AWS_ACCESS_KEY_ID='AK123'
    export AWS_SECRET_ACCESS_KEY='abc123'

    ansible-playbook main.yml

## Connect

    ssh -i ~/.ssh/ansible-demo ubuntu@<public_ip>

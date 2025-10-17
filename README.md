# ACIT-4640-Labwk7
- Required command(s) to: 
  - create new keys
    ```sh
    ssh-keygen -t ed25519 -f ~/.ssh/aws"
    ```
    - Creates a new key pair name aws and aws.pub in the the ~/.ssh folder
  - run included scripts to import and delete keys
    - Note: If they are not executable, run ```sh chmod +x <file-name>```
    - To import the lab key
        ```sh .\import_lab_key ~/.ssh/aws```
    - To delete the 
    .\delete_lab_key
  - terraform commands (init, fmt, validate, plan and apply)
    - terraform init
    - terraform apply
  - ansible commands (syntax check, run playbook)


- Put commands in code blocks and include a brief description of each command.
- A screenshot of the rendered html page from one of your servers, they should be almost the same, so just a screenshot of one is fine.


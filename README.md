# ACIT-4640-Labwk7
- Required command(s) to: 
  - create new keys
    ```sh
    # Creates a new key pair name aws and aws.pub in the the ~/.ssh folder
    ssh-keygen -t ed25519 -f ~/.ssh/aws"
    ```
  - run included scripts to import and delete keys
    - Note: If they are not executable, run 
    ```sh 
    # Makes <file-name> executable
    chmod +x <file-name>
    ```
    - To import the lab key
    ```sh 
    # Run import file with public key as the argument
    .\import_lab_key ~/.ssh/aws
    ```
    - To delete the lab key
    ```sh 
    #Run delete file (does not require an argument since it deletes based on the name of the key in the file)
    .\delete_lab_key
    ```

  - Terraform commands used (In the Terraform directory)
    - Initialize Terraform
    ```sh
    # Start Terraform
    terraform init
    ```
    - Validate Terraform configuration
    ```sh
    #Ensure terraform .tf file does not have any syntactical errors
    terraform validate
    ```
    - Apply Terraform and run
    ```sh
    #Run terraform file
    terraform apply
    ```
    - Destroy Terraform
    ```sh
    #Once the lab is completed, destroy all resources related to the terraform file
    terraform destroy
    ```
    - Ansible commands used
    ```sh
    #Ensure Ansible syntax is correct after edits
    ansible-playbook -i inventory/hosts.yml playbook.yml --syntax-check

    #Running Ansible playbook
    ansible-playbook -i inventory/hosts.yml playbook.yml
    ```


- A screenshot of the rendered html page from one of the servers
<img width="1048" height="379" alt="{BB8A8F91-F1B5-4285-B9CA-95B261533F1E}" src="https://github.com/user-attachments/assets/1c85a1d2-c941-496f-97c7-380bee01b229" />



# Ansible-lab


# Ansible Web Server Configuration

This Ansible playbook is used to configure web servers with Apache and Nginx.

## Usage

1. **Prerequisites**:
   - Ansible must be installed on the system where you intend to run the playbook.
   - Ensure you have SSH access to the target hosts with appropriate privileges.

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/mostafayounis1/Ansible-lab.git
   cd Ansible-lab






   Modify Playbook (Optional):

    Open the playbook.yml file and modify it according to your requirements.
    Update the src parameter in the copy task to point to the location of your sample website file (any.html).
    Adjust file paths and configurations as needed.

Run the Playbook:

bash

    ansible-playbook -i inventory_file playbook1.yml
    


    Verify Configuration:
        After running the playbook, verify that Apache web server is installed, running, and serving the sample website on the target hosts.
        Check the ownership and permissions of the website files in /var/www/html.

    Access the Website:
        Open a web browser and navigate to the IP address or domain name of the target hosts to access the sample website deployed by Apache.

Playbook Explanation

    Install Apache web server: Installs the Apache web server package (httpd).
    Ensure Apache service is running: Starts the Apache service and enables it to start on boot.
    Deploy sample website for Apache: Copies the any.html file to /var/www/html directory on the target hosts.
    Set proper file permissions for Apache website files: Sets the owner, group, and permissions for the website files to ensure Apache has appropriate access.



    ![Screenshot 2024-05-26 185404](https://github.com/Mostafayouni/Ansible-lab/assets/105316729/639192ee-959d-4f11-a8f4-57cb9626ab15)








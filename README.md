The Ansible Automation Platform 2.4 export factory
=============

**Do you need an AAP 2.4 or AWX?**

1. [Ansible Automation Platform 2.4 here](https://github.com/ericcames/aap24_export_factory/blob/main/docs/NEW_AAP24_CONTROLLER.md "AAP24")<br>
2. [Ansible Web eXecutable](https://github.com/ericcames/aap24_export_factory/blob/main/docs/NEW_AWX_CONTROLLER.md "AWX")<br>

**Getting started**

1. [Get Automation Hub Token](https://console.redhat.com/ansible/automation-hub/token/ "Load Token")<br>
2. Ensure that we have a certified credential
    - Name
    ```
    Automation Hub - certified
    ```
    - Credential type
    ```
    Ansible Galaxy/Automation Hub API Token
    ```
    - Galaxy Server URL
    ```
    https://console.redhat.com/api/automation-hub/content/published/
    ```
    - Auth Server URL
    ```
    https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token
    ```
    - API Token

![alt text](https://github.com/ericcames/aap24_export_factory/blob/main/docs/images/aap24cred.png "certified")

3. Ensure that we have a validated credential
    - Name
    ```
    Automation Hub - validated
    ```
    - Credential type
    ```
    Ansible Galaxy/Automation Hub API Token
    ```
    - Galaxy Server URL
    ```
    https://console.redhat.com/api/automation-hub/content/validated/
    ```
    - Auth Server URL
    ```
    https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token
    ```
    - API Token

4. Ensure the Galaxy credentials are related to the Default Organization
![alt text](https://github.com/ericcames/aap24_export_factory/blob/main/docs/images/aap24orgcreds.png "Default Organization")

5. Create your project
![alt text](https://github.com/ericcames/aap24_export_factory/blob/main/docs/images/aap24proj.png "Project")<br>

    - Name
    ```
    aap24_export_factory
    ```
    - Organization
    ```
    Default
    ```
    - Source Control Type
    ```
    Git
    ```
    - Source Control URL
    ```
    https://github.com/ericcames/aap24_export_factory.git
    ```
6. Create your ansible automation platform credential
![alt text](https://github.com/ericcames/aap24_export_factory/blob/main/docs/images/aap24platcred.png "Cred")

    - Name
    ```
    AAP Credential
    ```
    - Credential Type
    ```
    Red Hat Ansible Automation Platform
    ```
    - Red Hat Ansible Automation Platform
    ```
    https://dev0-aap.apps.rosa.rosa-86rjc.jsdv.p3.openshiftapps.com
    ```

7. Create your job template
![alt text](https://github.com/ericcames/aap24_export_factory/blob/main/docs/images/aap24temp.png "Template")

- Name
```
Export AAP 24 Objects
```

Survey variables
```
personal_access_token
```
8. Launch the job template

9. You will find your AAP 2.4 objects here:

   - [AAP 2.4 Conversation Factory](https://github.com/ericcames/aap24_conversion_factory/tree/main/aap24_configs "Conversion Factory")<br>

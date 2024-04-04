---
title: Git & GitHub
weight: 1
---

# Git Setup
1. Download and install [Git](https://git-scm.com/downloads)
    - If you are prompted with an option similar to `Add to PATH?`, select `Yes`
2. Open a terminal (or command prompt) and run the following commands:
    - Make sure it's an email you don't mind disclosing publicly
    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

# GitHub Setup
1. Create a [GitHub](https://github.com) account
    - Follow the instructions in the signup flow
2. You will be required to have 2FA (2-Factor Authentication) enabled. To enable it:
    1. Click your profile picture
    2. Click `Settings`
    3. Go to the `Password and authenthication` tab
    4. Click `Enable` on the `Two-factor authentication` section
    5. Follow the instructions to set up 2FA
        - It is highly recommended to choose either `Security Key` (if you have one available), or `Authenticator app (TOTP)` as your 2FA method
3. Setup authentication in Git

    === "SSH"
        SSH authentication is **recommended** because it provides improved security over HTTP(S). However, please read the warning below.

        !!! warning

            School WiFi appears to block SSH connections. If you choose to use SSH authenthication, you may be unable to connect
            to Git while on school WiFi (you will have to use a VPN, data connection, or similar). You may want to consider using [HTTP](#http) instead.
        
        1. 
    
    === "HTTP"

        1. 

4. Contact the Programming Lead to request the appropriate access to the organization, if required for your role


# Cloning the Repository
Once you have Git, GitHub, and GitHub authentication set up, you can begin cloning the repository. To do so, follow the instructions below:

1. Navigate to the folder you want the repository to be cloned to
    - It will be in a subfolder named after the repository you're cloning (e.g. `FRC2024`), you do not need to create a folder yourself
2. Open a terminal (or command prompt) and run the clone command with the appropriate address for the repository you're cloning.  
*Make sure you are cloning the right year's code, at time of writing, this is `FRC2024`.*
    ```bash
    # For SSH authentication
    git clone git@github.com:AgincourtSkunkworks/FRC2024.git

    # For HTTP authentication
    git clone https://github.com/AgincourtSkunkworks/FRC2024.git
    ```
3. You should now have a folder named after the repository you cloned (e.g. `FRC2024`). This is the root of the repository, and all code will be contained within this folder.

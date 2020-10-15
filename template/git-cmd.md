### How to Fork FIPS

 1. Login Your Github account, Fork the repository by clicking "Fork" button.

 2. Then clone the repository to your local space.You can get the URL by clicking the "Code" button.

    ```bash
    git clone https://github.com/yourname/FIPS.git
    cd FIPS
    ```

 3. Put your fip-xxx.md into the "FIPS" directory.Then "git add" it add "git commit".

    ```bash
      git add FIPS/fip-xxx.md
    
      git commit -m (your commit message)
    ```

 4. Then push to your remote repository.

    ```bash
    git push origin master
    ```

 5. Open your repository on browser and click the "Pull request" button below the "Code" button. The link should be "https://github.com/xxx/FIPS/pull/new/master".And choose correct repository and branch name on the right. Click the "Create pull request" button and wait for further message.

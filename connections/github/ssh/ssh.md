
# SSH CONNECTION

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent


## 1. Create SSH Key

    $ ssh-keygen -t ed25519 -C "andresganc@gmail.com"


## 2. Start the ssh-agent in the background.

    $ eval "$(ssh-agent -s)"
        > Agent pid 59566


## 3. Add your SSH private key to the ssh-agent.

    $ ssh-add ~/.ssh/id_ed25519


## 4. Copy Public Key 

    $ nano ~/.ssh/id_ed25519.pub


## 5. Adding a new SSH key to your GitHub account

    ![Alt text](image.png)


### 5.1 In the "Access" section of the sidebar, click  SSH and GPG keys.

### 5.2 Click New SSH key or Add SSH key.

### 5.3 In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal laptop, you might call this key "Personal laptop".

### 5.4 Select the type of key, either authentication or signing. For more information about commit signing, see "About commit signature verification."

### 5.5 In the "Key" field, paste your public key.

### 5.6 Click Add SSH key.


## 6. In the upper-right corner of any page, click your profile photo, then click Settings.
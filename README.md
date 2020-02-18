# Useful Terminal Commands

## BASH

### Create a script
```
touch <SCRIPT_NAME>.sh
chmod +x <SCRIPT_NAME>.sh
echo '#!/bin/bash' > <SCRIPT_NAME>.sh
```

### Run a script
```
./<SCRIPT_NAME>.sh
```

## DIRECTORY & FILE

### Change directory ownership
```
sudo chown -R <USER> <DIRECTORY>
```

### Create file
```
touch <FILE>
```

### Delete directory
```
rm -rf <DIRECTORY>
```

### Delete file
```
rm <FILE>
```

### Rename file
```
mv <OLD_FILE> <NEW_FILE>
```

## GIT

### Clear Git history
```
rm -rf .git
git init
git add .
git commit -m "<MESSAGE>"
git remote add origin git@github.com:<YOUR_ACCOUNT>/<YOUR_REPOS>.git
git push -u --force origin master
```

### Get Git repository URL
```
git remote get-url origin
```

### Keep a fork up to date
```
git clone git@github.com:<YOUR_ACCOUNT>/<YOUR REPOS>.git
cd <YOUR_REPOS>/
git remote add upstream git://github.com/<THEIR_ACCOUNT>/<THEIR_REPOS>.git
git fetch upstream
git merge upstream/master <BRANCH>
```

## JEKYLL

### Start project after cloning
```
bundle install --path vendor/bundle
bundle exec jekyll serve
```

## SSH

### Generate new SSH Key
```
ssh-keygen -o
cat ~/.ssh/id_rsa.pub
```
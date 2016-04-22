# Setting up the Homebrew package manager

http://brew.sh

### Prereqs

- sudo permissions for current user
- Command Line Tools via  
  ```
  xcode-select --install
  ```

### Install

1. Install brew via  
  ```
  ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  ```
1. Verify brew intall via  
  ```
  brew help
  ```

### Some popular installs

`brew install ...`

- node
- git _(since default mac version is potentialy out of date)_
- bash-completion

----

`brew cask install ...`

- [shuttle](http://fitztrev.github.io/shuttle/)
- [spectacle](https://www.spectacleapp.com/)
- java
- [atom](https://atom.io/)
- slack
- google-chrome

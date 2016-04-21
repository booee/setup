# Git

A setup guide for initializing and improving the git CLI experience

### Prereqs

- Homebrew
- Git
- bash-completion

```
  brew install git bash-completion
```

### Setup

1. Configure the global users configs
```
  git config --global user.name "First Last"
  git config --global user.email "email@example.com"
  ... etc
```

1. Create `~/.gitexcludes` and include the following:  
```
  .DS_Store
```

1. Integrate into the terminal prompt by updating `~/.bash_profile` to include  
```
  # Bash completion is where it's at
  if [ -f $(brew --prefix)/etc/bash_completion ]; then
      . $(brew --prefix)/etc/bash_completion
  fi

  # Customize the prompt to include your current working branch
  source $(brew --prefix)/etc/bash_completion
  GIT_PS1_SHOWDIRTYSTATE=true
  export PS1='\u@\h: \w$(__git_ps1) 🧀  '
```

### Resources

- https://git-scm.com/
- https://gist.github.com/trey/2722934

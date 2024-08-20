# Initial steps
* create a remote repository
* clone to local machine 
* index.html (copy from Zhenhua Yu)
# Install Jekyll (https://jekyllrb.com/docs/installation/macos/)

``` /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" ```

```brew install chruby ruby-install xz```

```ruby-install ruby 3.1.3```

```
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version
```
If you’re using Bash, replace ```.zshrc``` with ```.bash_profile```. If you’re not sure, read this external guide to find out which shell you’re using (https://www.moncefbelyamani.com/which-shell-am-i-using-how-can-i-switch/).


Quit and relaunch Terminal, then check that everything is working:

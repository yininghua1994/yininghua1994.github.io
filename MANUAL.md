# Initial steps
* create a remote repository
* clone to local machine 
* index.html (copy from Zhenhua Yu)
# Install Jekyll (https://jekyllrb.com/docs/installation/macos/)
## Install Ruby
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

```ruby -v```

First time the version is incorrect. Try the process again as below - 

```brew update```

```brew install ruby```

```
echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```
**Make sure using ```.zshrc``` rather than ```.bash_profile```** 

## Install Jekyll

```gem install jekyll```

check ``` jekyll -v```

I have some path issues, solution from chatgpt:

* Identify the Path to the Ruby bin Directory ```gem environment```
* I provide chatgpt the two path
1. INSTALLATION DIRECTORY is /opt/homebrew/lib/ruby/gems/3.3.0
2. EXECUTABLE DIRECTORY is /opt/homebrew/lib/ruby/gems/3.3.0/bin
  
Chatgpt said I should add ```export PATH="/opt/homebrew/lib/ruby/gems/3.3.0/bin:$PATH```to the end of ```.zshrc```
Then ```source ~/.zshrc```

check again ```jekyll -v``` - works.






# aubel-r.github.io
This repository hosts landing page (and related stuff like app-ads.txt, security policy) for _7 letters for 1 word_

# Jekyll on Ubuntu

[source](https://jekyllrb.com/docs/installation/ubuntu/)
Install Ruby and other prerequisites:

```
sudo apt-get install ruby-full build-essential zlib1g-dev
```  

Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your ~/.bashrc file to configure the gem installation path:

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```  

Finally, install Jekyll and Bundler:

```
gem install jekyll bundler
bundle install
```  

> Note: if `bundle install` fails, it may be necessary to delete the lock file (`rm Gemfile.lock`).

That’s it! You’re ready to start using Jekyll.

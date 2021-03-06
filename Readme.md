# Install Ruby on Rails
![Rails logo](/assets/images/rails.png)

- [macOS install](#macos-install)
- [Ubuntu/Linux install](#ubuntu-install)
- [Windows install](#windows-install)

---



### macOS install
![macOS logo](/assets/images/macos.png)

#### Install rbenv (ruby environment)
[rbenv](https://github.com/rbenv/rbenv) is a ruby version manager similar to [rvm](https://rvm.io/) however rbenv works on both Mac & Linux. If you have to learn something - it's nicer to learn something that covers two environments rather than one in case you ever need to use it in a mac/linux environment.

1. Install developer libraries from Apple
  ```
  xcode-select --install
  ```
2. Install [brew](https://brew.sh/)
3. Install rbenv (Terminal app)
  ```
  brew install rbenv
  ```
4. Setup rbenv
  ```
  rbenv init
  ```
5. Add rbenv to your *~/.bash_profile*
  NOTE: these will not give you back any feedback to tell you they are complete.
  ```
  echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
  ```
  ```
  echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
  ```
6. Reopen the terminal and install ruby
  ```
  rbenv install 2.4.1
  ```
7. Setup the version of Ruby you wish to use
  ```
  rbenv local 2.4.1
  ```
8. Once Ruby has been set to *local* you should be able to verify which version you have
  ```
  ruby -v
  ```
9. Install Ruby On Rails
  ```
  gem install rails --version 5.1.1 --no-ri --no-rdoc && rbenv rehash
  ```
  Type ```rails -v``` to test your version

---



### Ubuntu Install
![ubuntu logo](/assets/images/ubuntu.png)

#### Install rbenv (ruby environment)
[rbenv](https://github.com/rbenv/rbenv) is a ruby version manager similar to [rvm](https://rvm.io/) however rbenv works on both Mac & Linux. If you have to learn something - it's nicer to learn something that covers two environments rather than one in case you ever need to use it in a mac/linux environment.

1. Install [git](https://git-scm.com/download/linux) if you haven't already
2. Update your Ubuntu (in your terminal)
  ```
  sudo apt-get update
  ```
3. Get some required dependancies
  ```
  sudo apt-get install autoconf bison build-essential libssl-dev libyaml-dev libreadline6-dev zlib1g-dev libncurses5-dev libffi-dev libgdbm3 libgdbm-dev nodejs sqlite3 libsqlite3-dev  
  ```
4. Using git - download *rbenv* git repo to a hidden directory
  ```
  git clone https://github.com/rbenv/rbenv.git ~/.rbenv
  ```
5. Add terminal commands for rbenv
  NOTE: these will not give you back any feedback to tell you they are complete.
  ```
  echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
  ```
  ```
  echo 'eval "$(rbenv init -)"' >> ~/.bashrc
  ```
6. Run command for rbenv
  ```
  source ~/.bashrc
  ```
7. Check if rbenv works
  ```
  type rbenv
  ```
  You should get back a "rbenv is a function" in the terminal

8. Install ruby-build to help rbenv using git
  ```
  git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
  ```
9. Install ruby using rbenv
  ```
  rbenv install 2.4.1
  ```
10. Setup the version of Ruby you wish to use
  ```
  rbenv local 2.4.1
  ```
11. Once Ruby has been set to *local* you should be able to verify which version you have
  ```
  ruby -v
  ```  
12. Install Ruby On Rails
  ```
  gem install rails --version 5.1.1 --no-ri --no-rdoc && rbenv rehash
  ```
  Type ```rails -v``` to test your version

---




### Windows Install
![windows logo](/assets/images/windows.png)

1. Download and install [Ruby 2.4.1-1 (x64)](https://rubyinstaller.org/downloads/)
2. You will be given options during the install [1,2,3]. One at a time use all 3 options.
3. Once Ruby has been installed you should be able to verify which version you have, open **Powershell** or **cmd** and type:
  ```
  ruby -v
  ```
4. Install rails using Powershell/CMD
  ```
  gem install rails
  ```
5. Type ```rails -v``` to test your version

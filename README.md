# Gonzalo Acosta's Personal Page



This is Gonzalo Acosta's personal website. This gitpage is powered by [Jenkyll](https://jekyllrb.com/) which is a tool to create static websites.

### Install Jenkyll in Windows:

1. Download and install a Ruby+Devkit version from [RubyInstaller Downloads](https://rubyinstaller.org/downloads/). Use default options for installation.
2. Run the ridk install step on the last stage of the installation wizard. This is needed for installing gems with native extensions. You can find additional information regarding this in the [RubyInstaller Documentation](https://github.com/oneclick/rubyinstaller2#using-the-installer-on-a-target-system)
3. Open a new command prompt window from the start menu, so that changes to the `PATH` environment variable becomes effective. Install Jekyll and Bundler using `gem install jekyll bundler`
4. Check if Jekyll has been installed properly: `jekyll -v`

### Install Jenkyll in MacOS with Hombrew:

#### Installing Ruby

1. To run the latest Ruby version you need to install it through [Homebrew](https://brew.sh/).

   ```bash
   # Install Homebrew
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   
   # Install Ruby
   brew install ruby
   ```

2. Add the brew ruby and gems path to your shell configuration:

   ```bash
   # If you're using Zsh
   echo 'export PATH="/usr/local/opt/ruby/bin:/usr/local/lib/ruby/gems/3.0.0/bin:$PATH"' >> ~/.zshrc
   
   # If you're using Bash
   echo 'export PATH="/usr/local/opt/ruby/bin:/usr/local/lib/ruby/gems/3.0.0/bin:$PATH"' >> ~/.bash_profile
   
   # Unsure which shell you are using? Type
   echo $SHELL
   ```

3. Relaunch your terminal and check your Ruby setup:

   ```
   which ruby
   # /usr/local/opt/ruby/bin/ruby
   
   ruby -v
   ruby 3.0.0p0 (2020-12-25 revision 95aff21468)
   ```

#### Installing Jenkyll

1. Install the bundler and jekyll gems:

   ```bash
   gem install --user-install bundler jekyll
   
   ```

2. Get your Ruby version:

   ```
   ruby -v
   ruby 3.0.0p0 (2020-12-25 revision 95aff21468)
   ```

3. Append your path file with the following, replacing the `X.X` with the first two digits of your Ruby version:

   ```bash
   # If you're using Zsh
   echo 'export PATH="$HOME/.gem/ruby/X.X.0/bin:$PATH"' >> ~/.zshrc
   
   # If you're using Bash
   echo 'export PATH="$HOME/.gem/ruby/X.X.0/bin:$PATH"' >> ~/.bash_profile
   
   # Unsure which shell you are using? Type
   echo $SHELL
   ```

4. Check that `GEM PATHS:` points to your home directory:

   ```
   gem env
   ```

More informacion on how to install Jenkyll [here](https://jekyllrb.com/docs/installation/)



### Run Jenkyll

Run the following command in the folder

```bash
bundle exec jekyll serve
```



## Theme

The theme used for this page is the [modern-resume-theme](https://github.com/sproogen/modern-resume-theme) by  [James Grant](https://github.com/sproogen)

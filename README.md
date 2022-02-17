# nanoimaging.de


This webpage is based on [Jekyll](https://jekyllrb.com/), a very popular static website generator.
The main theme is [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes).
We use [GitHub Actions](https://jekyllrb.com/docs/continuous-integration/github-actions/) to automagically build the webpage.
The output is a static webpage which is hosted at GitHub. The domain `nanoimaging.de` just points to the IP adress of the webpage.
You don't have to update any server!
Hosted [here](bionanoimaging.github.io).

## A few notes
* Pictures of people only 300px * 300px!
* Please check always locally if the webpage still builds!
* Don't add pictures >1MB to git. In general don't update binary files (such as images, PDF, ...) too often.



## Hosting for Development
Navigate to the folder and then call:
```
bundle exec jekyll serve
```

## Installation (Linux)

Install:
```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Put the following lines in your `~/.bashrc` or `~/.zshrc`:
```bash
# Install Ruby Gems to ~/gems' >> ~/.bashrc
export GEM_HOME="$HOME/gems"
export PATH="$HOME/gems/bin:$PATH"
```
and call `soure ~/.zshrc`.

Then install Jekyll with
```bash
gem install jekyll bundler
```

For installation of the theme, see [here](https://github.com/mmistakes/minimal-mistakes#gem-based-method)


## Theme
In general we install the theme independently, however some files in `_includes` or `_layout` are changed and hence
we copied our version to that location. That overrides the default templates.

STEPS

    1 - jekyll new [nameOfTheSite]
    2 - cd [nameOfTheSite]
    3 - npm install -g glup
    4 - npm install --save-dev gulp-shell lodash gulp browser-sync


WINDOWS INSTALLATION

"""
C:/Ruby24-x64/lib/ruby/gems/2.4.0/gems/bundler-1.15.3/lib/bundler/resolver.rb:39
6:in `block in verify_gemfile_dependencies_are_found!': Could not find gem 'tzin
fo-data x64-mingw32' in any of the gem sources listed in your Gemfile. (Bundler:
:GemNotFound)
"""
Solution: You are missing a gem

- gem install tzinfo-data, platforms: [:mingw, :mswin, :x64_mingw]
- bundle install


"""
You have already activated liquid 4.0.0, but yo
ur Gemfile requires liquid 3.0.6. Prepending `bundle exec` to your command may s
olve this. (Gem::LoadError)
"""
Solution: Your Jekyll is using another version of liquid. You can for pacage usage with bundle exex

DON'T
- jekyll build
DO
- bundle exec jekyll build



http://railsapps.github.io/tutorial-rails-devise-rspec-cucumber.html
RailsApps Tutorials: Devise with RSpec and Cucumber
は rvm を利用する形で欠かれている。これを rbenv を利用して スクラッチからなぞってみた。(on mac 10.9.2)

最初の環境構築が、記事内とことなるだけで、あとは記事通りにすすめていけば良いはず。

    $ brew install rbenv ruby-build rbenv-gemset rbenv-gem-rehash
    $ rbenv install 2.0.0-p451 # 2.0.0 系の最新のものを指定する。
    
    $ cd work
    $ rbenv local 2.0.0-p451
    $ ruby -v                   # 2.0.0-p452 であることを確認する。
    
    $ rbenv gem create 2.0.0-p451 rails3-devise-rspec-cucumber
    $ echo rails3-devise-rspec-cucumber > .rbenv-gemsets
    $ rbenv gemset active      # rails3-devise-rspec-cucumber であることを確認する
    
    $ gem install bundler
    $ gem install rails -v 3.2.17
    
    $ rails new rails3-devise-rspec-cucumber -T
    $ cd rails3-devise-rspec-cucumber
    $ mv ../.ruby-version .
    $ mv ../.rbenv-gemsets .



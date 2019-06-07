require 'capistrano/setup'
require 'capistrano/deploy'

require 'capistrano/rbenv' if ENV['rbenv']
require 'capistrano/bundler'
require 'capistrano/rails/assets'
require 'capistrano/puma'

require 'capistrano/rvm'
require 'capistrano/rails/assets'

require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git
install_plugin Capistrano::Puma

Dir.glob('lib/capistrano/tasks/*.rake').each { |r| import r }

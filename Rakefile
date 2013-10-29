$:.unshift File.dirname(__FILE__) + 'lib'

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new
task :default => :spec

desc "Run /lib/racional.rb"
task :bin do
  sh "ruby /lib/racional.rb"
end

desc "Testeando con Rspec"
task :test do
 sh "rspec -I. racional_spec.rb --format documentation"
end

desc "Testeando con Rspec"
task :thtml do
 sh "rspec -I. racional_spec.rb --format html"
end


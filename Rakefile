require 'rubygems'
require 'rake/testtask'

task :default => :test

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "feedbag-grow20"
    gem.summary = "Fork of Feedbag"
    gem.email = "alvin@grow20.com"
    gem.homepage = "http://github.com/aliang/feedbag"
    gem.description = "Fork of Feedbag, for feed discovery, using nokogiri"
    gem.authors = ["Alvin Liang", "Axiombox", "David Moreno"]
    gem.add_dependency "nokogiri"
    gem.add_development_dependency "hpricot"
    gem.add_development_dependency "mocha"
    gem.add_development_dependency "active_support"
  end
rescue LoadError
  puts "Jeweler not available. Install it with: sudo gem install technicalpickles-jeweler -s http://gems.github.com"
end

Rake::TestTask.new do |t|
  t.libs << 'test'
  $: << "."
  t.test_files = FileList["./test/feedbag_test.rb"]
  t.verbose = true
end

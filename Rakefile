require 'rubygems'
require 'rake/testtask'

task :default => :test

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gemspec|
    gemspec.name = "the-perfect-gem"
    gemspec.summary = "Summarize your gem"
    gemspec.description = "Describe your gem"
    gemspec.email = "josh@technicalpickles.com"
    gemspec.homepage = "http://github.com/technicalpickles/the-perfect-gem"
    gemspec.description = "TODO"
    gemspec.authors = ["Josh Nichols"]
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

require 'bundler/gem_tasks'
require 'rake/testtask'
require 'rubocop/rake_task'

Rake::TestTask.new do |t|
  t.libs.push 'lib'
  t.test_files = FileList['test/test_*.rb']
  t.ruby_opts += ['-W1']
end

RuboCop::RakeTask.new

task default: [:test, :rubocop]

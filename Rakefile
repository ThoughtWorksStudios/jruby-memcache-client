begin
  require 'jeweler'
  Jeweler::Tasks.new do |gemspec|
    gemspec.version = "1.8.0"
    gemspec.name = "jruby-memcache-client-thoughtworks"
    gemspec.summary = "A drop in replacement for Ruby's memcache-client. Now with a stable jruby-memcached-release jar."
    gemspec.email = "sudhindra.r.rao@gmail.com"
    gemspec.homepage = "http://github.com/ThoughtWorksStudios/jruby-memcache-client"
    gemspec.description = "A drop in replacement for Ruby's memcache-client.Now with a stable jruby-memcached-release jar."
    gemspec.authors = ["Abhi Yerra", "Ikai Lan", "Frederic Jean", "Lennon Day-Reynolds",
		"slyphon", "Brayn Helmkamp", "Travis Tilley", "Sudhindra Rao(ThoughtWorksStudios)"]
  end
rescue LoadError
  puts "Jeweler not available. Install it with: sudo gem install technicalpickles-jeweler -s http://gems.github.com"
end

if RUBY_PLATFORM =~ /java/i
  begin
    require 'spec/rake/spectask'

    task :default => :spec

    desc "Run the specs for the jruby-memcache-client gem"
    Spec::Rake::SpecTask.new
  rescue LoadError
    puts "You must have rspec installed in order to run the tests."
  end
else
  puts "You must run rake under JRuby."
end

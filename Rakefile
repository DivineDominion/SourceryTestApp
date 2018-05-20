task :build do
  system "git submodule update --init external/Sourcery"
  system "cd external/Sourcery/; swift build"
end

task :run do
  sourcery_path = File.join(File.dirname(__FILE__), "external", "Sourcery", ".build", "debug", "sourcery")
  system "#{sourcery_path}"
end

task :default => [:build, :run]

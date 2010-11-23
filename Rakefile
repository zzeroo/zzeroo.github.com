

desc "Open a new Post in vim with $1 as title"
task :post do
  if ARGV[1].nil?; puts "usage: rake post a_describing_post_title"; exit 0; end
  system ( "vim ./_posts/`date +%F`-#{ARGV[1].gsub(/ /, '_')}.textile" )
end

desc "Make the blog"
task :make do
  system ( "jekyll --rdiscount" )
end

desc "Start a jekyll server"
task :jserver do
  system ( "jekyll --pygments --server --auto" )
end


desc "Install the environment"
task :install do
  system ( "bundle install" )
  system ( "sudo apt-get install python-pygments" )
end

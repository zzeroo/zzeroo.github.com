

desc "Open a new Post in vim with $1 as title"
task :post do
  system ( "vim ./_posts/`date +%F`-#{ARGV[1].gsub(/ /, '_')}.textile" )
end


desc "Start a jekyll server"
task :jserver do
  system ( "jekyll --pygments --server --auto" )
end

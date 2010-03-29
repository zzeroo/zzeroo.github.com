

desc "Open a new Post in vim with $1 as title"
task :post do
  system ( "vim ./_posts/`date +%F`-#{ARGV[1]}.textile" )
end

task :default => :html

task :html => %W[ch1.html ch2.html ch3.html]

rule ".html" => ".md" do |t|
  sh "pandoc -o #{t.name} #{t.source}"
end
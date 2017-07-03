[jekyll-import](https://github.com/jekyll/jekyll-import)

```
  ~$ irb -r jekyll-import
  >> JekyllImport::Importers::Tumblr.require_deps
  => ["rubygems", "fileutils", "open-uri", "nokogiri", "json", "uri", "time", "jekyll"]
  >> JekyllImport::Importers::Tumblr.process("url" => "http://backlog.robbevan.com")

```

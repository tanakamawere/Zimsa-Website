source "https://rubygems.org"

# Core dependencies
gem "webrick"        # Needed for local Jekyll server on Ruby 3.x
gem "jekyll"         # Main site generator
gem "csv"            # Ruby 3.4+ no longer includes this by default
gem "logger"    
gem "base64"     # Future-proofing: Ruby 3.5+ removes from default gems

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]

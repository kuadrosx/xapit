source "http://rubygems.org"

case ENV["MODEL_ADAPTER"]
when nil, "active_record"
  gem "sqlite3"
  gem "activerecord", :require => "active_record"
  gem "with_model"
when "data_mapper"
  gem "dm-core", "~> 1.0.2"
  gem "dm-sqlite-adapter", "~> 1.0.2"
  gem "dm-migrations", "~> 1.0.2"
else
  raise "Unknown model adapter: #{ENV["MODEL_ADAPTER"]}"
end

gemspec

rvm use ruby-2.2.1@global

gem install bundler

rm -rf vendor/bundle;
rm -rf build
rm -rf source/assets/images/files
bundle install --path ~/.shared_gems
bundle exec site321 download;
bundle exec middleman deploy --build-before;

if [[ -n '$SEARCH' ]]; then
  bundle exec middleman sus;
fi

# Peastash::Mongo

*IN PROGRESS*: this gem is not working yet.

With the release of `Mongoid` 4, the `MongoDB` driver switched from `Moped` to the official `Mongo` ruby driver.
Unfortunately, this new ruby driver does not instrument queries with `ActiveSupport::Notifications` like `Moped` did.

Luckily, it provides hooks to plug any kind of instrumentation and monitoring, which is even better, and precisely what this gem does.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'peastash-mongo'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install peastash-mongo

## Usage

If you're already using peastash in a Rails project, you're all set!
Just watch the following `ActiveSupport::Notifications`: `query.mongo`.

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/peastash-mongo. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).


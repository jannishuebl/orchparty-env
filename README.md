# Orchparty::Env

[![Build Status](https://travis-ci.org/jannishuebl/orchparty-env.svg?branch=master)](https://travis-ci.org/jannishuebl/orchparty-env)
[![Gem Version](https://badge.fury.io/rb/orchparty-env.svg)](https://badge.fury.io/rb/orchparty-env)

This is a [Orchparty](https://orch.party/) plugin to extract
environment variables of a orchparty file.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'orchparty-env'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install orchparty-env

## Usage

Run orchparty with the env generator:

```bash
orchparty generate env -f stack.rb -a application-name
```

For more information run:

```bash
orchparty generate env --help

```

For exec a command with the environment variables you can run:

```bash
export `orchparty generate env -f input.rb -a application-name`; bash -c "echo $EXAMPLE_VARIABLE"
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at
https://github.com/jannishuebl/orchparty-env.


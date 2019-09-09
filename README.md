# hrsc-style

HRSC shared style configs.

## Installation

Add this line to your application's Gemfile:

```ruby
group :test, :development do
  gem 'hrsc-style'
end
```

Or, for a Ruby library, add this to your gemspec:

```ruby
spec.add_development_dependency 'hrsc-style'
```

And then run:

```bash
$ bundle install
```

## Usage

Create a `.rubocop.yml` with the following directives:

```yaml
inherit_gem:
  hrsc-style:
    - default.yml
```

Now, run:

```bash
$ bundle exec rubocop
```

You do not need to include rubocop directly in your application's dependences. HRSC-style will include a specific version of `rubocop` that is shared across all projects.

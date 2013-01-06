# LetterOpenerWeb

Gives [letter_opener](https://github.com/ryanb/letter_opener) an interface for
browsing sent emails.

## Installation

Add this line to your application's Gemfile:

    gem 'letter_opener_web'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install letter_opener_web

## Usage

Add to your routes.rb:

```ruby
Your::Application.routes.draw do
  if Rails.env.development?
    mount LetterOpenerWeb::Engine, at: "/letter_opener"
  end
end
```

## Credits

Part of the code was based on [this pull request](https://github.com/ryanb/letter_opener/pull/12)
by [@alexrothenberg](https://github.com/alexrothenberg).

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

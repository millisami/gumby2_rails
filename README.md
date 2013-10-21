# Gumby2Rails

TODO: Write a gem description

## Installation

Add this line to your application's Gemfile:

    gem 'gumby2_rails'

You should also add the following supporting gems to your `Gemfile`

    gem "compass-rails", "~> 2.0.alpha.0"
    gem "modular-scale"
    gem "modernizr-rails"


And then execute:

    $ bundle

## Usage

If your app is using the asset pipeline with sprocket manifest, then just require it in the `application.css`

    *= require 'gumby2_rails'

#### If you want to use the Mixins provided by GumbyFramework

To use the (sass mixins)[http://sass-lang.com/#mixins] given by the (GumbyFramework)[http://gumbyframework.com/], it has to be imported instead of required.
So, if you are using `application.css` and have sprocket directives, you need to change it to the sassy way.

First, rename the file to '.scss' or '.sass' extension, whichever syntax you prefer.
Then replace the directives with imports.

So, change the `application.scss` file with appropriate `@imports` to your other files, if you have and add
    
    @import gumby2_mixins_rails;

Now, in your `scss` files, you can use all the (GumbyFramework Mixins)[http://gumbyframework.com/docs/mixins/]

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

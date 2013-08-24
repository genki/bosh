# Rosh

Rosh is roaming shell.
It can automatically reconnect to the host with the remote GNU screen session.

## Installation

Add this line to your application's Gemfile:

    gem 'rosh'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install rosh

## Usage

    rosh [options] hostname [GNU_screen_session_name]

    -a alive-interval   Set ssh option ServerAliveInterval. Default: 5
    -e escape           Set the escape charactor of the outer screen session.
                        Default: "^t"

To detach the outer screen session,

    ^t d

To send the command to the inner screen session,

    ^a

Currently it is not configurable, but the source code is very simple
to be customizable.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

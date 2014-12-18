# Dockerized Ruby for non-root processes

# Versions

* 2.1.5, latest


# Usage

## Base image

As expected, use it in the `FROM` instruction.

    FROM arnau/ruby:2.1.5
    # your instructions

## Single run

    docker run -it --rm \
      -v "$(pwd)":/usr/local/foo \
      -w /usr/local/foo \
      arnau/ruby:2.1.5 \
      ruby foo.rb


# License

View [license information](https://www.ruby-lang.org/en/about/license.txt)
for the software contained in this image.

medium2markdown
===============

[Medium](http://www.medium.com/) is a blogging platform, currently in beta. They offer the ability to take the content you've written on their platform and export it. The export is currently just HTML, so I wrote medium2markdown to parse it and dump it as Markdown, which you can then use elsewhere. (It's quite possible that Medium will provide Markdown export in the future, which would be ideal.)

This isn't to say that you shouldn't use Medium. The people there have built a very interesting platform, which I've enjoyed using, and I'm watching its progress with interest.

I've written medium2markdown to be fairly bare-bones, and you may disagree with my parsing choices - forks are welcome, as are pull requests. At some point I'll probably add medium2jeykll to write out a more Jekyll-specific format.

## Requirements

perl, with HTML::TreeBulder.

## Usage

By default, it will take all .html files in the current directory and convert them, taking foo.html and writing foo.md:

    medium2markdown

Alternatively, you can specify specific HTML files to parse:

    medium2markdown foo.html bar.html


ctape
=====

Save digital data onto a Compact Cassette using a format
resembling that of Commodore Datassette.

Needs a config file named `config.yml`. Example:

    device: -t alsa "default"
    bitlen: 16
    volume: 0.98

Usage:

* encoding: `./tape-write.rb < FILE`
* decoding: `./tape-read.rb > FILE`

Explanation and videos in [this blog post](http://windytan.blogspot.fi/2012/08/vintage-bits-on-cassettes.html).

NOTE: This is an art project, built for fun, and not in active development any more.
Many people haven't gotten it working. Can you find why it doesn't work? Can you perhaps fix it?

`tape-write.rb` encodes data from stdin to the sound card. `tape-read.rb` records from
the sound card and decodes to stdout.

A WORD OF WARNING. Before running the script, please make sure
that your speakers are turned off. For noise immunity, the signal contains
a lot of power. That means it is very loud, and
its spectral composition is guaranteed to turn your speakers into
a long-range acoustic weapon.

Requires [SoX](http://sox.sourceforge.net/).

Original by winytan, brought back to life by Foxy6670

© windytan (Oona Räisänen)

ISC license

# NanoSynth

A miniature tone generator written in Ruby, intended to show how to create a minimal Ruby program that generates sound.

For a detailed description of how it works, check out this blog post: [http://www.joelstrait.com/blog/2014/6/14/nanosynth_create_sound_with_ruby](http://www.joelstrait.com/blog/2014/6/14/nanosynth_create_sound_with_ruby)

# Installation

* Download `nanosynth.rb`
* Install the [WaveFile gem](http://wavefilegem.com): `gem install wavefile`
* need to install 0.6.0 version, select 0.6.0 version, then copy "INSTALL" command in right row
* gem install wavefile -v 0.6.0

# Example Usage

NanoSynth expects 3 arguments: the waveform, frequency, and amplitude. It will then generate 1 second of sound and write it to a file called `mysound.wav` in the current directory.

For example:

    ruby nanosynth.rb square 440.0 0.2

The command above will generate a square wave of 440Hz, at 20% full volume, and write it to `mysound.wav` in the current directory.

The waveform can be one of `sine`, `square`, `saw`, `triangle`, or `noise`.

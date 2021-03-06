## 0.2.7 2010-11-16

* Add documentation for an overview of the Bzip2 module
* Document the class methods on Bzip2 and get them to show up in yarddoc
* Remove the ConfigError class because searching for it showed no instances of its usage
* Add a Usage section to the README and a bit about adding it to a Gemfile
* Improve the reader_spec.rb by making it more resilient in lots of places and a bit more descriptive/terse in
* Add a lot more documentation for the Reader class and also touch up the Writer class a bit
* Make the Writer specs more descriptive by giving them some doc strings.
* Wrap up documentation of the Bzip2::Writer class.
* Add lib/bzip2-ruby.rb so it's not always necessary to specify to require 'bzip2' in Gemfiles and such
* Start documenting the Bzip2::Writer class
* Fix a few compiler warnings
* Removed some dead code
* Fix for ruby 1.9 compatibility.
* Fix segfault when exiting in ruby 1.9
* Follow the newer conventions of rspec
* Migrate to using Bundler instead of Jeweler
* use malloc/free instead of ruby_xmalloc/ruby_xfree

## 0.2.6 2009-10-6

* Updated to support Ruby 1.8.5

## 0.2.5 2009-06-07

* initial conversion of original tests over to rspec

## 0.2.4 2009-05-02

* renamed BZ2 module/namespace to Bzip2

## 0.2.3 2009-05-02

* renamed gem to bzip2-ruby from bz2
* initial conversion to jeweler
* bundling gemspec
* README and file structure organization updates
* updated Init_*() ruby initializer function to match new gem name

## 0.2.2 2008-12-22

* 1 major enhancement:
  * Gemify bz2 library from http://moulon.inra.fr/ruby/bz2.html
  * All credit goes to Guy Decoux <ts@moulon.inra.fr>

## 0.2.1

* replaced rb_proc_new() with bz_proc_new() for 1.6
(Thanks "Akinori MUSHA" <knu@iDaemons.org>)

## 0.1.9

* corrected BZ_FINISH_OK (Thanks Rudi Cilibrasi <Rudi.Cilibrasi@cwi.nl>)

## 0.1.6

* adapted for 1.8.0 (ihi)
* modified ::new
* BZ2::Writer#finish (same than #flush)

## 0.1.5

* corrected extconf.rb
* added close!
* replaced close(false) by #finish
* corrected #flush

## 0.1.4

* corrected bz_iv
* #to_io
* corrected ::Reader#close

## 0.1.3

* corrected #lineno
* corrected ::Writer::new(nil)
* taint result

## 0.1.2

* better (???) interface for #read
* finalize for objects which respond to #closed?

## 0.1.1

* better interface for T_FILE
* corrected bug with gc (buf)
* Reader#lineno, Reader#lineno=, Reader#ungets
* corrected Reader#unused
* taint check in #initialize
* BZ2::bzip2, BZ2::bunzip2
* too many exceptions
Additional real/virtual attribute dirty tracking independent of ActiveRecords

This a wrap up of some legacy code so it can be refactored/tested, not recommeneded for use yet :)

Install
=======

    gem install dirty_delta

Usage
=====

    class User < ActiveRecord::Base
      include DirtyDelta::Extension
      dirty_delta :columns => [:name], :attributes => [:full_name]
    end

Author
======
[Michael Grosser](http://grosser.it)<br/>
michael@grosser.it<br/>
License: MIT<br/>
[![Build Status](https://secure.travis-ci.org/grosser/dirty_delta.png)](http://travis-ci.org/grosser/dirty_delta)

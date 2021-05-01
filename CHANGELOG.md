# Changelog

### v2.9.0

* Resolve Fixnum deprecation warnings with Ruby 2.4+

### v2.8.1

* Create shared CLI module

### v2.8.0

* Add new diff-* executables for matching JSON & CSV files on the command line

### v2.7.1

* Use `failure_message` from RSpec matchers in diff output. (denyago)

### v2.7.0

* Add rspec custom matcher `be_json_matching` for Rspec v2.x & v3.x

### v2.6.0

* Add rspec custom matcher `be_matching` for RSpec v3.x

### v2.5.0

* Add rspec custom matcher `be_matching`

### v2.4.1

* BUGFIX match values where their classes are different but one is a subclass of the other

### v2.4.0

* Add class configuration of Difference from a block

### v2.3.3

* Allow HTML output using `:html_output=>true` option

### v2.3.2

  Summarize `Hash` and `Array` output in diff with `"..."`
```
  eg.
  - [...]+ {...}
```

### v2.2.3

* set color_enabled/color_scheme on the class

  (ie. so it can be used by default)

### v2.2.2

* BUGFIX for `AllMatcher`

  - return a diff instead of raising an exception
  - (raising an exception was a bad idea as it blew up the entire match
     when used in conjuction with an or-matcher, or embedded into other
     matchers)

### v2.2.1

* AllMatcher also accepts a size (`Fixnum` or `Range`)

### v2.2.0

* Added Matcher and AllMatcher
  - Matcher returns the *closest* diff.
* Added `:min`, `:max` args to `AllMatcher` and `:optional_keys` to `Matcher`
* Added range matcher

### v2.0.0

* Remove `:verbose` option

  More often than not users want this as the default.

### v1.0.1

* BUGFIX for ruby 1.8.7

### v1.0.0

* initial release (as a gem in the wild)

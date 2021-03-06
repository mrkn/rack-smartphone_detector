# Rack::SmartphoneDetector [![Build Status](https://secure.travis-ci.org/ihara2525/rack-smartphone_detector.png?branch=master)](http://travis-ci.org/ihara2525/rack-smartphone_detector)

It's a very simple Rack middleware which detect the request comes from smartphones (iPhone/iPad/Android/Android Tablet/Windows Phone).  

You can use #from_smartphone? to detect the request.

```ruby
request.from_smartphone? # true if it comes from such devices
```

or, use methods for each devices.

```ruby
request.from_iphone?         # true if it comes from iphone
request.from_ipad?           # true if it comes from ipad
request.from_android?        # true if it comes from android mobile
request.from_android_tablet? # true if it comes from android tablet
request.from_windows_phone?  # true if it comes from windows phone
```

What this middleware does is just matching HTTP_USER_AGENT with identifier of smartphones.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'rack-smartphone_detector'
```

And then execute:

```
$ bundle
```

Or install it yourself as:

```
$ gem install rack-smartphone_detector
```

## Usage with Rails 3

If you are using Rails 3, you have no futher steps to do.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

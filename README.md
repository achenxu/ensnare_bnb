# EnsnareBnb

EnsnareBnb is a simple scraper designed to get listings from AirBNB in JSON
format.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'ensnare_bnb'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install ensnare_bnb

## Usage



### United States

To find a city in the US, only city and country are required. To prevent inaccurate results for common city names (for example, Dover or St. Louis), provide the state name as well.

```
EnsareBnb.find_locations(
	city: 'Seattle', 
	state: 'WA', 
	country: 'United States')
```
=> Returns JSON results of all AirBNB listings found in Seattle, WA.

#### Optional Fields
:start\_date, :end\_date
:guests, :price\_min, :price\_max, :max_pages

--

### Contributing

1. Fork it ( https://github.com/[my-github-username]/ensnare_bnb/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

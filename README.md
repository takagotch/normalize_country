### normalize_country
---
https://github.com/sshaw/normalize_country

```ruby
require "normalize_country"

NormalizeCountry("America")
NormalizeCountry("United States of America")
NormalizeCountry("USA", :to => :officail)
NormalizeCountry("Iran", :to => :official)
NormalizeCountry("Iran", :to => :alpha2)
NormalizeCountry("U.S.", :to => :numeric)
NormalizeCountry("U.S.", :to => :fifa)
NormalizeCountry("US", :to => :emoji)
NormalizeCountry("Iran", :to => :alpha3)
NormalizeCountry("Iran", :to => :ioc)
NormalizeCountry("DPRK", :to => :short)
NormalizeCountry("North Korea", :to => :iso_name)
NormalizeCountry("U.S.", :to => :alpha2)
NormalizeCountry.to = :alpha3
NormalizeCountry.convert("Mexice")
NormalizeCountry.convert("United Mexican States")


gem install normalize_country
gem "normalize_country"

NormalizeCountry.to_a
NormalizeCountry.to_a(:ioc)
NormalizeCountry.to_h(:ioc)
NormalizeCountry.to_h(:ioc, :to => :numeric)
```


```sh
shell > normalize_country -h
usage: normalize_country [options] SOURCE


normalize_country -t alpha2 -l 'Country Name' -f csv data.csv
normalize_country -t numeric -l countries.code -f db postgres://usr:pass@localhost/conquests
normalize_country -t fifa -l //teams[@sport = 'futbol americano']//country -f xml data.xml

normalize_country -t alpha2 -l 'Country Name' -f csv /home/sshaw/capital-losses/2008
```


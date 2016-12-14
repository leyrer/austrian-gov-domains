Austrian Government Domains
=========================

An incomplete listing of austrian government domains (and the code for the scraper used to build the list).

We try to use the same format as the [US GSA](https://github.com/GSA/data) ([example](https://github.com/GSA/data/blob/e0de99db0e1367e304043e88dbd4da8f391774be/dotgov-domains/2016-01-19-full.csv)), so the CSV file has a header of `Domain Name,Domain Type,Agency,City,State` and currently contains government agencies and cities.

## Variants

If you only want a subset of the available data, variants filtered by `Domain Type` are provided:

* [`data/domains.csv`](data/domains.csv) contains everything

## Why?

There currently isn't a publicly available directory of all the government sites in Austria and I needed one for "an art project". This is by no means an official or a complete list. 


## What can I do with it?

* Plug the CSV into [18F/domain-scan](https://github.com/18F/domain-scan) to get more data (like HTTPS support) about the domains
* Check the IPv6 reachability
* Test if the sites are reachable even without the `www.` subdomain
* ...?


## How to update

The list is populated by scrapers and static files and merged by a makefile.
To run the process yourself, checkout this repository and run:

    make

After everything ran, you can look into `data/domains.csv`.


## Scrapers and Sources


## Contributing

I'd love to have some help with this! Please feel free to [create an issue](https://github.com/leyrer/austrian-gov-domains/issues) or [submit a pull request](https://github.com/leyrer/austrian-gov-domains/pulls) if you notice something that can be better. Specifically, suggesting additional pages we can scrape and domains that are either not found or have incorrect organization names associated with them would be very helpful.

## Ideas

* scrape even more domains

## Thanks

Thanks to [@robbi5](https://github.com/robbi5) for the [German Government Domains](https://github.com/robbi5/german-gov-domains) and [@esonderegger](https://github.com/esonderegger) for the [dotmil domains project](https://github.com/esonderegger/dotmil-domains) that served as an template for this repo.

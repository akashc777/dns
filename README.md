<img width="150" src="https://akash.page/assets/images/logo.svg" />

dns.akash.page is a DNS server that takes creative liberties with the DNS protocol to offer handy utilities and services that are easily accessible via the command line.

For docs, visit [**www.dns.akash.page**](https://www.dns.akash.page)

## Sample commands

```shell
dig help @dns.akash.page

dig mumbai.time @dns.akash.page

dig 2023-05-28T14:00-bengaluru-berlin/de.time @dns.akash.page

dig newyork.weather @dns.akash.page

dig 42km-mi.unit @dns.akash.page

dig 100USD-INR.fx @dns.akash.page

dig ip @dns.akash.page

dig 987654321.words @dns.akash.page

dig pi @dns.akash.page

dig 100dec-hex.base @dns.akash.page

dig fun.dict @dns.akash.page

dig A12.9352,77.6245/12.9698,77.7500.aerial @dns.akash.page
```

## Running locally

- Clone the repo
- Copy `config.sample.toml` to `config.toml` and edit the config
- Make sure you have a copy of the `cities15000.txt` file at the root of this directory (instructions are in the `config.sample.toml` file)
- Make sure to download the `wordnet` from [Wordnet website](https://wordnetcode.princeton.edu/3.0/WNdb-3.0.tar.gz).(more instructions are in the `config.sample.toml` file)
- Extract the tarball and rename extracted the directory to `wordnet`
- Run `make build` to build the binary and then run `./dnstoys.bin`

## Others

- [DnsToys.NET](https://github.com/fatihdgn/DnsToys.NET) - A .net client library for the service.

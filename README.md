# cymru-lookup

The `cymru-lookup` tool is a bash-wrapper tool around the [GNU version of netcat](http://netcat.sourceforge.net/)
and the ip-to-asn lookup service provided by cymru, described here
 - https://www.team-cymru.com/IP-ASN-mapping.html#whois

The last octet of (IPv4) input addresses is stripped and thus grouped into their 
respective /24 netblock, this is bacause the smallest possible public netblock 
via external-BGP is a /24.


## Project
* [github.com/ndejong/cymru-lookup](https://github.com/ndejong/cymru-lookup)

## Usage
```
Usage: cymru-lookup <filename>
 <filename> must be a flat file containing ip-addresses only.
 Duplicate address values are counted and shown in the cymru output
 comment column shown as the 'addr-count:' value.
```

****

## Authors
[Nicholas de Jong](https://nicholasdejong.com)

## License
BSD-2-Clause - see LICENSE file for full details.

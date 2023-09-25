# public-resolvers

This is an extensive list of public DNS resolvers supporting the
DNSCrypt and DNS-over-HTTP2 protocols.

This list is maintained by Frank Denis <j @ dnscrypt [.] info>

Warning: it includes servers that may censor content, servers that don't
verify DNSSEC records, and servers that will collect and monetize your
queries.

Adjust the `require_*` options in dnscrypt-proxy to filter that list
according to your needs.

To use that list, add this to the `[sources]` section of your
`dnscrypt-proxy.toml` configuration file:

    [sources.'public-resolvers']
    urls = ['https://raw.githubusercontent.com/gophc/dnscrypt-resolvers/master/vk/public-resolvers.md', 'https://raw.githubusercontent.com/gophc/dnscrypt-resolvers/master/vk/public-resolvers.md']
    minisign_key = 'RWQz9CWovHe/e8swTDimYy+8haDVhef71mzx70/clJCQyX3+B+1fh8fT'
    cache_file = 'public-resolvers.md'

--

## alidns-doh

A public DNS resolver that supports DoH/DoT in mainland China, provided by Alibaba-Cloud.

Warning: GFW filtering rules are applied by that resolver.

Homepage: https://alidns.com/

sdns://AgAAAAAAAAAACTIyMy41LjUuNSCY49XlNq8pWM0vfxT3BO9KJ20l4zzWXy5l9eTycnwTMA5kbnMuYWxpZG5zLmNvbQovZG5zLXF1ZXJ5


## cloudflare

Cloudflare DNS (anycast) - aka 1.1.1.1 / 1.0.0.1

sdns://AgcAAAAAAAAABzEuMC4wLjEAEmRucy5jbG91ZGZsYXJlLmNvbQovZG5zLXF1ZXJ5


## cloudflare-ipv6

Cloudflare DNS over IPv6 (anycast)

sdns://AgcAAAAAAAAAFlsyNjA2OjQ3MDA6NDcwMDo6MTExMV0AIDFkb3QxZG90MWRvdDEuY2xvdWRmbGFyZS1kbnMuY29tCi9kbnMtcXVlcnk


## dnscry.pt-hongkong-ipv4

DNSCry.pt Hong Kong - no filter, no logs, DNSSEC support (IPv4 server)

https://www.dnscry.pt

sdns://AQcAAAAAAAAACzg5LjIxMy4wLjI2IDLd7cTU2bJRmCo3O9PZ4ReJKVbbj9lP1KerGmf2Le81GTIuZG5zY3J5cHQtY2VydC5kbnNjcnkucHQ


## dnscry.pt-hongkong-ipv6

DNSCry.pt Hong Kong - no filter, no logs, DNSSEC support (IPv6 server)

https://www.dnscry.pt

sdns://AQcAAAAAAAAAFFsyYTEzOjgyYzE6ODUwYTo6YjddIDLd7cTU2bJRmCo3O9PZ4ReJKVbbj9lP1KerGmf2Le81GTIuZG5zY3J5cHQtY2VydC5kbnNjcnkucHQ


## dnspod

A public DNS resolver that supports DoH/DoT in mainland China, provided by dnspod/Tencent-cloud.

Warning: GFW filtering rules are applied by that resolver.

Homepage: https://dnspod.cn/

sdns://AgAAAAAAAAAACjEuMTIuMTIuMTIgj0tzmXxLBOpQ_q-pGiQx1CvKa1TCO8-du_VyJJOU4QwHZG9oLnB1YgovZG5zLXF1ZXJ5


## google

Google DNS (anycast)

sdns://AgUAAAAAAAAABzguOC44LjigHvYkz_9ea9O63fP92_3qVlRn43cpncfuZnUWbzAMwbmgdoAkR6AZkxo_AEMExT_cbBssN43Evo9zs5_ZyWnftEUgalBisNF41VbxY7E7Gw8ZQ10CWIKRzHVYnf7m6xHI1cMKZG5zLmdvb2dsZQovZG5zLXF1ZXJ5


## google-ipv6

Google DNS (anycast)

sdns://AgUAAAAAAAAAFlsyMDAxOjQ4NjA6NDg2MDo6ODg4OF2gHvYkz_9ea9O63fP92_3qVlRn43cpncfuZnUWbzAMwbmgdoAkR6AZkxo_AEMExT_cbBssN43Evo9zs5_ZyWnftEUgalBisNF41VbxY7E7Gw8ZQ10CWIKRzHVYnf7m6xHI1cMKZG5zLmdvb2dsZQovZG5zLXF1ZXJ5


## qihoo360-doh

DoH server runned by Qihoo 360, has logs, supports DNSSEC. GFW filtering rules are applied.

Homepage: https://sdns.360.net/

sdns://AgEAAAAAAAAAACBZPi1Jp0AjVVUmrvm3QisZ5bixZzkbbe5e0pKxyiOnTApkb2guMzYwLmNuCi9kbnMtcXVlcnk


## yandex

Yandex public DNS server (anycast)

sdns://AQQAAAAAAAAAEDc3Ljg4LjguNzg6MTUzNTMg04TAccn3RmKvKszVe13MlxTUB7atNgHhrtwG1W1JYyciMi5kbnNjcnlwdC1jZXJ0LmJyb3dzZXIueWFuZGV4Lm5ldA


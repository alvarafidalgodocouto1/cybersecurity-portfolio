# Pre Security — How the Web Works

## Module overview

This module covers DNS, HTTP, how websites work, and how the different components fit together when a browser requests a resource.

## 1. DNS in detail

DNS helps translate domain names into records used by clients and services. Common record types include A (IPv4), AAAA (IPv6), CNAME (alias), MX (mail exchange), and TXT (text records).

Example commands:

```bash
nslookup example.com
dig example.com
```

Results may be affected by caching, resolver configuration, and the authoritative records.

## 2. HTTP in detail

HTTP is a request-response protocol. Common methods include:
- `GET`: retrieve a resource
- `POST`: submit data for processing
- `PUT`: create or replace a resource, depending on the API
- `DELETE`: request deletion

Status-code families:
- `2xx`: success
- `3xx`: redirection
- `4xx`: client/request issue
- `5xx`: server-side error

HTTPS protects HTTP communication using TLS. A `200 OK` indicates that the HTTP request succeeded; it does not prove the content is safe or should have been public.

## 3. How websites work

A website can involve a browser, DNS resolver, CDN, load balancer, web server, application server, database, and third-party services. The browser may request multiple resources to render a page.

URLs can contain a scheme, hostname, port, path, query, and fragment.

## 4. Putting it all together

A simplified request flow:
1. The user enters a URL.
2. DNS resolution finds an address.
3. The client establishes the necessary connection.
4. TLS may secure the connection for HTTPS.
5. The browser sends an HTTP request.
6. The server responds with status, headers, and content.
7. The browser processes the response and may request more resources.

## Web logs

Access logs may record client address, timestamp, request path, status code, response size, and other fields depending on configuration. These records support troubleshooting and security investigations.

An IP address in a log may belong to a proxy or gateway, not the original person. A single request does not prove malicious intent.

## Key takeaways

- DNS supports name resolution.
- HTTP uses requests and responses; HTTPS adds TLS protection.
- Websites often depend on multiple systems and services.
- Web logs provide useful evidence but must be interpreted in context.

## Rooms covered by this module

- DNS in Detail
- HTTP in Detail
- How Websites Work
- Putting it all together

## Official reference

[TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity)

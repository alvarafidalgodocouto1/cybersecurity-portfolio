# Hidden File Discovery and HTTP File Retrieval

## Summary

The supplied lab debrief reports that a hidden file named `.flag.txt` was retrieved using `wget` over HTTP.

## Method reported

1. Identified the resource path as `/.flag.txt`.
2. Requested the resource over HTTP with `wget`.
3. The debrief reported successful retrieval and HTTP `200` status.

## Concepts

- Dot-prefixed names are typically hidden from ordinary directory listings on Unix-like systems.
- `wget` retrieves resources from URLs.
- HTTP GET is commonly used to request a resource.
- HTTP `200 OK` indicates that the request succeeded, not that the content should necessarily have been publicly accessible.

## Security relevance

A hidden filename is not an access-control mechanism. Resources containing sensitive information need appropriate server configuration and authorisation controls.

## Evidence note

This write-up reflects the supplied debrief from TryHackMe.

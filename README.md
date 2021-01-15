# Go-Concurrency
Some higher function snippets to make go code in concurrency much easy


# Some big questions

## ALL or ANY

## TIMEOUT (https://github.com/golang/go/wiki/Timeouts)
To abandon synchronous calls that run too long, use the select statement with time.After.

## Rate Limiting (https://github.com/golang/go/wiki/RateLimiting)
To limit the rate of operations per unit time, use a [time.Ticker](http://golang.org/pkg/time/#NewTicker).
This works well for rates up to tens of operations per second.
For higher rates, prefer a token bucket rate limiter such as [golang.org/x/time/rate.Limiter](https://godoc.org/golang.org/x/time/rate) (also search godoc.org for
[rate limit](http://godoc.org/?q=rate+limit)).

# Snippets

go_all_with_timeout([]func, timeout)

go_any_with_timeout([]func, timeout)

go_



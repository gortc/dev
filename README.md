# dev

Hi, here you can find development info about [gortc](https://gortc.io) project, it's goals,
principles, etc. Feel free to ask anything via issues.

## Original author
I'm Aleksandr Razumov ([ernado](https://github.com/ernado)), full time go developer with commercial experience
starting from 2014 (and non-go from 2011) and currently working at
German company not related to project.

## Goals
* Create tools and libraries for NAT traversal and ICE
* Make them safe, reliable, fast, stable and simple to use and extend
* Make them useful (extensible and flexible) for enterprise while staying open source
* Don't be hype and PR driven, popularity and stars count are not appropriate metrics

## Principles
* High and rigorous standards for core packages:
    * Minimum (none is ideal) 3-rd party deps
    * Greater than 90% test coverage
    * Benchmarks to track performance
    * Zero-allocation in hot paths
    * Tests for zero allocation
    * [Fuzz](https://en.wikipedia.org/wiki/Fuzzing)-testing
    * Integration (functional, e2e) tests
    * Static checks (linters)
    * Test with `-race` flag
    * Run ci tests with `go tip` daily
    * API backward compatibility [check](https://github.com/gortc/api)
* Mostly bottom-up development with feedback loop
* Decoupling and abstraction layer isolation
* Conscious architecture design with clear goals
* Follow [effective go](https://golang.org/doc/effective_go.html) and [CodeReviewComments](https://github.com/golang/go/wiki/CodeReviewComments)
* Follow [semver](https://semver.org/) with `v` prefix for tags, like `v1.2.0`
* Use RFC wording whenever possible but not at the expense of idiomaticity
* Manage dependencies with [dep](https://github.com/golang/dep) until vgo stabilizes and will allow
reproducible builds without net connectivity

## Contributors
Thanks so much for contribution to the gortc project:
* [backkem](https://github.com/backkem)

Current development status for tech stack for NAT traversal and WebRTC interoperation in golang.

rfc | name  | status | build | description
---|-------|--------|-------|----
[RFC4566](https://tools.ietf.org/html/rfc4566) | [SDP](http://github.com/gortc/sdp)    | ![status](https://img.shields.io/badge/status-beta-green.svg) | [![Build Status](https://travis-ci.org/gortc/sdp.svg?branch=master)](https://travis-ci.org/gortc/sdp) | SDP decoding and encoding
[RFC5389](https://tools.ietf.org/html/rfc5389) | [STUN](http://github.com/gortc/stun)  | ![status](https://img.shields.io/badge/status-beta-green.svg)  | [![Build Status](https://travis-ci.org/gortc/stun.svg)](https://travis-ci.org/gortc/stun) | STUN server and client 
[RFC5766](https://tools.ietf.org/html/rfc5766) | [TURN](http://github.com/gortc/turn)  | ![status](https://img.shields.io/badge/status-beta-green.svg) | [![Build Status](https://travis-ci.org/gortc/turn.svg)](https://travis-ci.org/gortc/turn) | STUN + Tunnels
[RFC5245](https://tools.ietf.org/html/rfc5245) | [ICE](http://github.com/gortc/ice)    | ![status](https://img.shields.io/badge/status-dev-blue.svg)  | [![Build Status](https://travis-ci.org/gortc/ice.svg)](https://travis-ci.org/gortc/ice) | Uses STUN and TURN for TRAVERSAL 
[RFC6347](https://tools.ietf.org/html/rfc6347) | [DTLS](http://github.com/gortc/dtls)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/gortc/dtls.svg)](https://travis-ci.org/gortc/dtls) | Datagram Transport Layer Security Version 1.2
[RFC4960](https://tools.ietf.org/html/rfc4960) | [SCTP](http://github.com/gortc/sctp)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/gortc/sctp.svg)](https://travis-ci.org/gortc/sctp) | Stream Control Transmission Protocol
[WebRTC](https://tools.ietf.org/html/draft-ietf-rtcweb-overview) | [RTC](http://github.com/gortc/rtc)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/gortc/rtc.svg)](https://travis-ci.org/gortc/rtc) | WebRTC

So far **25K** SLOC and **230+** RFC pages implemented as go code.

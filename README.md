# dev

Hi, here you can find development info about [gortc](https://gortc.io) project, it's goals,
principles, etc. Feel free to ask anything via issues.

## Original author
I am Aleksandr Razumov, full time go developer with commercial experience
starting from 2014 (and non-go from 2011) and currently working in
German company not related to that project.

## Goals
* Create tools and libraries for NAT traversal and ICE
* Make them safe, reliable, fast, stable and simple to use
* Don't be hype and PR driven
* Make them useful for enterprise while staying open

## Principles
* Bottom-up development with feedback loop
* High and rigorous standards for core packages:
    * Minimum (none is ideal) 3-rd party deps
    * Greater than 90% test coverage
    * Benchmarks to track performance
    * Zero-allocation in hot paths
    * Tests for zero allocation
    * Fuzz-testing
    * Integration (functional, e2e) tests
    * Static checks (linters)
* Decoupling and abstraction layers
* Conscious architecture design with clear goals
* Follow [effective go](https://golang.org/doc/effective_go.html) and [CodeReviewComments](https://github.com/golang/go/wiki/CodeReviewComments)

## Contributors
Thanks so much for contribution to the development:
* [backkem](https://github.com/backkem)

Current development status for tech stack for NAT traversal and WebRTC interoperation in golang.

rfc | name  | status | build | description
---|-------|--------|-------|----
[RFC4566](https://tools.ietf.org/html/rfc4566) | [SDP](http://github.com/gortc/sdp)    | ![status](https://img.shields.io/badge/status-alpha-green.svg)  | [![Build Status](https://travis-ci.org/gortc/sdp.svg?branch=master)](https://travis-ci.org/gortc/sdp) | SDP decoding and encoding
[RFC5389](https://tools.ietf.org/html/rfc5389) | [STUN](http://github.com/gortc/stun)  | ![status](https://img.shields.io/badge/status-beta-green.svg)  | [![Build Status](https://travis-ci.org/gortc/stun.svg)](https://travis-ci.org/gortc/stun) | STUN server and client 
[RFC5766](https://tools.ietf.org/html/rfc5766) | [TURN](http://github.com/gortc/turn)  | ![status](https://img.shields.io/badge/status-dev-blue.svg) | [![Build Status](https://travis-ci.org/gortc/turn.svg)](https://travis-ci.org/gortc/turn) | STUN + Tunnels
[RFC5245](https://tools.ietf.org/html/rfc5245) | [ICE](http://github.com/gortc/ice)    | ![status](https://img.shields.io/badge/status-dev-blue.svg)  | [![Build Status](https://travis-ci.org/gortc/ice.svg)](https://travis-ci.org/gortc/ice) | Uses STUN and TURN for TRAVERSAL 
[RFC6347](https://tools.ietf.org/html/rfc6347) | [DTLS](http://github.com/gortc/dtls)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/gortc/dtls.svg)](https://travis-ci.org/gortc/dtls) | Datagram Transport Layer Security Version 1.2
[RFC4960](https://tools.ietf.org/html/rfc4960) | [SCTP](http://github.com/gortc/sctp)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/gortc/sctp.svg)](https://travis-ci.org/gortc/sctp) | Stream Control Transmission Protocol
[WebRTC](https://tools.ietf.org/html/draft-ietf-rtcweb-overview) | [RTC](http://github.com/gortc/rtc)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/gortc/rtc.svg)](https://travis-ci.org/gortc/rtc) | WebRTC

So far **17449** SLOC and **230+** RFC pages implemented as go code.

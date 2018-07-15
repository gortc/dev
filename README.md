# dev
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

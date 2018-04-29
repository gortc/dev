# tech-status
Current status for tech stack for NAT traversal and WebRTC interoperation in golang


rfc | name  | status | build | description
---|-------|--------|-------|----
[rfc4566](https://tools.ietf.org/html/rfc4566) | [sdp](http://github.com/gortc/sdp)    | ![status](https://img.shields.io/badge/status-alpha-green.svg)  | [![Build Status](https://travis-ci.org/gortc/sdp.svg?branch=master)](https://travis-ci.org/gortc/sdp) | SDP decoding and encoding
[rfc5389](https://tools.ietf.org/html/rfc5389) | [stun](http://github.com/gortc/stun)  | ![status](https://img.shields.io/badge/status-beta-green.svg)  | [![Build Status](https://travis-ci.org/gortc/stun.svg)](https://travis-ci.org/gortc/stun) | STUN server and client 
[rfc5766](https://tools.ietf.org/html/rfc5766) | [turn](http://github.com/gortc/turn)  | ![status](https://img.shields.io/badge/status-dev-blue.svg) | [![Build Status](https://travis-ci.org/gortc/turn.svg)](https://travis-ci.org/gortc/turn) | STUN + Tunnels
[rfc5245](https://tools.ietf.org/html/rfc5245) | [ice](http://github.com/ernado/ice)    | ![status](https://img.shields.io/badge/status-dev-blue.svg)  | [![Build Status](https://travis-ci.org/ernado/ice.svg)](https://travis-ci.org/ernado/ice) | Uses STUN and TURN for TRAVERSAL 
[rfc6347](https://tools.ietf.org/html/rfc6347) | [dtls](http://github.com/ernado/dtls)  | ![status](https://img.shields.io/badge/status-research-orange.svg)  | [![Build Status](https://travis-ci.org/ernado/dtls.svg)](https://travis-ci.org/ernado/dtls) | DTLS

So far **9392** SLOC written and **230+** RFC pages implemented as go code.

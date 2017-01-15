# tech-status
Current status for tech stack for NAT traversal and WebRTC interoperation in golang


rfc | name  | status | build | description
---|-------|--------|-------|----
[rfc4566](https://tools.ietf.org/html/rfc4566) | [sdp](http://github.com/ernado/sdp)   | ![status](https://img.shields.io/badge/status-alpha-green.svg)  | [![Build Status](https://travis-ci.org/ernado/sdp.svg?branch=master)](https://travis-ci.org/ernado/sdp) | SDP decoding and encoding
[rfc5389](https://tools.ietf.org/html/rfc5389) | [stun](http://github.com/ernado/stun)  | ![status](https://img.shields.io/badge/status-alpha-green.svg)  | [![Build Status](https://travis-ci.org/ernado/stun.svg)](https://travis-ci.org/ernado/stun) | STUN server and client 
[rfc5766](https://tools.ietf.org/html/rfc5766) | turn  | ![status](https://img.shields.io/badge/status-research-lightgrey.svg)  | ![status](https://img.shields.io/badge/build-unknown-lightgrey.svg) | STUN + Tunnels
[rfc5245](https://tools.ietf.org/html/rfc5245) | [ice](http://github.com/ernado/ice)   | ![status](https://img.shields.io/badge/status-dev-blue.svg)  | [![Build Status](https://travis-ci.org/ernado/ice.svg)](https://travis-ci.org/ernado/ice) | Uses STUN and TURN for TRAVERSAL 

So far **4607** SLOC written and **230+** RFC pages implemented as go code.

![logo](docs/logo.png "logo")

[![NetflixOSS Lifecycle](https://img.shields.io/osslifecycle/Netflix/chaosmonkey.svg)](OSSMETADATA) [![Build Status][travis-badge]][travis] [![GoDoc][godoc-badge]][godoc] [![GoReportCard][report-badge]][report]

[travis-badge]: https://travis-ci.org/Netflix/chaosmonkey.svg?branch=master
[travis]: https://travis-ci.org/Netflix/chaosmonkey
[godoc-badge]: https://godoc.org/github.com/gaofanmichael/chaosmonkey?status.svg
[godoc]: https://godoc.org/github.com/gaofanmichael/chaosmonkey
[report-badge]: https://goreportcard.com/badge/github.com/gaofanmichael/chaosmonkey
[report]: https://goreportcard.com/report/github.com/gaofanmichael/chaosmonkey

Chaos Monkey randomly terminates virtual machine instances and containers that
run inside of your production environment. Exposing engineers to
failures more frequently incentivizes them to build resilient services.

See the [documentation][docs] for info on how to use Chaos Monkey.

Chaos Monkey is an example of a tool that follows the
[Principles of Chaos Engineering][PoC].

[PoC]: http://principlesofchaos.org/

### Requirements

This version of Chaos Monkey is fully integrated with [Spinnaker], the
continuous delivery platform that we use at Netflix. You must be managing your
apps with Spinnaker to use Chaos Monkey to terminate instances.

Chaos Monkey should work with any backend that Spinnaker supports (AWS, GCP,
Azure, Kubernetes, Cloud Foundry). It has been tested with AWS and Kubernetes.

### Install locally

To install the Chaos Monkey binary on your local machine:

```
go get github.com/gaofanmichael/chaosmonkey/cmd/chaosmonkey
```

### How to deploy

See the [docs] for instructions on how to configure and deploy Chaos Monkey.

### Support

[Simian Army Google group](http://groups.google.com/group/simianarmy-users).

[Spinnaker]: http://www.spinnaker.io/
[docs]: https://netflix.github.io/chaosmonkey

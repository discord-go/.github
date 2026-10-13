<p align="center">
  <img src="https://raw.githubusercontent.com/discord-go/discord.go/main/docs/public/logo.svg" alt="discord.go" width="180">
</p>

<h1 align="center">discord.go</h1>

<p align="center">
  A typed Go library for building Discord applications.<br>
  Low-level Discord API foundation and high-level bot facade.
</p>

<p align="center">
  <a href="https://github.com/discord-go/discord.go/actions/workflows/ci.yml"><img src="https://github.com/discord-go/discord.go/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <a href="https://pkg.go.dev/github.com/discord-go/discord.go"><img src="https://pkg.go.dev/badge/github.com/discord-go/discord.go.svg" alt="Go Reference"></a>
  <a href="https://goreportcard.com/report/github.com/discord-go/discord.go"><img src="https://goreportcard.com/badge/github.com/discord-go/discord.go" alt="Go Report Card"></a>
  <img src="https://img.shields.io/badge/Discord%20API-v10-5865f2.svg" alt="Discord API v10">
  <img src="https://img.shields.io/badge/Go-1.26+-00add8.svg" alt="Go Version">
  <img src="https://img.shields.io/badge/license-Apache--2.0-blue.svg" alt="License">
</p>

---

## Projects

### [discord.go](https://github.com/discord-go/discord.go)

A typed Discord API client and bot framework for building Discord bots and
applications in Go.

- **Two-layer architecture.** A typed low-level protocol/REST foundation and a
  high-level `bot` facade with commands, middleware, collectors, and lifecycle
  management. Use the facade for application code, drop to the low-level API
  for protocol work.
- **Gateway v10 with sharding.** Dispatch, heartbeat, reconnect, resume,
  zlib-stream compression, multi-shard support with concurrency buckets, and
  automatic shard count detection.
- **Voice with DAVE.** WebSocket, UDP, RTP, AES-256-GCM transport encryption,
  Opus frame handling, and DAVE/MLS end-to-end encryption support.
- **Components V2.** Full support for Discord's Components V2 message model
  including containers, media galleries, separators, and section components.
- **Typed throughout.** Every REST resource, gateway event, and interaction
  type has a typed Go model. Nullable fields use pointers where omission
  differs from `null`.
- **Production-oriented.** Rate limiting with bucket hashing, invalid-request
  tracking to prevent Cloudflare bans, audit-log reasons, multipart uploads,
  and context-aware cancellation on all REST calls.

```bash
go get github.com/discord-go/discord.go
```

Requires Go 1.26 or newer. The library targets Discord API v10.

## Links

- **Documentation** — [discord-go.github.io/discord.go](https://discord-go.github.io/discord.go/)
- **API reference** — [pkg.go.dev/github.com/discord-go/discord.go](https://pkg.go.dev/github.com/discord-go/discord.go)
- **Releases** — [github.com/discord-go/discord.go/releases](https://github.com/discord-go/discord.go/releases)
- **Contributing** — [CONTRIBUTING.md](https://github.com/discord-go/discord.go/blob/main/CONTRIBUTING.md)

## License

Apache License 2.0 — see [LICENSE](https://github.com/discord-go/discord.go/blob/main/LICENSE).

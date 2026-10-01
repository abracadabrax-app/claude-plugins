# Abracadabrax plugins for Claude

Two plugins that let Claude create media with Abracadabrax. Each one talks to a hosted Abracadabrax MCP server and shows a panel where you check the settings and the credit price before anything is rendered.

| Plugin | Creates | Install |
|---|---|---|
| [Abracadabrax AI Image & Video Generator](abracadabrax-image-video) | Images and short videos from a prompt | `/plugin install abracadabrax-image-video@abracadabrax` |
| [Abracadabrax AI Song & Music Maker](abracadabrax-song-maker) | Songs with vocals, or instrumentals, from lyrics written with Claude | `/plugin install abracadabrax-song-maker@abracadabrax` |

Add this marketplace in Claude Code first:

```
/plugin marketplace add abracadabrax-app/claude-plugins
```

## Accounts and credits

Drafts are free and need no account. Rendering happens in your [Abracadabrax](https://abracadabrax.app) account: Claude asks you to sign in (OAuth 2.1 with PKCE) the first time, and every render shows its credit price before it starts.

All images, videos and songs are produced by generative AI models, and only when you confirm.

## Links

- [How the connectors work](https://abracadabrax.app/mcp)
- [Privacy policy](https://abracadabrax.app/privacy) · [Terms of service](https://abracadabrax.app/terms)
- [Help](https://abracadabrax.app/support)

## License

Released under the MIT license, see [LICENSE](LICENSE). Claude is a product of Anthropic; Abracadabrax is a separate product and this repository is not an Anthropic project.

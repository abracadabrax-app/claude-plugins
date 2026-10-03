# Abracadabrax plugins for Claude

Plugins that let Claude create media with Abracadabrax. Each one talks to a hosted Abracadabrax MCP server and shows a panel where you check the settings and the credit price before anything is rendered.

| Plugin | Creates | Install |
|---|---|---|
| [Abracadabrax AI Image & Video Generator](abracadabrax-image-video) | Images and short videos from a prompt | `/plugin install abracadabrax-image-video@abracadabrax` |
| [Abracadabrax AI Song & Music Maker](abracadabrax-song-maker) | Songs with vocals, or instrumentals, from lyrics written with Claude | `/plugin install abracadabrax-song-maker@abracadabrax` |
| [Abracadabrax AI Video Generator](abracadabrax-ai-video-generator) | Short video clips from a scene description, for YouTube, TikTok, Reels or Shorts | `/plugin install abracadabrax-ai-video-generator@abracadabrax` |
| [Abracadabrax YouTube Thumbnail Maker](abracadabrax-youtube-thumbnail-maker) | 16:9 YouTube thumbnails with a readable headline | `/plugin install abracadabrax-youtube-thumbnail-maker@abracadabrax` |
| [Abracadabrax AI Product Photo Generator](abracadabrax-product-photo-generator) | Product photos: packshots, lifestyle scenes, flat lays, hero banners | `/plugin install abracadabrax-product-photo-generator@abracadabrax` |
| [Abracadabrax Social Media Image & Post Maker](abracadabrax-social-media-image) | Post, story and pin images sized for each platform | `/plugin install abracadabrax-social-media-image@abracadabrax` |
| [Abracadabrax Poster & Flyer Maker](abracadabrax-poster-flyer-maker) | Posters and flyers with the headline and details on the design | `/plugin install abracadabrax-poster-flyer-maker@abracadabrax` |
| [Abracadabrax AI Background Music Generator](abracadabrax-background-music-generator) | Instrumental background music for videos, podcasts, ads and games | `/plugin install abracadabrax-background-music-generator@abracadabrax` |
| [Abracadabrax Birthday Song Maker](abracadabrax-birthday-song-maker) | Personalized birthday songs with the person's name and your lyrics | `/plugin install abracadabrax-birthday-song-maker@abracadabrax` |
| [Abracadabrax Album Cover Art Maker](abracadabrax-album-cover-maker) | Square cover art for albums, singles, EPs, mixtapes and playlists | `/plugin install abracadabrax-album-cover-maker@abracadabrax` |
| [Abracadabrax Coloring Page Maker](abracadabrax-coloring-page-maker) | Printable black-and-white coloring pages for toddlers, kids and adults | `/plugin install abracadabrax-coloring-page-maker@abracadabrax` |
| [Abracadabrax Greeting Card & Invitation Maker](abracadabrax-greeting-card-maker) | Personal greeting cards and invitations with your message printed on them | `/plugin install abracadabrax-greeting-card-maker@abracadabrax` |
| [Abracadabrax Podcast Intro & Jingle Maker](abracadabrax-podcast-jingle-maker) | Short podcast and channel intros: instrumental or a sung tagline with the show's name | `/plugin install abracadabrax-podcast-jingle-maker@abracadabrax` |

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

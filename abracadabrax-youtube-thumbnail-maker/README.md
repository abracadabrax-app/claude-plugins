# Abracadabrax YouTube Thumbnail Maker

Give Claude the topic of your video and a short headline, and get a 16:9 thumbnail designed to stand out in the feed. Abracadabrax renders it with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude what the video is about and, if you want, the 2-6 words to print on the thumbnail.
2. Claude saves a 16:9 draft with the subject, the style, the colors and the image model, and shows its price in credits.
3. You adjust the wording or the look, then ask Claude to render it.
4. Abracadabrax renders the thumbnail and Claude hands you the link to the image.

## Good to know

- **Made by AI.** Every image and video comes from generative AI models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **New designs only.** Putting your own photo or face on a thumbnail needs an upload, which happens in the Abracadabrax workspace, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/youtube-thumbnail-maker/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you render something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_youtube_thumbnail` | Creates a 16:9 draft from the video topic, an optional headline, the main subject, the style and the colors | none, guest allowed |
| `render_media_widget` | Shows a saved draft again in the panel | none |
| `update_media_project` | Applies the changes made in the panel | none |
| `generate_media` | Starts the render after you confirm | charged, sign-in needed |
| `get_media_job` | Reports progress and returns the file link | none, read-only |

## Try asking

- "Thumbnail for my video about baking sourdough bread, headline "24 HOUR SOURDOUGH""
- "A gaming thumbnail for a speedrun world record, neon colors, no text"
- "Minimal tech review thumbnail for a new laptop, headline "WORTH IT?""

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#youtube-thumbnail-maker
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

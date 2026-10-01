# Abracadabrax AI Video Generator

Describe a scene and get a short AI video clip without leaving Claude: a landscape shot for YouTube, a vertical clip for TikTok, Reels or Shorts, or a square loop. Abracadabrax renders it with the credits of your own Abracadabrax account.

## How a request flows

1. You describe what happens in the clip: subject, action, setting, camera movement.
2. Claude saves a draft with the style, the format, the length and the video model (Kling 3.0, Seedance, Sora 2, Veo 3.1), and shows its price in credits.
3. You change anything you like, then ask Claude to render it.
4. Abracadabrax renders the clip and Claude hands you the link to the video file.

## Good to know

- **Made by AI.** Every image and video comes from generative AI models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **Text to video only.** Animating an existing photo or editing a video you already have happens in the Abracadabrax workspace, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/ai-video-generator/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you render something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_ai_video` | Creates a draft from the scene, style, format (landscape, vertical, square), length and video model | none, guest allowed |
| `render_media_widget` | Shows a saved draft again in the panel | none |
| `update_media_project` | Applies the changes made in the panel | none |
| `generate_media` | Starts the render after you confirm | charged, sign-in needed |
| `get_media_job` | Reports progress and returns the file link | none, read-only |

## Try asking

- "Make a 5-second vertical clip of a paper boat sailing down a rainy street, cinematic"
- "A slow drone shot over snowy mountains at sunrise, 16:9, 10 seconds"
- "An anime-style cat jumping between rooftops at night, square format"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#ai-video-generator
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

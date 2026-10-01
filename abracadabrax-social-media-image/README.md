# Abracadabrax Social Media Image & Post Maker

Turn a post idea into an image already sized for the platform where it will run: square and portrait Instagram posts, vertical stories and reel covers, Facebook, LinkedIn and X posts, Pinterest pins. Abracadabrax renders it with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude the platform and what the post is about.
2. Claude saves a draft with the right aspect ratio, any text to print, the style, the colors and the image model, and shows its price in credits.
3. You adjust it, then ask Claude to render it.
4. Abracadabrax renders the image and Claude hands you the link to the file.

## Good to know

- **Made by AI.** Every image and video comes from generative AI models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **New images only.** Editing photos you already have, or adding your logo file, happens in the Abracadabrax workspace, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/social-media-image/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you render something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_social_media_image` | Creates a draft sized for the platform, from the idea, optional text on the image, style and brand colors | none, guest allowed |
| `render_media_widget` | Shows a saved draft again in the panel | none |
| `update_media_project` | Applies the changes made in the panel | none |
| `generate_media` | Starts the render after you confirm | charged, sign-in needed |
| `get_media_job` | Reports progress and returns the file link | none, read-only |

## Try asking

- "Instagram post announcing our autumn menu, warm tones, text "Now serving""
- "Pinterest pin of a cozy reading nook, text "Cozy season""
- "LinkedIn post image about remote team rituals, clean flat illustration"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#social-media-image
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

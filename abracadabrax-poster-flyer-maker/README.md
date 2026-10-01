# Abracadabrax Poster & Flyer Maker

Give Claude a headline and the key details, such as date, place or offer, and get a poster or flyer design with the text laid out on it, in portrait, square or landscape format. Abracadabrax renders it with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude what the poster is for, the headline and the details to print.
2. Claude saves a draft with the visual theme, the format and the image model, and shows its price in credits.
3. You fix the wording or the look, then ask Claude to render it.
4. Abracadabrax renders the design and Claude hands you the link to the image.

## Good to know

- **Made by AI.** Every image and video comes from generative AI models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **Designs from text.** Placing your own photos or logo files on the design needs an upload, which happens in the Abracadabrax workspace, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/poster-flyer-maker/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you render something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_poster_flyer` | Creates a draft from the kind of poster, the headline, the details to print, the theme and the format | none, guest allowed |
| `render_media_widget` | Shows a saved draft again in the panel | none |
| `update_media_project` | Applies the changes made in the panel | none |
| `generate_media` | Starts the render after you confirm | charged, sign-in needed |
| `get_media_job` | Reports progress and returns the file link | none, read-only |

## Try asking

- "Event poster for "Summer Jazz Night", Friday 12 July, 9 pm, Riverside Park"
- "A sale flyer for a bakery: "20% off all pastries this weekend", pastel colors"
- "Concert poster for a garage rock band called The Static, retro 70s style"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#poster-flyer-maker
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

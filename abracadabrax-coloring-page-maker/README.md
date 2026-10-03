# Abracadabrax Coloring Page Maker

Describe a subject or a scene and get a printable coloring page: black outlines on white, with closed shapes ready to color and no shading. The line detail follows who is coloring: big simple shapes for toddlers, a moderate amount of detail for kids, intricate patterns for adults. Abracadabrax renders it with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude what to draw and who will color it.
2. Claude saves a draft with the line detail, a plain or scene background, the page format and the image model, and shows its price in credits.
3. You adjust the subject or the detail, then ask Claude to render it.
4. Abracadabrax renders the page and Claude hands you the link to the image, ready to print.

## Good to know

- **Made by AI.** Every image and video comes from generative AI models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **Pages from text.** Turning your own photo or drawing into a coloring page needs an upload, which happens in the Abracadabrax workspace, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/coloring-page-maker/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you render something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_coloring_page` | Creates a draft from the subject, the line detail (toddler, kids or adults), the background and the page format | none, guest allowed |
| `render_media_widget` | Shows a saved draft again in the panel | none |
| `update_media_project` | Applies the changes made in the panel | none |
| `generate_media` | Starts the render after you confirm | charged, sign-in needed |
| `get_media_job` | Reports progress and returns the file link | none, read-only |

## Try asking

- "A coloring page of a dinosaur playing football for my 4-year-old"
- "An intricate mandala with flowers for adult coloring, square page"
- "A castle with dragons and a moat, with a background scene to color, for a 7-year-old"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#coloring-page-maker
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

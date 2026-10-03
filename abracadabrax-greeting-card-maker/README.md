# Abracadabrax Greeting Card & Invitation Maker

Make a card for someone in your life: a birthday, a wedding or an anniversary, a baby shower, the holidays, a thank-you, a graduation or a get-well wish. Tell Claude who it is for and what it should say, and get the front of a greeting card or an invitation with your message printed exactly as you wrote it and, on invitations, the date, place and RSVP in smaller text. Abracadabrax renders it with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude the occasion, who the card is for and the message.
2. Claude saves a draft with the card or invitation layout, the style, the format and the image model, and shows its price in credits.
3. You fix the wording or the look, then ask Claude to render it.
4. Abracadabrax renders the card and Claude hands you the link to the image, ready to print or send.

## Good to know

- **Made by AI.** Every image and video comes from generative AI models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **Check the spelling.** The message and the event details are printed as you give them; read the finished card before you print or send it.
- **Cards from text.** Adding your own photos to the card needs an upload, which happens in the Abracadabrax workspace, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/greeting-card-maker/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you render something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_greeting_card` | Creates a draft from the occasion, card or invitation, the recipient, the message, the event details and the style | none, guest allowed |
| `render_media_widget` | Shows a saved draft again in the panel | none |
| `update_media_project` | Applies the changes made in the panel | none |
| `generate_media` | Starts the render after you confirm | charged, sign-in needed |
| `get_media_job` | Reports progress and returns the file link | none, read-only |

## Try asking

- "A birthday card for Grandma Rose: "Happy 80th Birthday, Grandma Rose!", watercolor flowers"
- "An invitation to Anna's baby shower, Sunday 9 November at 3 pm, 12 Elm Street, RSVP to Kate"
- "A thank-you card for my son's teacher, Mr. Lee, in a cute cartoon style"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#greeting-card-maker
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

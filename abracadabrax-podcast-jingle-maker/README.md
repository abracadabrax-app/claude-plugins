# Abracadabrax Podcast Intro & Jingle Maker

Give Claude the name of your podcast, channel or stream and its feel, and get a short signature theme to open or close every episode: 30 or 60 seconds, instrumental, or with a short sung tagline that says the show's name. Abracadabrax produces it with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude the show's name and its mood.
2. Claude saves a jingle draft with the genre, instrumental or sung tagline, the length and the model, and shows its price in credits.
3. You adjust it, then ask Claude to produce it.
4. Abracadabrax renders the jingle and Claude hands you the link to the audio file.

## Good to know

- **Made by AI.** Vocals and music come from generative AI music models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **Short by design.** Jingles are 30 or 60 seconds long, with a clear start and a clean ending.
- **New tracks only.** Remixing, extending or splitting an existing recording needs an upload, which happens in the Abracadabrax music studio, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/podcast-jingle-maker/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you produce something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_podcast_jingle` | Creates a jingle draft from the show's name, the mood, the genre, the sung tagline or instrumental choice and the length (30 or 60 seconds) | none, guest allowed |
| `render_song_widget` | Shows a saved draft again in the panel | none |
| `update_song_project` | Applies the changes made in the panel | none |
| `generate_song` | Starts the render after you confirm | charged, sign-in needed |
| `get_song_job` | Reports progress and returns the audio link | none, read-only |

## Try asking

- "A 30-second intro jingle for my podcast "The Morning Brew", upbeat and friendly, funky bass"
- "A sung tagline "You're listening to Deep Dive" with a female voice, synth pop, 60 seconds"
- "An instrumental outro for a cozy book review channel called Shelf Life"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#podcast-jingle-maker
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

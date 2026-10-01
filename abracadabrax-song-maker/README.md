# Abracadabrax AI Song & Music Maker

From an idea to a finished track in one conversation. Claude writes the lyrics with you, and Abracadabrax sings and produces them, or builds an instrumental, using the credits of your own Abracadabrax account.

## How a song gets made

1. Tell Claude what the song is about, the genre, the mood and whether you want vocals.
2. Claude drafts the lyrics and saves a song draft with title, style brief, model and length, shown in a panel together with the price in credits.
3. Change the lyrics or the settings until they feel right, then ask Claude to produce it.
4. Abracadabrax renders the track and Claude gives you the link to the audio file.

## Good to know

- **Made by AI.** Vocals and music come from generative AI music models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **New songs only.** Covering, extending or splitting an existing recording into stems needs an upload, which happens in the Abracadabrax music studio, not in this plugin.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/song/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you produce a song, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_song_project` | Creates a draft with title, style, lyrics, model and length | none, guest allowed |
| `render_song_widget` | Shows a saved draft again in the panel | none |
| `update_song_project` | Applies the changes made in the panel | none |
| `generate_song` | Starts the render after you confirm | charged, sign-in needed |
| `get_song_job` | Reports progress and returns the audio link | none, read-only |

## Try asking

- "Write a punk rock anthem about Monday mornings and produce it with a female singer"
- "Make a gentle lullaby for my newborn niece called Sofia, soft piano and whispered vocals"
- "I need 90 seconds of upbeat synthwave with no vocals for a product demo"

## Your data

Abracadabrax receives only what the tools carry: the lyrics, the style brief, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the audio. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#song
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

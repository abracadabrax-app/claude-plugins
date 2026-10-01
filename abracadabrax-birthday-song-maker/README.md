# Abracadabrax Birthday Song Maker

Make a birthday song that uses the person's name and your own memories: Claude helps you write the lyrics, and Abracadabrax sings and produces the track in the style you pick. It is produced with the credits of your own Abracadabrax account.

## How a request flows

1. You tell Claude who the song is for, their age and a few memories or inside jokes.
2. Claude writes the lyrics with you and saves a draft with the style, the voice and the model, and shows its price in credits.
3. You polish the words, then ask Claude to produce it.
4. Abracadabrax renders the song and Claude hands you the link to the audio file.

## Good to know

- **Made by AI.** Vocals and music come from generative AI music models that Abracadabrax runs with its model partners. Drafts cost nothing; credits are only used when you confirm a render.
- **New songs only.** Singing over an existing song or cloning someone's voice is not available; covers and edits of uploaded tracks happen in the Abracadabrax music studio.

## Connection

Endpoint: `https://abracadabrax.app/api/claude/birthday-song-maker/mcp` (remote MCP, Streamable HTTP).

Drafting works as a guest. The first time you produce something, Claude opens the Abracadabrax sign-in page (OAuth 2.1 with PKCE), where you can also create an account. On clients without MCP Apps, such as Claude Code, the same tools answer with text and links instead of the panel.

## Tool reference

| Tool | Purpose | Credits |
|---|---|---|
| `prepare_birthday_song` | Creates a draft from the name, the lyrics written with Claude, the style, the voice and the occasion | none, guest allowed |
| `render_song_widget` | Shows a saved draft again in the panel | none |
| `update_song_project` | Applies the changes made in the panel | none |
| `generate_song` | Starts the render after you confirm | charged, sign-in needed |
| `get_song_job` | Reports progress and returns the audio link | none, read-only |

## Try asking

- "A happy birthday song for my sister Giulia, she turns 30 and loves surfing"
- "An acoustic birthday song for my dad, with a line about his terrible jokes"
- "A funny pop-punk birthday song for my best friend Sam"

## Your data

Abracadabrax receives only what the tools carry: your request, the chosen settings and the ids of your drafts and renders. They are kept in your Abracadabrax account and passed to the model partner that renders the file. Nothing runs locally and the plugin reads nothing else from your conversation.

## Links

- Documentation: https://abracadabrax.app/mcp#birthday-song-maker
- Privacy policy: https://abracadabrax.app/privacy
- Terms of service: https://abracadabrax.app/terms
- Help: https://abracadabrax.app/support

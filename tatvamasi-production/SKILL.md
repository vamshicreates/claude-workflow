---
name: tatvamasi-production
description: Use for any work on Smita's Tatvamasi devotional song series: lyric subtitles, English meaning text in After Effects, AI visuals (Nano Banana 2 → Kling), and release captions or ads.
---

# Tatvamasi production playbook

## 1. The series

- **Tatvamasi by Smita**: devotional and philosophical song videos in Telugu, Sanskrit and Kannada (Annamacharya keerthanas, stotrams, folk songs). Released on YouTube, with Instagram reel cuts tagged "Tatvamasi – Chapter 1 | Song N".
- Ricky produces: live performance shot on art-directed sets (warm practical light, brass lamps, diyas, rich textiles), edited in After Effects, with AI visuals for chosen lyric lines.
- Songs so far (for reference): Antee Antaka, Annapurna Ashtakam, Telisite Mokshamu, Ninu Vidisi (Ninnu Vidisi Undalenayya), Margabandhu Stotram, Vasudeva Kamalasana, Sojugadu (Kannada folk), Pibare Ramarasam, Ye Kulajudaina Nemi, Aakati Velala, Chinta Nastikila, Brahmam Okkate, Narayanachyutha, Entha Matramuna, Goodu Chinnaboyera, Maithreem Bhajatha, Ekkadi Paapamulu.
- Look: warm cinematic realism with South Indian cultural grounding. The Divine is implied through light, breath and stillness, not shown literally. Colours always come from the video's own palette.

## 2. Working with Ricky

- Show options quickly: visual mock-ups on real frames from the video, with no long setup first. He says so when things take too long.
- Show before building. Build in After Effects only after he picks.
- Apply his feedback exactly (sizes, percentages, hex values, line breaks).
- When a choice is low-stakes, take a sensible default and say which one you took.
- Ask before taking over his screen.
- After he approves a meaning-text design or effect, save it to memory in the meaning-text style "approved designs" log (his standing request). Before designing meaning text, read that memory file if available; it is newer than this skill.

## 3. Usual order for a song

1. Get the lyrics, and later the meanings, from him. Don't spend long researching lyrics; ask for them.
2. Lyric subtitles.
3. Meaning-text design options, then his approval.
4. Add the meaning texts in AE.
5. AI visuals for the lyric lines he chooses: lock the images, then animate.
6. Captions and release copy.

## 4. Lyric subtitles (constant across all songs)

- Lora Regular, 100 px, white, bottom-centre (about y 1954 on a 4096×2160 comp), soft drop shadow (black, 50%, direction 135, distance 5), short fade in and out.
- One text layer per sung line, named by the lyric, orange label (AE label 11).
- Timing: Claude can't hear audio. Extract the audio, separate the vocals, force-align the lyrics to the vocal track, then sanity-check. Also deliver an .srt file.
- Chants and repeats not in his lyrics: flag them and ask whether to add.
- Once he edits the subtitle layers, his edits are the source of truth. Meaning timing follows his subtitle layers.

## 5. Meaning text

### Reference style (his earlier videos)
- A poetic title block in the open space beside the singer: left or right third, mid-height or upper area. Never over faces, never a subtitle bar or box.
- 2–4 short lines, centred or gently staggered, larger than the lyric line.
- Upright classical serif mixed with an italic or flowing face for the key phrase.
- Warm ivory or cream for most words, warm gold (often a light gradient) on key words or the last line.
- Legibility from a soft dark glow or halo only; the text should sit naturally in the scene.

### Approved designs (oldest first; newer preferences win)
- **Antee Antaka / Annapurna**: Carattere script with gold key phrases, plus a clean sans body.
- **Vasudeva Kamalasana ("E2")**: Cormorant Garamond Italic plus Playfair Display Italic. Shade follows the letter shapes (#53261F at about 25%), never a rectangle. Meanings kept to 2–4 lines.
- **Telisite Mokshamu ("Option A")**: client rejected "one word big, the rest small". Every word in one font (Cormorant Garamond Medium Italic) at one size, key words in gold, body ivory, soft drop shadow.
- **Ninu Vidisi**: plain words in Prata Regular; key phrase on its own line in Playfair Display SemiBold Italic. Light gold gradients, never heavy (plain #FFF7E6 → #E6CB96, key #FFF6DA → #E2B96E). Plain at about 87% of key size (130 / 150 px on 4096×2160). Soft dark glow.
- **Margabandhu Stotram ("Kailash moonlight")**: moonlight white (plain #FFFFFF → #DCE7F2, key #FFFFFF → #CFE4F4) with a sky-blue glow (#77ABCC / #96C8EB) taken from the video, a light sweep on the key line and small star glints. Plain lines Cormorant Garamond SemiBold Italic about 116 px; key line Libre Baskerville Bold Italic about 112 px with a stronger glow. Subtle text-in animation.
- **Sojugadu ("B1 Lamp Gold" + "Diya Bloom")**: plain line Cormorant Garamond SemiBold Italic about 132 px, white → #F8EBCD. Key line Fraunces Italic (SOFT 100, wght ~500, opsz 72) about 136 px, #FFF6DE → #EBC47A. Warm brass glow #F2B04E taken from the set's lamps; thin dark warm halo #2A1A0A hugging the letters. Diya Bloom: letters drift up one by one from soft to sharp; the glow swells as they land, then breathes like a diya flame; a slow light sweep crosses the key line; the block fades out with a soft blur.

### Rules
- **Placement:** beside the singer, never over a face, clear of the subtitle zone, inside title-safe (205 px at the sides, 216 px top and bottom on 4096×2160). Check every block against every shot it spans. Move a block at a shot cut only when no single spot works.
- **Size:** readable but not big. Plain about 116–132 px, key about 112–150 px on 4096×2160. Key words only a little bigger than plain (about 80/100). 140–160 px for everything was too big. Never one word much bigger than the rest.
- **Lines:** usually 2. For long meanings, split into 3 lines (4 at most); never shrink the font to fit. Use semantic, balanced line breaks.
- **Colour:** only from the video's own palette, divine-feeling, no random colours. Keep gradients light. A glow must never wash letters out to flat white: in AE Glow use Composite Original = On Top with warm glow colours.
- **Legibility:** a thin halo hugging the letters plus a soft drop shadow so text reads on bright shots. No blurred ellipse or box shade layers behind blocks (rejected as "a black circular mark"). If he adds his own low-opacity shade solids, keep them.
- **Motion:** subtle, neat, divine text-in; soft fade-out. Use the same fade timing on every block (about 0.6 s in, 0.5 s out). Two meanings never on screen together except a short crossfade (about 0.4 s).
- **Editability:** real text layers he can type into, move, trim and duplicate. Don't drive text or position from lookup-table expressions.
- Meaning layers use the red label (AE label 1).

### Mapping meanings to lyrics
- His meaning sheets often give one row per pair of lyric lines. Check each row:
  - **Two-part meaning** (a line break in the cell): each part goes with its own lyric line.
  - **One single meaning** (no break): one block spanning both lyric lines; 3–4 lines is fine.
- Tell him the mapping you used.
- Use his wording verbatim and flag possible typos; don't silently fix them. Shorten only when he asks.
- Timing: in = the lyric start (or the old meaning's in point); out = just before the next meaning (crossfade only).

### Showing design options
- Grab real frames from the comp viewer and render 3–6 labelled options side by side on them (fonts, colours, sizes), e.g. an HTML page rendered with Playwright.
- Say clearly that mock-ups are not the final AE render.
- Use fonts already on his Mac or free Google Fonts. Check in AE with `app.fonts.getFontsByFamilyNameAndStyleName(family, style)`.

## 6. After Effects automation on his Mac

### Two ways to drive After Effects (his choice)
- **A. Scripts via computer use (default, always available):** write .jsx files into his project folder and run them from File > Scripts. Everything below in this section describes this route.
- **B. After Effects MCP (optional):** only if he has set it up and its tools show up in the session (check the device's local MCP servers if unsure). If both routes are available and he hasn't said which to use, ask him once; don't switch routes on your own.
  - Server: `@kumoproductions/mcp-aftereffects` (unofficial, MIT, macOS + Windows, AE 2024–2026, Node.js 24+). Repo: https://github.com/kumoproductions/mcp-aftereffects
  - His setup (he does these on his Mac; Claude can't edit the Claude app's config or type in Terminal): install Node.js 24+; in AE turn on Settings > Scripting & Expressions > "Allow Scripts to Write Files and Access Network"; in the Claude desktop app Settings > Developer > Edit Config add `"aftereffects": {"command": "npx", "args": ["-y", "@kumoproductions/mcp-aftereffects"]}` under `mcpServers`; restart the Claude app; allow macOS Automation access to After Effects if asked. Optional: `"env": {"AE_MCP_READONLY": "1"}` for a look-only mode.
  - Main tools: `ae_context` (read the project), `ae_do` (operations, e.g. `instance.list`), `ae_save_project`. It can also render single frames, which is the best way to check text placement. Full list: the repo's docs/TOOLS.md.
  - Keep arbitrary ExtendScript (`AE_MCP_ENABLE_EVAL`) off unless he asks for it; it can affect the whole computer.
  - Same rules as route A: read before changing, one undo step per change, back up layers before replacing them, never touch the orange subtitle layers, and don't save unless he asks (`ae_save_project` only on request). Try it on a backup .aep the first time.
  - If the MCP fails or isn't responding, say so and offer route A; don't retry endlessly.

### Access (route A)
- Use computer use on his Mac (After Effects 2026). He often has a full-screen app in front, where background control can't click AE; ask before requesting full-screen control.
- Request access to the project folder (projects are on the "Extreme SSD" drive). Put scripts in a subfolder next to the project, e.g. `_meaning_text_scripts`.
- Comps are 4096×2160, 24 fps, about 3–3.5 min, named like `SONGNAME_SONG_4K_DDMMYY`.

### Running scripts
- Use File > Scripts > Run Script File…, then Cmd+Shift+G, type the full path, Return, Open.
- **Before typing, take a screenshot to confirm the Open dialog is really open.** If it isn't, stop: typed characters become AE shortcuts. If the picker can't be operated, ask him to pick the file once.
- Recent Script Files can run a cached old version. Give every new version a new filename, and verify the committed file (stage it back and compare) before running.
- "Allow Scripts to Write Files" may be off, so read-only report scripts should show results in a ScriptUI dialog (monospace multiline edittext) and be read by zooming and scrolling. Never change that preference yourself. If he has turned it on (route B needs it), report scripts can write their results to a text file next to the script instead.

### Script hygiene
- Run a read-only report first: index, label, in/out, text, font, size, fill, position, sourceRectAtTime, opacity keys, effects.
- One `app.beginUndoGroup` per change, plus a `confirm()` that says what will change.
- Find layers by label and in-point, not by index (indices shift when he edits).
- Before replacing layers, back them up: duplicate them, precompose the copies into a hidden "OLD … (backup)" precomp, disable it and move it to the end.
- Never touch the orange subtitle layers. Don't save the project; he saves.
- Dry-run complex scripts against a mock built from the report data (e.g. in Node) before running for real.

### API notes
- `allCaps` is ignored in AE 2026: use `td.fontCapsOption = FontCapsOption.FONT_NORMAL_CAPS`.
- Per-word colour: `td.characterRange(start, end).fillColor = [...]`, then `sourceText.setValue(td)`.
- PostScript names differ from family names (e.g. CormorantGaramondItalic-MediumItalic): always look fonts up by family and style.
- Point text, centre-justified: position is the first line's baseline. Use `sourceRectAtTime` for bounds.
- Drop Shadow matchNames are `ADBE Drop Shadow-0001`…`-0005` (opacity runs 0–255).
- The project may use a linear working space, so fill hex values look brighter on screen than they read. Reuse existing fills rather than inventing new ones.

### Verifying
- Step through every meaning block in the viewer: click the current-time field, type a timecode (e.g. `13110` = 0:01:31:10), Return, then zoom on the viewer.
- Fix any clashes with a small nudge script.
- For larger jobs, shot-cut detection and person segmentation help choose clear space.

## 7. AI visuals

- **Images:** Nano Banana 2 for photoreal stills (Higgsfield `nano_banana_2` or Magnific `imagen-nano-banana-2-flash`). Avoid Soul Cinema and Soul 2 for this series: they come out looking painted.
- First pass at 1k–2k, often two concepts per chosen lyric line. He picks, then upscale the finals. Use 16:9 to match the footage, 9:16 for reel-native frames, 21:9 only when asked.
- **Continuity:** the singer appears as herself in AI frames, using face-reference-locked generation from her stills. Recurring characters get a character anchor sheet passed as a reference on every frame, with wardrobe restated in the prompt.
- Identity models (Higgsfield Soul) only after a consent and likeness check. Soul output works only through Soul text-to-image.
- **Look:** grade to the set's palette so AI shots feel like visions inside the same film. Humans photoreal. Deity frames symbolic, or in a soft watercolour devotional style (ivory parchment washes, fine linework on jewellery, edges dissolving into paper). A warm-gold-into-white glow works as a continuity signature.
- **Story scenes** go in instrumental gaps so lyrics aren't interrupted. Use proper film grammar (wide → medium → close) within one location.
- **Animation:** lock the images first, then Kling 3.0 (Pro), 5 s. Locked camera or an imperceptible push-in; faces and hands locked; breath and aura as baseline motion; one signature moving element per shot; a detailed negative prompt; silent render for AE.
- When there are many frames, give him a selection aid (a storyboard page or a picking sheet).

## 8. Release and social

- **Instagram captions:** three options (poetic, reflective or hook-first, minimal), built from the YouTube description he gives.
  - The first line is the hook, before the "…more" cutoff.
  - Include the lyric line (Telugu or Sanskrit) with an English interpretation, then "Tatvamasi – Chapter 1 | Song N".
  - Hashtags mix broad (#SpiritualMusic #TeluguMusic) and niche (#Tatvamasi #Tattvam, a song-title tag).
  - Frame around universal themes (inner peace, impermanence, detachment) to reach beyond devotional audiences.
- **Meta ads** (verify current platform rules before advising):
  - Religion interests and detailed-targeting exclusions are gone, and Advantage+ treats interests as suggestions, so age is the main hard lever. For modern reinterpretations, test an 18–27 set and a 25–40 set.
  - Target tier-1 metros plus the diaspora, with wellness and fusion-music interests.
  - Build custom audiences from reel video engagement, and lookalikes from engaged young viewers.
  - Turn on Hidden Words; hide rather than delete negative comments; pin supportive ones.
  - Frame the copy as a reverent offering of timeless wisdom to a new generation.

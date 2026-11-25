# After Effects MCP – setup (optional)

Server: `@kumoproductions/mcp-aftereffects` (unofficial, free, MIT). Repo: https://github.com/kumoproductions/mcp-aftereffects
Works on macOS with After Effects 2024–2026. Needs Node.js 24 or newer.

## Steps on the Mac

1. **Node.js** – open Terminal and run `node -v`.
   If it says "command not found" or a version below v24, install the current LTS from https://nodejs.org (macOS installer), then check `node -v` again.

2. **After Effects** – Settings > Scripting & Expressions > turn on
   "Allow Scripts to Write Files and Access Network". Restart After Effects.

3. **Claude desktop app** – Settings > Developer > Edit Config. In `claude_desktop_config.json` add:

   ```json
   {
     "mcpServers": {
       "aftereffects": {
         "command": "npx",
         "args": ["-y", "@kumoproductions/mcp-aftereffects"]
       }
     }
   }
   ```

   If the file already has `"mcpServers"`, add only the `"aftereffects": { ... }` entry inside it.
   Optional look-only mode: add `"env": { "AE_MCP_READONLY": "1" }` inside the `"aftereffects"` entry.

4. **Restart the Claude app** (Quit fully, then open again). Open After Effects with a project.

5. If macOS asks to let Claude control After Effects, allow it
   (System Settings > Privacy & Security > Automation).

6. In a chat linked to this Mac, say "test the AE MCP". Claude will check it on a backup copy of a project first.

## Notes
- It's optional: Claude can still work the usual way (scripts via File > Scripts) if you prefer.
- Leave `AE_MCP_ENABLE_EVAL` off (it allows any script, which can affect the whole computer).
- Layer names, text and paths it reads are sent to Claude.

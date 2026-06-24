# @runapi.ai/grok-imagine-mcp

RunAPI MCP server for the **Grok Imagine** model line. Create tasks,
poll their status, and check pricing through a single RunAPI API key.

## Tools

- `edit_image` — create a Grok Imagine task (edit image) and (optionally) poll until it reaches a terminal status. Returns the task id, status, output URLs, and a price snapshot. Models: `grok-imagine-edit-image`, `grok-imagine-image-to-video`, `grok-imagine-text-to-image`, `grok-imagine-text-to-video`.
- `extend_video` — create a Grok Imagine task (extend video) and (optionally) poll until it reaches a terminal status. Returns the task id, status, output URLs, and a price snapshot. Models: `grok-imagine-edit-image`, `grok-imagine-image-to-video`, `grok-imagine-text-to-image`, `grok-imagine-text-to-video`.
- `image_to_video` — create a Grok Imagine task (image to video) and (optionally) poll until it reaches a terminal status. Returns the task id, status, output URLs, and a price snapshot. Models: `grok-imagine-edit-image`, `grok-imagine-image-to-video`, `grok-imagine-text-to-image`, `grok-imagine-text-to-video`.
- `text_to_image` — create a Grok Imagine task (text to image) and (optionally) poll until it reaches a terminal status. Returns the task id, status, output URLs, and a price snapshot. Models: `grok-imagine-edit-image`, `grok-imagine-image-to-video`, `grok-imagine-text-to-image`, `grok-imagine-text-to-video`.
- `text_to_video` — create a Grok Imagine task (text to video) and (optionally) poll until it reaches a terminal status. Returns the task id, status, output URLs, and a price snapshot. Models: `grok-imagine-edit-image`, `grok-imagine-image-to-video`, `grok-imagine-text-to-image`, `grok-imagine-text-to-video`.
- `upscale_image` — create a Grok Imagine task (upscale image) and (optionally) poll until it reaches a terminal status. Returns the task id, status, output URLs, and a price snapshot. Models: `grok-imagine-edit-image`, `grok-imagine-image-to-video`, `grok-imagine-text-to-image`, `grok-imagine-text-to-video`.
- `get_task` — fetch the current status and latest payload for a task.
- `check_pricing` — look up pricing for a model in this line.

## Configuration

Set a RunAPI API key via the `RUNAPI_API_KEY` environment variable, or write
it to `~/.config/runapi/config.json`:

```bash
mkdir -p ~/.config/runapi
echo '{"api_key":"YOUR_KEY"}' > ~/.config/runapi/config.json
```

Get an API key at https://runapi.ai. Pricing is listed at
https://runapi.ai/pricing.

## Usage

Run the server over stdio:

```bash
npx -y @runapi.ai/grok-imagine-mcp
```

Add it to an MCP client (see `examples/` for per-client configs):

```json
{
  "mcpServers": {
    "grok-imagine": {
      "command": "npx",
      "args": ["-y", "@runapi.ai/grok-imagine-mcp"],
      "env": { "RUNAPI_API_KEY": "${RUNAPI_API_KEY}" }
    }
  }
}
```

## License

Apache-2.0

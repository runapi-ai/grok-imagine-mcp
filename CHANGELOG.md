# Changelog

## [v0.1.12](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.12) - 2026-08-21

### Added
- Add Image 2.0 text-to-image, segment-map, and segment-backed image editing tools.


## [v0.1.11](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.11) - 2026-07-31

### Changed
- Resolve MCP prices from the RunAPI Price Schedule API instead of embedded package data.


## [v0.1.10](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.10) - 2026-07-23

### Changed
- Refresh the generated pricing snapshot for reviewed Preview and Fast video requests.


## [v0.1.9](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.9) - 2026-07-20

### Breaking
- Replace Grok Imagine image-to-video `source_image_urls` with scalar `source_image_url`.
  Migration: Set `source_image_url` to the source image URL when creating an image-to-video task.


## [v0.1.8](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.8) - 2026-07-17

### Changed
- Refresh Grok Imagine MCP contract and pricing data for the Fast video model.

## [v0.1.7](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.7) - 2026-07-16

### Changed
- Refresh the Grok Imagine MCP contract, pricing data slice, tests, and package metadata for the Video 1.5 Preview variant.

## [v0.1.6](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.6) - 2026-07-08

### Fixed
- Publish corrected MCP runtime metadata for the login release.

## [v0.1.5](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.5) - 2026-07-08

### Changed
- Publish MCP login onboarding, optional API key metadata, and the updated core dependency.

## [v0.1.4](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.4) - 2026-06-24

### Changed
- Publish grok-imagine-mcp v0.1.4.
- Pin the package to @runapi.ai/mcp-core v0.1.3.
- Refresh package and MCP Registry metadata for this release.

## [v0.1.3](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.3) - 2026-06-24

### Changed
- Refresh public README metadata for the focused Grok Imagine MCP package.

### Fixed
- Correct the GitHub repository badge URL so package README badges render cleanly on npm and GitHub.

## [v0.1.2](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.2) - 2026-06-24

### Changed
- Refresh the public README with focused install paths, model links, and agent prompt examples.
- Update npm and GitHub metadata for developer discovery.
- Keep server.json and packaged contract/pricing data aligned with the release artifact.

## [v0.1.1](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.1) - 2026-06-24

### Changed
- Distinct per-line README, npm keywords/description, and GitHub topics for Grok Imagine so the package is discoverable on its own name and capabilities. No tool, schema, or behavior changes.

## [v0.1.0](https://github.com/runapi-ai/grok-imagine-mcp/releases/tag/v0.1.0) - 2026-06-24

### Added
- Initial release of the Grok Imagine MCP server: create tasks, poll their status, and check pricing for every Grok Imagine model with a single RunAPI API key.

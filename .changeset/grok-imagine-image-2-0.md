---
'@tanstack/ai-grok': minor
---

Add first-class support for `grok-imagine-image-2.0`, the current generation of xAI's Imagine image models.

- New model in `GROK_IMAGE_MODELS` and all image type maps (provider options, size, input modalities).
- New `GrokImagineImage2ProviderOptions` with the 2.0-only `quality` option (`'low' | 'medium'`, default `'medium'`).
- Image-editing requests now send `type: 'image_url'` on each source image (`image` / `images` entries), matching xAI's documented request shape.
- `grok-imagine-image-quality` is marked deprecated in code comments and the docs note (kept for backward compatibility); prefer `grok-imagine-image-2.0`.

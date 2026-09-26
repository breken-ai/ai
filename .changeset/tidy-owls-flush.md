---
'ai': patch
---

fix(ai): `extractReasoningMiddleware` now flushes its buffer when a text part ends. A reasoning block without a closing tag (for example when the output is cut off by `maxOutputTokens`) now gets a `reasoning-end`, and a trailing partial tag such as `<` is kept as text instead of being dropped.

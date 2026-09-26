---
'@ai-sdk/mcp': patch
---

fix(mcp): report each failed HTTP transport request to `onerror` once. A non-2xx POST response or a failed authorization reached `onerror` (and the client's `onUncaughtError`) twice.

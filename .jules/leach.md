# Leach's Journal

## Critical Learnings

- **Dangling Intervals in Discord.js Helpers**: The `handleUserRequest` function in `functions/interactions.js` uses `setInterval` for a typing indicator. If an error occurs or the function returns early without hitting the `finally` block (e.g., due to an unhandled exception or process termination), the interval might persist if not handled carefully.
- **Map vs WeakMap**: Several maps (`responseMap`, `botToAuthorMap`, `CANONICAL_CACHE`, `PAGE_DATA_CACHE`) use manual pruning instead of `WeakMap`. While `WeakMap` isn't always suitable (e.g., when keys are strings), ensure that string-keyed maps are strictly capped.
- **Event Listeners in initialise.js**: `client.on` listeners are added once and are generally fine for a bot's lifecycle, but if the client were to be re-initialized without clearing these, it would leak.
- **Unbounded Map Growth**: The `botToAuthorMap` in `initialise.js` was identified as a source of memory leaks as it grew indefinitely with every message reaction. Pruning this Map is essential for long-term stability.

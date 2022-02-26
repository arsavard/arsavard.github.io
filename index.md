# Svelte / Sveltekit Does manifest file exist?
Feb. 25, 2022

Svelte is still a pretty small community, so if I find something that I didn't get right away or couldn't quickly find an answer, I'm putting them here for posterity, or perhaps to help someone else.

You'll maybe have seen something akin to the following:

```[vite] Internal server error: Failed to resolve import "../../src/routes/delete.svelte" from ".svelte-kit/generated/manifest.js". Does the file exist?```

Maybe you're familiar with it, maybe you've never seen it before, but it took me a moment to catch it. Easy fix:

```
svelte run build
```

Everything works!

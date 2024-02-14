
This documents some of the weirdest bugs I've seen and some tricks to fix it

## `Esc` key is equal to `Ctrl+[` 

Not really a bug, but something to note. In Linux it just so happens that the combination of the keys `Ctrl` and `[` gives the keycode for the `Esc` key, so just a tip for the future


## `Astro-lsp` doesn't work!

This one's actually pretty annoying, as at 2024-14-02, the astro-lsp on neovim dosen't work the only solution I found was to install a previous version 
```bash
:MasonInstall astro-language-server@1.0.8
```

Hope it's fixed soon
# space.vim

space.vim is a plugin which remaps the `<Space>` key to act as a clever
key to repeat motions. It hooks into several of the more complex motion
commands, such as search commands, diff movement commands, quickfix and
location list commands, tag commands and more. When a command that space.vim
has hooked into is issued, it remaps the `<Space>` key to repeat that
command, and it also remaps `<S-Space>` and `<BS>` to do the inverse.

This is a slightly modified version of the original version from
[spiiph][space] with ability to support some of [vim-unimpaired][unimpaired]
keymap.

It's also able to unmap `;`, `,` which often remapped to colon `:`
and `<leader>` as a common habit of Vim user. (`<space>` still works as
expected: `fX<space><space>`...)

Add this line to `.vimrc`:

```vim
let g:space_no_character_repeat_movements = 1
```

[space]: https://github.com/spiiph/vim-space 
[unimpaired]: https://github.com/tpope/vim-unimpaired
 vim:set ts=4 sw=4 tw=78:

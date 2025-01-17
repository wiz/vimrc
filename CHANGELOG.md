## Changelog

= 1.20.36 =
* The nnoremap `<Leader>wd` (`DeleteTrailing()`) changes to `<Leader>td`.

= 1.20.35 =
* Add semicolon to Maxima strings when it's needed.

= 1.20.34 =
* Reduce automatic pclose to deoplete functionality.

= 1.20.33 =
* Set `nomodeline` to fix vulnerability.

= 1.20.32 =
* Change the maps `<C-q>` (neosnippet) to `<C-s>`.

= 1.20.31 =
* Rename `Converter()` to `EPS2PNG()`.

= 1.20.30 =
* Add the cnoremap `<C-q>` to delete a word, forward; as I do in Zsh.

= 1.20.29 =
* Cnoremap `<C-z>` must paste yanked text instead of word under the cursor.

= 1.20.28 =
* Fix: delete the previous content in the preview window.

= 1.20.27 =
* Unify functions to generate images to only one: `Generator()`.
* Remove the old five functions.
* Add support to generate PNG images with Asymptote language.
* Add support to images with POV-Ray.
* Redirect the stderr to the preview window when generator fails.
* Split `Commander()` function to `ResizeWinPreview()`.

= 1.20.26 =
* Add Lua and PHP commands in `Runners()` to execute them.

= 1.20.25 =
* Fix: delete tmux window when it's already open (rename tmux window).

= 1.20.24 =
* Autoupdate buffer before running the script.

= 1.20.23 =
* Remove some makeprg settings.
* The nnoremap to preview code in a tmux window changes to `<Leader>ij`.
* Add the function `Scripty()` to output code in the preview window.
* Add the nnoremap `<Leader>ii` to output code in the preview window.
* Add the function `Runners()` to define commands for some languages.

= 1.20.22 =
* Remove the plugin Quickrun, since I'm using own functions.
* Remove the maps `<Leader><Tab>` to run Quickrun.
* Add the function `PyShebang` to check the python version in the shebang.
* Prevents `Tmuxy()` to don't close the tmux window until Enter is pressed.

= 1.20.21 =
* Change all the nnoremaps to convert, generate or run to `<Leader>ii`.
* Reorganize the configuration.

= 1.20.20 =
* Add the function `Texy()` to convert LaTeX to PDF.
* Add thte nnoremap `<Leader>ix` to convert LaTeX to PDF and preview it.
* Add the linter `chktex` for LaTeX syntax checking.

= 1.20.19 =
* Remove the nnoremap `<M-p>` for `:TmuxNavigatePrevious`.
* Add the nnoremap `<M-d>` to scroll down the preview window from another.
* Add the nnoremap `<M-u>` to scroll up the preview window from another.
* Remove the last empty line from the output of the `:Commander` function.
* Remove the plugin sexy_scroller.

= 1.20.18 =
* Move the cursor to top in the preview window.

= 1.20.17 =
* Resize automatically the preview window.

= 1.20.16 =
* Fix `ToggleSpelllang()`: better conditionals to check the language.
* Fix `SQLExec()`: format queries only when it's a SQL `SELECT`.

= 1.20.15 =
* Improve the nnoremaps to work on bufer.
* Fix an error in the SQL queries execution.

= 1.20.14 =
* Add the nnoremap `q` to close the temporary preview window from inside.

= 1.20.13 =
* Remove the plugin vim-notebook.
  - It needs blocks in markdown and the output writes same document.
  - It requires to start the kernel first...
* Implement a function to execute Maxima instructions, as in SQL queries.
  - This solution is cleaner because it uses a temporary preview window.
  - A second instruction overwrites the previous one (better workflow).
  - It has syntax enabled, using MAX files.
  - It does not require extra commands to start a kernel.
  - It executes one line or one selection instead of a markdown block.

= 1.20.12 =
* Exclude csv syntax from vim-polyglot.
* Add `Plotty()` to generate 2D/3D graphs with Gnuplot and mupdf preview.

= 1.20.11 =
* Improve `Eucly()` to echo syntax errors when it's required.

= 1.20.10 =
* Add `convert` options for the EUK to PNG conversion.

= 1.20.9 =
* Create a new configuration section: "External tools integration".

= 1.20.8 =
* Add `Eucly()` to generate PNG from EUK using Eukleides and mupdf preview.
* Add the nnoremap `<Leader>ie` to run `Eucly()`.

= 1.20.7 =
* Set properly the height of the preview window.

= 1.20.6 =
* Remove the plugin vim-dadbod.
* Improve the function `SQLExec()` to handle sqlite natively.
* Implement a function to create a temporary preview window.
* Implement a function to send a command to the preview window.
* Add the map `<Leader>.` to close the preview window faster.
* The map for wincmd is now `<Leader>,` (faster to type).
* Create the command `Commander` to preview shell commands.

= 1.20.5 =
* Split vimwiki into subfolders based on categories.

= 1.20.4 =
* Check if sqlite database exists before running SQL queries.

= 1.20.3 =
* Refactor `ToggleColorColumn()`.
* Refactor `ToggleCPosition()`, and execute it silently.

= 1.20.2 =
* Improve `ToggleResize()` so it maximizes the window on WinEnter event.
* Remove the command `ToggleResize`. The nnoremap `<C-f>` is enough and faster.

= 1.20.1 =
* Extend `SQLExec()` to execute SQL queries from the visual mode.
* Add the nnoremap `<Leader>ia` to add/change the database path.

= 1.20.0 =
* Install the plugin vim-dadbod to use Vim as databases client.
* Add the nnoremap `<Leader>is` to execute SQL queries (one by line).

= 1.19.13 =
* Add `Planty()` to generate PNG from UML using PlantUML and mupdf preview.
* Add the nnoremap `<Leader>iu` to run `Planty()`.
* Add plantuml output for vim-quickrun to preview with feh.

= 1.19.12 =
* Remove the nnoremap `<C-z>` (omni SQL completion). Deoplete is enough.
* Disable omni SQL default maps with global variable.

= 1.19.11 =
* Use `<Leader>ii` with `<buffer>` to extend `Tmuxy()`.
* Improve `Tmuxy()`: it wraps for any FileType.

= 1.19.10 =
* Improve `Marky()` adding `grep mupdf`.

= 1.19.9 =
* Add the nnoremap `<Leader>io` to run bash in a tmux window.
* Improve `Marky()` changing `lsof -a` to a good `ps -ef`filter.
* Add options to convert to MD to PDF with better fontsize and margins.

= 1.19.8 =
* Fix markdown keymaps!
* The nnoremap `<Leader>ins` (`:NotebookStart`) is now `<Leader>ims`.
* The nnoremap `<Leader>inc` (`:NotebookClose`) is now `<Leader>imc`.
* The nnoremap `<Leader>inn` (`:NotebookEvaluate`) is now `<Leader>imm`.
* Add `--webtex` service to generate math formulas in EPUB.

= 1.19.7 =
* Fix surround settings: double quotes required.
* Remove closetag settings for php and erb.

= 1.19.6 =
* Reduce markdown fenced languages (only sh and python).
  - This change reduces de timeload of a markdown file.

= 1.19.5 =
* Downgrade deoplete, again (Vim).

= 1.19.4 =
* Add auto-shebang for new `*.js` files (node).

= 1.19.3 =
* Add `auto_complete_delay` for deoplete plugin.
* Fix auto-shebang for new `*.py` files (use python3).

= 1.19.2 =
* Remove the plugin vim-instant-markdown. Marky has better workflow.
* Remove the nnoremap `<Leader>im` for `InstantMarkdownPreview`.
* Set the option `conceallevel` to 0.
* Add the nnoremap `<Leader>coo` to set `conceallevel` to 0.
* Add the nnoremap `<Leader>coi` to set `conceallevel` to 2.
* Remove the nnoremap `<Leader><Del>y` to delete a file. Use other methods.
* Stop removing automatically trailing whitespaces. Now is a command.
* Add the nnoremap `<Leader>wd` to remove trailing white spaces.
* Unset default spell for markdown files. It's annoying.
* Stop renaming title of tmux tab with current filename.
* Change the inoremap `çç` to `ÑÑ` to insert `{}` faster.

= 1.19.1 =
* Improve Marky: use Mathjax for HTML, and fix "bug" on lsof command.

= 1.19.0 =
* The nnoremap `<C-b>` (close buffer) changes to `<Leader>bd`. Regression.
* Install the plugin vim-notebook to use maxima into Vim.
* Add the nnoremap `<Leader>ins` to run the command `:NotebookStart`.
* Add the nnoremap `<Leader>inc` to run the command `:NotebookClose`.
* Add the nnoremap `<Leader>inn` to run the command `:NotebookEvaluate`.

= 1.18.4 =
* Upgrade deoplete.nvim (Vim only). They fixed bugs.
* Remove `ToggleGsPrev()`. Use `:Gstatus` directly.

= 1.18.3 =
* Extend Marky function to export to PDF and HTML.

= 1.18.2 =
* Function to convert MD to EPUB and preview it with Mupdf

= 1.18.1 =
* Downgrade deoplete.nvim (Vim only).
* Add csslint in the ALE options.

= 1.18.0 =
* Install the plugin vim-polyglot (better syntax support).
* Install the plugin perlomni.vim (Perl support).
* Install the plugin vim-ruby (Ruby support).
* Install the plugin vim-rails (RoR support).
* Install the plugin vim-endwise (end certain structures).
* Install the plugin phpcomplete.vim (PHP support).
* Install the plugin vim-racer (Rust support).
* Remove the plugin neopairs.vim (using auto-pairs).
* Remove the plugin vim-jquery (not used).
* Remove the plugin vim-javascript (already into vim-polyglot).
* Reformat plugins organization.

= 1.17.14 =
* Fix italics issue (only in Vim).
* Fix tmux-navigator setting introduced in v1.17.12 (only in Neovim).

= 1.17.13 =
* Switch nnoremaps `<F7>` (is now terminal) and `<C-t>` (is now Tagbar).
* Create a custom function to have a better toggle for Tagbar.

= 1.17.12 =
* Remove 'runner/vimproc' (vim-quickrun settings).
* Improve markdown otuput for vim-quickrun.

= 1.17.11 =
* Change the workspace directory name (for vimwiki).

= 1.17.10 =
* The nnoremap `<Leader>cc` (toggle NERDCommenter) changes to `cc`.
  - Faster to type.
* Remove the inoremaps `<C-k>` and `<C-j>` to move lines from Insert Mode.
  - These maps must be only for Normal and Visual modes.
* Add the map `<M-n>` to jump to the next AutoPairs match.
* Add the map `<M-p>` to toggle the plugin AutoPairs.
* Add a workaround to fix an AutoPairs bug into nvim for `<M-">`.
* Update `closetag_filenames` with `*.html.erb`.
* Set fillchars with different unicode symbols.
* The nnoremap `<Leader>df` changes to `cv`.
  - Faster to type.
* The nnoremap `<Leader>ds` changes to `cx`.
  - Faster to type.
* Add the inoremap `ññ` to insert `[]` faster.
  - Faster to type.
* Add the inoremap `çç` to insert `{}` faster.
  - Faster to type.
* The nnoremap `<Leader>wd` (switch CWD) changes to `<Leader>bw`.
  - Back to the version 1.17.4.
* Remove the inoremap `<C-s>` to delete the last character.
* Remove the cnoremap `<C-s>` to delete the last character.
* KEYMAPS.md file has been reorganized.

= 1.17.9 =
* Add the cmap `<C-l>` to init CapsLock into the command-line.

= 1.17.8 =
* Function `Tmuxy()` for python doesn't need to use the interactive mode.

= 1.17.7 =
* Remove `make` from the `autocmd QuickfixCmdPre`.
* Add the function `Tmuxy()` to run code into a tmux window.
* Add the nnoremap `<Leader>ii` to run the function `Tmuxy()`.
* The nnoremap `<Leader>M` (InstantMarkdownPreview) changes to `<Leader>im`.
* Redistribute some Fkeys and avoid the Shift + Fkeys:
* - The nnoremap `<F4>` (toggle Tagbar) is now `<F7>`.
* - The nnoremap `<S-F3>` (toggle relative numbers) is now `<F4>`.
* - The nnoremap `<S-F8>` (toggle spell dictionaries) is now `<F9>`.
* - The nnoremap `<F9>` (toggle colorcolumn) is now `<F10>`.
* - The nnoremap `<S-F12>` (reload colorscheme) is now `<F11>`.
  - (F7, F10 and F11 were available).

= 1.17.6 =
* Check if vim 8 has terminal.
* The nnoremap `<Leader>ii` changes to `<Leader>gs` (stage hunk).
* The nnoremap `<Leader>io` changes to `<Leader>gu` (unstage hunk).
  - This change avoids staging hunks by error pressing double i.
* Add the nnoremap `<Leader>gg` to search a string between commits (Glog).
  - With this, I extended the function `GrepWrapper()`.
* Add the path for the plugin vim-sessions.
  - Neovim was using `~/.vim` path by default...
* Add the path for the clang library.
  - Deoplete couldn't find it on Debian. It worked fine on Arch, though.
* The nnoremap `<C-W><CR>` (close the window) changes to `<C-W>j`.
* The nnoremap `<F10>` (fullscreen window) changes to `<C-f>`.
* The nnoremap `<Leader>bd` (close buffer) changes to `<C-b>`.
* Remove the nnoremap `<Leader>ba` (to close all buffers). Never used it.

= 1.17.5 =
* Add terminal keycodes on vim to make it compatible with rxvt.
* Remove paste mode on nvim (bracketed-paste-mode is built-in).
* Configure vim to use bracketed-paste-mode under 'screen' &term.
* Remove the map `<F7>` to toggle between paste/nopaste. Obsolete.
* Fix URL referencing my tmux config from dotfiles repository.

= 1.17.4 =
* The nnoremap `<Leader>g` (Gvdiff) changed to `<Leader>gv`.
* Add the nnoremap `<Leader>gh` to split horizontally (Gsdiff).
* Add the nnoremap `<Leader>gb` to run the command Gblame.
* The nnoremap `<Leader>i` (GitGutterStageHunk) change to `<Leader>ii`.
* Add the nnoremap `<Leader>io` to run the command GitGutterUndoHunk.
  - These maps are more intuitive.
* The nmap `gl` (openbrowser) changed to `<Leader>gl`. Avoid conflict with Vimwiki.
* The nnoremap `<Leader>bw` (switch CWD) changed to `<Leader>wd`.
* Remove the cnoremap `%%` to expand the path of the current buffer.

= 1.17.3 =
* Remove xterm-modifier-keys for tmux. It works well using URxvt.
  - `$TERM` must be rxvt-unicode-256color (.Xresources and .tmux.conf).

= 1.17.2 =
* Add `\<` and `\>` to highlight the word under the cursor.
  - Removed it in the version 1.14.1 (it's better with it).
* Add options to `grep -R`: exclude CVS directories and LICENSE file.

= 1.17.1 =
* Add `g:NERDCustomDelimiters` for Python.
* Remove the `gv` after toggle comment with `<Leader>c`.
  - Tired of pressing `<C-c>` to return to Normal Mode.
* Add highlights (headers and checkbox) for the Vimwiki.
* Fix some vint warnings.
* Add the setting `mouse=a` in Vim (like in Neovim).
* I decided to adjust `colorcolumn=80` and `set number`.
* Add file headers for Python, Ruby, Perl and Bash new files.

= 1.17.0 =
* Remove phpcomplete-extended plugin.
* Remove neocomplete plugin from Vim8.
* Remove jedi-vim plugin from Vim8.
* Install deoplete plugin on Vim8.
* Install nvim-yarp plugin (required to use deoplete on Vim8).
* Install vim-hug-neovim-rpc plugin (required to use deoplete on Vim8).
* Install deoplete-jedi plugin for Vim8 (Python autocomplete).
* Install deoplete-ternjs plugin (javascript autocomplete).
* Install deoplete-zsh plugin (zsh autocomplete).
* Install neco-ghc plugin (Haskell autocomplete).
* Update all settings for deoplete.
* Add pylint (python linter).
* Quickrun outputter uses vertical buffer instead of quickfix.
* Vimwiki: avoid URL shortener (show full URL). Shortener was buggy.
* Rename `CloseLastQF` function to `CloseLastBuffer`.
* Function `CloseLastBuffer` closes 'nofile' `&buftype`.
* Function `CloseLastBuffer` calls system to rename tmux window.

= 1.16.3 =
* Change `g:ftplugin_sql_omni_key` to `<C-z>`.
  - Default was `<C-c>` (it was in conflict).

= 1.16.2 =
* Add the `--ignore-case` option to grepprg.

= 1.16.1 =
* The nnoremap `<Leader>g` (Gstatus) changed to `<C-s>`.
  - It's faster to toggle Gstatus having Ctrl pressed.
* The nnoremap `<Leader>G` (Gvdiff) is now `<Leader>g`.
  - It reduces one keystroke to make a Gvdiff (faster).
* The nnoremap `<C-s>` (OpenSession) moved to `<C-q>`.
  - It's normally used once at start, so I put it farther.
* The nnoremap `<Leader>v` (vimgrep %) changed to `<Leader>vg`.
* The nnoremap `<Leader>V` (vimgrep \*\*/\*.) changed to `<Leader>vf`.
* Add the nnoremap `<Leader>vv`: grep the highlight (current buffer).
* Add the nnoremap `<Leader>vb`: grep the highlight (loaded buffers).
* Add the nnoremap `<Leader>vn`: grep the highlight (current directory).
* Add the nnoremap `<Leader>vm`: addgrep the highlight (current buffer).
* Add the nnoremap `<Leader>va`: grep the highlight (current arglist).
* Add two functions: `QFCounter()` and `GrepWrapper()` for the last commands.
* The nnoremap `<Leader>R` now uses `:bufdo` instead of `:argdo`.
* Add the nnoremap `<Leader>Q`: replace the highlight to each quickfix entry.
* Improve the function to toggle the cursor position (`ñ`).

= 1.16.0 =
* Add the plugin js-beautify, mapped to `<Leader>bf`.
* Add the maps `<Leader>bf` to autoformat SQL and XML.
* Add the nnoremap `<Leader>tf` to `:retab` the buffer.

= 1.15.2 =
* Remove the plugin Vimshell from vim.
* Add a new function for Vim: `ToggleTerminal()`.
* Improve the same function on Neovim.
* Add the tnoremap `<Esc>` to `<C-\><C-n>`.

= 1.15.1 =
* Allow plugin CtrlP to follow symlinks.
* Fix double quotes in function `WrapForTmux(s)`.

= 1.15.0 =
* Add the plugin vimwiki.
* Add the maps `<Leader>we` to `:VimwikiToggleListItem`.
* Configure the plugin open-browser to use w3m into a tmux window.

= 1.14.1 =
* Follow vimscript style guide.
* Switch nnoremaps `<Leader><BS>` and `<Leader>m`.
* Remove `\<` and `\>` from highlight the word under the cursor.
* Remove nnoremaps `<Leader>ww` and `<Leader>wg` (spelling).
* Add `g:markdown_fenced_languages` for some languages.
* Fix `ToggleCPosition`, use `$` instead of `g_`.

= 1.14.0 =
* Install Atomic color scheme as plugin.
* Add the nnoremap `<Leader>i` for `:GitGutterStageHunk`.
* Add the nnoremap `<Leader>I` for `:GitGutterUndoHunk`.
* Remove background setting. Color scheme manages it.
* Remove the workaround for ncurses 6.0 on neovim.
* Add the cnoremap `<C-z>` to paste yanked text (`<C-R><C-W>`).
* Change foldmethod to marker.

= 1.13.1 =
* Fix vnoremap `<Leader><Tab>` to execute `:QuickRun`.

= 1.13.0 =
* Remove Syntastic and Neomake from Vim/Neovim. Use ALE.
  - Syntastic is not async.
  - Syntastic and Neomake don't lint while coding.
* Use QuickRun to run code in Neovim, with better settings.
  - QuickRun can run the selected lines in 'Visual mode'.
* Remove function for `:Glog`. Use the plugin GV.
  - It does not populate the quickfix, so it's better for me.
  - It is possible to track the changes in the selected lines.
  - And it shows the last commits with a nicer format.
* Finally, remove FZF plugins. I prefer CtrlP + GV combo.
* So, remove the nnoremap `<Leader>C` to open `:Commits`.
* Also, install the plugin vim-ruby. (Support for ruby).
* Expand neosnippet with `<C-q>` instead of `<C-z>`.
  - `<C-q>` is closer to `Tab` and avoid conflicts with GV.
* Fix some makeprg settings, and drop cpp.

= 1.12.3 =
* The command `:W` changed to :`WW`. It was in conflict.
* Added a new function for Neovim: `ToggleTerminal`.

= 1.12.2 = (only Neovim)
* Added python2 path for deoplete. It's optional.
* Added `mouse=a` because it's not a default in nvim 2.0.
* Cursor shape options changed in nvim 2.0, so I updated them.
* Disabled true colors for terminal (old option is ignored).

= 1.12.1 =
* Fixed the command `:W`. It was not well defined.
* Added a workaround for ncurses 6.0 on Archlinux/nvim.
* Yank the last pasted text automatically (`pgvy`).

= 1.12.0 =
* Added the command `:W` to save a file with sudo permissions.

= 1.11.0 =
* Removed Vimshell plugin from Neovim (unnecessary).
* The nmap `<G-p>` (GitGutter preview) changed to `<C-g>`.
* Improved the nnoremap `<Leader>G` (added `gg`).
* The map `<C-s>` (CtrlP menu) changed to `<C-p>`.
* Better prompt mappings (readline) for CtrlP plugin.
* Added the nnoremap `<C-s>` to open `:OpenSession`.
* The vnoremaps `<Leader><` (toggle case) changed to `<Leader>z`.
* The nnoremap `<Leader>z` (`:FZF`) now toggles the caps.
* The nnoremap `<Leader>Z` (`:Commits`) changed to `<Leader>C`.
* Added new function to toggle vim-fugitive-:Glog with `<C-z>`.
* Deleted the navigation maps from Insert mode `<expr>^X@sh`.
* Deleted the navigation maps from Command mode `<expr>^X@sh`.
* Added the inoremap `<C-s>` to delete the last character.
* Added the inoremap `<C-d>` to delete the current character.
* Added the cnoremap `<C-s>` to delete the last character.
* Added the cnoremap `<C-d>` to delete the current character.
* Extended the nnoremap `<C-t>` to vim (open `:Vimshell`).
* Vim supports cursor shape only for `rxvt\|xterm\|tmux`.

= 1.10.0 =
* Added the plugin goyo.

= 1.9.0 =
* Switched the plugin Gundo to Undotree (tired of Python 2.4+ requirement).

= 1.8.2 =
* Fixed Neomake settings: `BufEnter` changed to `BufWinEnter`.
* Added a function to close the quickfix window if it's the last window.

= 1.8.1 =
* Added the nnoremap `<C-t>` to open the `:terminal` (only for Neovim).
* Added the tnoremap `<C-c>` to switch `:terminal` to the last window.

= 1.8.0 =
* Added the plugin neco-vim.
* Added the plugin neco-syntax.
* Added the plugin neopairs.

= 1.7.6 =
* Maps `<C-s>` (neosnippet) changed to `<C-d>`; had conflict with CtrlP maps.

= 1.7.5 =
* Autocompletion fixes.
* Removed the plugin deoplete-ternjs because it has a .tern-port issue.

= 1.7.4 =
* Tern fix: do not create .tern-port file.

= 1.7.3 =
* Show hidden files into CtrlP menu.

= 1.7.2 =
* Removed the nnoremap and vnoremap `<Leader>4` to `g$`.
* Removed the nnoremap and vnoremap `<Leader>6` to `g^`.

= 1.7.1 =
* The maps `<C-d>` (expand neosnippet) changed to `<C-s>`. Conflict fix.

= 1.7.0 =
* Removed all the `<Leader>` commands from Insert mode.
* Removed most of the `<Leader>` commands from Visual mode.
* Removed the fast Escape key (`<Leader><Leader>`).
* The `<Esc>` function can be used with the triggered `<C-c>`.
* Removed the plugin (a.vim), it was annoying and useless.
* Added the nnoremap `<Leader>G` for the command `:Gvdiff`.
* CtrlP map changed to `<C-s>` (`<C-c>` crashed in Visual mode).
* The nnoremap `<C-s>` (show syntax groups) changed to `<Leader>B`.
* Added the nnoremap `<Leader><Space>` to search backward (`?`).
* Also, better notation for `^C` maps (letters in lowercase).

= 1.6.0 =
* Installed the plugin 'deoplete-go' (autocompletion).
* Installed the plugin 'gocode' (autocompletion).
* Installed the plugin 'deoplete-ternjs' (autocompletion).
* Installed the plugin 'jspc' (autocompletion).
* Installed the plugin 'phpcomplete-extended' (autocompletion).
* Installed the plugin 'clang_complete' (autocompletion).
* Removed the plugin 'phpcompletion'.
* Removed the plugin 'vim-clang'.
* Added the nnoremap `<Leader>g` to toggle `:Gstatus` (fugitive).
* Added ignore git, hg and svn files for CtrlP plugin
* Added more general settings for deoplete plugin.
* Added settings for the plugin 'deoplete-go'.
* Added settings for the plugin 'deoplete-jedi'.
* Added settings for the plugin 'deoplete-ternjs'.
* Added settings for the plugin 'phpcompletion-extended'.
* Added settings for the plugin 'clang_complete'.
* The maps `<C-s>` (expand neosnippet) changed to `<C-d>`.
* The maps `<Leader>ga` (EasyAlign plugin) changed to `gi`.
* The vnoremap `<Leader>ta` (tabularize) changed to `<Leader>x`.
* The vnoremap `<Leader>t1` (tabularize first) changed to `<Leader>X`.
* Added settings for the plugin 'closetag', also for PHP and Ruby.
* Added settings for the plugin 'surround', also for PHP and Ruby.
* Added «omnifunc» settings (better autocompletions).
* Duplicated for Visual modes the function to toggle `^`/`g_`.

= 1.5.7 =
* Added the inoremaps `<Tab>` and `<S-Tab>`.
* Better misspelled words navigation with `ç` and `Ç`.
* The map `<Leader>w?` (suggestions) changed to `<Leader>ç`.
* The map `<Leader>wa` (wrong is good) changed to `<Leader>wg`.
* The map `<Leader>wx` (wrong is wrong) changed to `<Leader>ww`.

= 1.5.6 =
* Removed the nnoremap `<C-c>` (stop pressing message).
* The map `<Leader><Space>` (open CtrlP) changed to `<C-c>`.
* The maps `<Leader>x` (open FZF buffers) have been removed.
* The maps `<Leader>C` (poen FZF commits) changed to `<Leader>Z`.

= 1.5.5 =
* Added and fixed the vnoremap to vimgrep into the visual selection.
* The nnoremap `<Leader>do` (replace to all open files) changed to `<Leader>R`.

= 1.5.4 =
* Added `:copen` to `:vimgrep` nnoremaps.
* Removed the vnoremap to vimgrep into the visual selection.

= 1.5.3 =
* Jump to the search results (grep, vimgrep) in buffers, not in tabs.

= 1.5.2 =
* New toggle function to switch start and end of line with `ñ`.

= 1.5.1 =
* New NERDCommenter settings: default maps disabled.
* The maps `<Leader>x` (toggle comments) changed to `<Leader>c`.
* New Neomake/Syntastic settings: new error signs.
* New CtrlP settings: changed some prompt mappings.
* Added a new map `<Leader>x` to open `:Buffers` (FZF).
* Added a new map `<Leader>C` to open `:Commits` (FZF).
* The maps `<Leader>gu` (toggle Gundo) changed to `<Leader>u`.
* The map `<Leader>cd` (pwd directory) changed to `<Leader>bw`.
* The map `<Leader>by` (copy filepath) changed to `<Leader>by`.
* Added new 'Readline commands' for the Command mode, navigate like in a terminal.
* The maps `<Leader>u` (toggle case) changed to `<Leader><`.
* The function to toggle GitGutterPreviewHunk has been improved.

= 1.5.0 =
* Added a new function: search into a Visual selection.
* Removed the inoremap ';;' (inserts a comma and `<Esc>`).
* The map `<Leader>m` now returns to the last column cursor position.
* Display the current dictionary when we toggle between dictionaries.

= 1.4.4 =
* Removed indentation settings from markdown and mail file types.
* Removed useless nnoremap and vnoremap to `<NOP>` for Windows key.
* Fixed Caps Lock setting: leaving 'Insert Mode' now disables CAPS automatically.

= 1.4.3 =
* Added the setting `nomore` to avoid the pause of listings.

= 1.4.2 =
* Fixed the inoremap `<Leader>p` (paste from clipboard one character left).

= 1.4.1 =
* The maps `<Leader>g` (`:GundoToggle`) changed to `<Leader>gu`.
* Better Neocomplete/Deoplete settings.
* Deleted the inoremap `<C-D>` to delete a line.
* Added the inoremap `<C-D>` to expand Jedi completions.
* Fixed the imap `<C-L>` (Caps Lock) to prevents popup completions.
* Better cursor shape detection for older Vim versions.
* New maps to switch between Vim and Tmux windows even from the Insert/Visual Modes.
* Now easily navigate between characters from Insert Mode with Windows key + hjkl.
* Added the cnoremaps `^X@sh` and `^X@sl` to move one character left and right.
* The nnoremap `<Leader>da` (`:argdo`) changed to `<Leader>**do**`.
* The nnoremap `<Leader>F` now it enters a new line Up.

= 1.4.0 =
* Added a new section: 'Filetype settings'.
* More time delay for `timeoutlen` (3000).
* New inoremap to insert a colon and return to Normal Mode.
* Trigger `InsertLeave` autocmd when using `<C-C>` to escape.
* Echo a warning when pressing `<C-C>` in Normal Mode.
* Disabled Q Mode.
* New cnoreabbrev to open help in a vertical window.
* Installed the plugin 'fzf'.
* Installed the plugin 'tern_for_vim'.
* Installed the plugin 'vim-closetag'.
* Installed the plugin 'targets.vim'.
* Installed the plugin 'vim-sort-motion'.
* Installed the plugin 'vim-expand-region'.
* Installed the plugin 'MatchTagAlways'.
* Installed the plugin 'vim-argwrap'.
* Installed the plugin 'vim-characterize'.
* GitGutter will ignore space at EOL.
* The map `<C-P>` (open CtrlP plugin) changed to `<Leader><Space>`.
* Added the nmap `<C-P>` to toggle preview GitGutter hunks.
* All maps `<C-C>` (toggle comment) changed to `<Leader>x`.
* Added new maps `<Leader>h` to jump to the previous error.
* Added new maps `<Leader>l` to jump to the next error.
* Added new maps `<Leader>z` to open FZF plugin.
* All maps `<C-T>` (toggle Tagbar) changed to `<F4>`.
* All maps `<C-N>` (expand neosnippet) changed to `<C-S>`.
* Added the nnoremap `<C-Z>` to open `:VimShell` or `:terminal`.
* The plugin 'easy-align' now uses the map `<Leader>ga`.
* The plugin 'tabularize' now uses the map `<Leader>t1`.
* The plugin 'expand-region' uses the vmap `v` and `<C-V>`.
* Added settings for the plugin 'MatchTagAlways'.
* Added settings for the plugin 'ArgWrap' and `<Leader>W`.
* The plugin 'vim-instant-markdown' now uses the map `<Leader>M`.
* Added new settings to change the cursor shape.
* To reload the `colorscheme` now it is mapped to `<S-F12>`
* The nnoremap `<C-Z>` (show syntax) changed to `<C-S>`.
* Added the onoremap `af` and `aF` to work on all file.
* Added the nnoremap `<Leader>cf` to copy the filepath to clipboard.
* Added the cnoremap `%%` to expand the path of the current buffer.
* All maps `<F4>` (toggle relative numbers) changed to `<S-F3>`.
* Removed maps to treat long lines as break lines using arrows.
* Removed maps to move lines using arrows.
* Removed maps to duplicate a line using arrows.
* Added four 'Readline commands': `<C-A>`, `<C-E>`, `<C-B>`, `<C-F>`.
* The nnoremap `<Leader><Space>` (`:vimgrep`) changed to `<Leader>v`.
* The vnoremap `<Leader><Space>` (`:vimgrep`) changed to `<Leader>v`.
* The nnoremap `<Leader>v` (`:vimgrep`) changed to `<Leader>V`.
* The nnoremap `<Leader>l` (`:cnext`) changed to `<Leader>n`.
* The nnoremap `<Leader>h` (`:cprev`) changed to `<Leader>N`.
* The nnoremap `<Leader>aa` (`:args *.`) changed to `<Leader>a`.
* The nnoremap `<Leader>as` (`:args **/*.`) changed to `<Leader>A`.
* The nnoremap `<Leader>ad` (`:argdo %s...`) changed to `<Leader>da`.
* The vnoremap `<Leader>x` (toggle case) changed to `<Leader>u`.
* Added the nnoremap `<Leader>u` to toggle case: easier than `~`.
* Added the inoremap `<Leader>u` to toggle case from Insert Mode.
* Added maps to toggle spell dictionary using `<S-F8>`.
* Added the inoremap `<Leader>p` to paste the clipboard from Insert Mode.
* Added the nnoremap `Y` to yank everything from the cursor to the EOL.
* Added the inoremap `<C-D>` to delete de current line from Insert Mode.
* Added the nnoremap `<Leader>o` to isolate the current line.
* Added the nnoremap `<Leader>f` to add a new line below.
* Added the nnoremap `<Leader>F` to join lines.
* Added 'binary' filetype settings.
* Added 'markdown' filetype settings.
* Added 'mail' filetype settings.

= 1.3.0 =
* Installed the plugin 'vim-capslock': use `<C-L>` (Insert Mode) instead of Caps Lock key.
* Removed the nnoremap `<Leader>e` (replace the word under the cursor). Use `ciw` instead.
* The nnoremap `<Leader>h` (`:GitGutterPreviewHunk`) changed to `<Leader>f`.
* The nnoremap `<Leader>l` (toggle the 'loclist') changed to `<Leader>e`.
* The nnoremap `<Leader>p` (`:cprev`) changed to `<Leader>h`.
* The nnoremap `<Leader>n` (`:cnext`) changed to `<Leader>l`.
* Added the nnoremap `<Leader>p` to paste from the clipboard.
* The nnoremap `<Leader>y` changed to `<Leader>ya` (**y**ank **a**ll).

= 1.2.0 =
* Installed the plugin 'vim-instant-markdown'
* Added a map to preview markdown files using `<Leader>z`.
* The vnoremap `<Leader>z` (sorting lines) changed to `<Leader>az`.
* Installed the plugin 'open-browser'.
* Installed the plugin 'MatchTagAlways'.
* Installed the plugin 'Emmet'.

= 1.1.2 =
* Fixed `xterm-keys` for tmux.
* Improved conditional to enable 256 colors, matching to a `$TERM` pattern.
* Turn `viminfo^=%` to comment (don't remember the last open buffer on close).
* Better maps for splitting and resizing windows, so it fits in my `.tmux.conf`.
* Stop resizing all windows when the terminal is resized. Makes no sense.
* Removed the nnoremap `<BS>` (delete the last character).

= 1.1.1 =
* Fixed the map for reloading settings `.vimrc`. Now it uses `$MYVIMRC` var.
* Fixed `DeleteTrailing`, so it works in all files (`*`).
* The nnoremap `<CR>` (search the word under the cursor) changed to `<Leader><CR>`.
* The vnoremap `<CR>` (search the visual selection) changed to `<Leader><CR>`.
* The nnoremap `<Leader><CR>` (disable highlight) changed to `<Leader><BS>`.
* The inoremap `<C-C>` (toggle NERDCommenter) have been deleted.
* The nnoremap `<NUL>` (toggle 'NERDTree') changed to `<C-N>`.
* Jump to the end of line in Insert Mode using `<C-E>`.

= 1.1.0 =
* Installed a pluggin for a smoother scrolling.
* Changed `scrolloff` to 0.
* Set `mousehide` (always, in term and GUI).
* Added a map to reload the current colorscheme.
* Added a map to display syntax highlighting groups.
* Added a map for `:retab` (Visual Mode).
* Added a map to jump to the end of line in the Insert Mode.
* Added ignore case when autocompletes when browsing files.
* Added maps for 'gitgutter' hunks: next, prev and preview.
* Added a map to delete the current file: `<Leader><Del>y`.
* Added a map to reload the current colorscheme: `<Leader><F5>`.
* Removed conditional statement on 'tabularize' settings.
* Rename the title of tmux tabs with the current filename.
* New `showbreak` characters: `│——»`. (4 characters).
* Search the word under cursor without jumping to the next result.
* Search the selected text without jumping to the next result.
* Disabled 'Fly Mode' from plugin 'auto-pairs'.
* Vim-airline's tabline show only the filename instead of path.
* Installed plugins for autocomplete and snippets.
* Added a new category for `:make` settings.
* Installed the plugin 'QuickRun'.
* Set `updatetime` to 250.

= 1.0.0 =
* Initial commit, first version.

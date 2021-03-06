# Bookmark

Bookmark is alfred workflow which enables to manage and search bookmark.
You can add browser's URL to bookmark, add multiple tags to it, and search it.

[![youtube](https://img.youtube.com/vi/ImXADq0mBRM/0.jpg)](https://www.youtube.com/watch?v=ImXADq0mBRM)

This workflow works *without* pinboard.in account.
You can link pinboard.in account with this workflow also.

Download: https://github.com/jmjeong/alfred-extension/blob/master/bookmark/bookmark.alfredworkflow?raw=true

After integrating pinboard.in account, you can download the data pinboard.in using `pbreload`
command.

Bookmark workflow provides...

- Add bookmark - add frontmost browser's url to bookmark
  - In adding bookmark, you can assign multiple tags.
- Search bookmark
- Delete bookmark
- Assign [private], [star] attribute in bookmark
  - You can narrow the search space using this attribute
- Several sort options
  - launch count
  - accessed
  - added
- Pinboard integration
  - **Your local bookmarks are replaced with pinboard.in data after integration**
  - After integration, add/delete operation is synced with pinboard.in
  - You can download pinboard.in bookmark  with `pbreload` command.

### Install

You need to **set key manually** after installing bookmark.

- Cmd-Shift-Ctrl-P : Workflow launch (Search condition follows setting)
- Cmd-Shift-Ctrl-K(!) : Search every bookmark temporary (Ignore settings)
- Cmd-Shift-Ctrl-L(\*) : Search marked bookmark only
- Cmd-Shift-Ctrl-;(+) : Add bookmark (**This key is valid only when browser is the frontmost window**)

### Assign attribute to bookmark

You can change search condition from setting menu(**_**).

- private : Toggle with [shift] modifier key
- star : Toggle with [ctrl] modifier
- You can change attributes of multiple bookmarks of the same tag. 
	- ctrl: set mark, shift: unset mark, alt: set private, cmd: unset private

### Setting 

- mark[filter]
- private[filter] 
- sort
	- accessed, launch_count, time
	- launch_count, accessed, time
	- time, accessed

### Command 

- bm (ctrl-shift-cmd-p) 
	- ! (ctrl-shift-cmd-k) - Search every bookmarks (ignores search condition in setting)
	- \* (ctrl-shift-cmd-l) - Search marked bookmark only
	- \+ (ctrl-shift-cmd-;) - Add URL to bookmark
	- \# - Tag search

- For entries
  - Enter : launch bookmark
  - Ctrl : toggle mark attribute
  - Shift : toggle private attribute 
  - Alt : delete bookmark
  - Cmd : copy URL

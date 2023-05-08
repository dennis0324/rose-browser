<br>
<h3 align=center>Rose Browser</h3>

<p align=center>
Small browser built on gtk and webkit. <br>
</p>

## ⚡️ Requirements
  - webkitgtk (4.0|6.0)
  - gtk (3|4)
  
  - Video and audio:
  	- gst-plugins-bad
	- gst-plugins-base
	- gst-plugins-good
	- gst-libav
	- gstreamer-vaapi (gpu acceleration)
	
## ✨ Features
  - supports the lastes webkit and gtk features
  - configuration via lua modules
  
## 📦 Installation
```sh
$ git clone https://github.com/mini-rose/rose && cd rose
$ (doas|sudo) GTK=(3|4) BUILDTYPE=RELEASE make install
```

## 🚀 Usage
Configure rose in ~/.config/rose/init.lua:
```lua
rose.startpage = "https://duckduckgo.com"

rose.webkit = {
	gestures = true
}
```

## Work in progress

For now i recommend to use old rose (at "old" branch).

Moved to main becouse old branch will not be maintained.

## 📝 TODO
Here is a list of tasks to be completed for the next releases of the Rose:

- [ ] - Implement keyboard shortcuts support in Lua: The browser needs to be able to handle user-defined keyboard shortcuts for various functions such as opening a new tab, closing a tab, or switching between tabs. This can be achieved by using the Lua C API to register keyboard shortcut handlers.

- [ ] - Reintroduce functionality from previous versions: There are some features that were available in previous versions of the browser that are currently missing. These features need to be reimplemented, including the ability to customize the browser's user interface, tabs etc.

- [ ] - Implement split view: The browser needs to support split view, which allows users to view multiple web pages side by side in the same window. This can be implemented by using the browser's existing tab system and creating multiple webview widgets to display the content.

- [ ] - Implement vertical tab view: Another useful feature that should be added is vertical tab view, which displays tabs in a vertical list on the side of the window instead of across the top.

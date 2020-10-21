# electron-quick-start

**Clone and run for a quick way to see Electron in action.**

This is a minimal Electron application based on the [Quick Start Guide](https://electronjs.org/docs/tutorial/quick-start) within the Electron documentation.

**Use this app along with the [Electron API Demos](https://electronjs.org/#get-started) app for API code examples to help you get started.**

A basic Electron application needs just these files:

- `package.json` - Points to the app's main file and lists its details and dependencies.
- `main.js` - Starts the app and creates a browser window to render HTML. This is the app's **main process**.
- `index.html` - A web page to render. This is the app's **renderer process**.

You can learn more about each of these components within the [Quick Start Guide](https://electronjs.org/docs/tutorial/quick-start).

## To Use

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/electron/electron-quick-start
# Go into the repository
cd electron-quick-start
# Install dependencies
npm install
# Run the app
npm start
```

Note: If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.

## Resources for Learning Electron

- [electronjs.org/docs](https://electronjs.org/docs) - all of Electron's documentation
- [electronjs.org/community#boilerplates](https://electronjs.org/community#boilerplates) - sample starter apps created by the community
- [electron/electron-quick-start](https://github.com/electron/electron-quick-start) - a very basic starter Electron app
- [electron/simple-samples](https://github.com/electron/simple-samples) - small applications with ideas for taking them further
- [electron/electron-api-demos](https://github.com/electron/electron-api-demos) - an Electron app that teaches you how to use Electron
- [hokein/electron-sample-apps](https://github.com/hokein/electron-sample-apps) - small demo apps for the various Electron APIs

## License

[CC0 1.0 (Public Domain)](LICENSE.md)

# FEATURE IDEALS AND PROJECT GOALS

## Features Overview:
will be RTF, and accept external linking, but minimal use of connectivity to outside apps
except for background email or texting for reminders and scheduling purposes

### Persistently saves
### Auto format features
	-assume an indent is a block (copy indentation for all newlines until second backspace is entered)
### Email lists as reminders
	-have a menu to schedule this
	-hotkey for both line reminder or list reminder
### Words
	-Smallest tracked pieces, any space detected breaks the word
	-They are only tracked in relation to lines
	-word data points:
		-parent line
		-location in line
### Lines
	-The most commonly manipulated chunk of data
	-Treated as the building block of lists
	-every "enter" keystroke saves a history of the line
		-line data points
			-number of children
			-time last edited
			-type of edit
			-time first created
### Phrase
	Any part of a line selected less than a whole line
	used in hotkeys
	not stored in database
### Lists
	Created with a hotkey
	Stored in a hover-collapsable / hidden or possibly hotkey activated menu
	Marked list moved to the menu and stored at bottom of page
	Menued lists display isolated when selected
	Automatically moved to bottom of page in shrunken, "blocks" that are "stacked" and "stackable"(future / maybe?)
	Add option for type of list - [today/urgent ----> can wait], have urgent lists frozen at top of page until 			complete or de-prioritized
	Tabs
		
### Dumpster
	Trashed items are saved in history that can be viewed
	Trash views can be filtered by Tags,colors, lists, etc
### Tags
	hotkey activates line added to tag
	list can also be given a parent tag
	Tags can be viewed similar to links, tree view, parents--> children
		select tag from tree view to view in "tag list" mode
### Text as object (maybe)
### Color coding
	hotkey select current line and choose from menu (keystroke) for category color
	adaptive color modes (dark mode changing tone of colors, slider)
		bg (white to black)
		color codes (tones appropriate for bg)
		perhaps a few profiles as well (soft, hard, pastel etc)
### Internal linking --> lists and graphs
	mark with "\\"
### Hotkeys
	hk display list of hotkeys
	hk create list	
	hk add line to list
	hk color code line
	hk display list menu
	hk open menu in tab
	hk select tab
	hk cycle back / forth tabs
	hk display link tree for current list
	hk display link tree for document
	hk display colored lists by timestamp
	hk send selected lines to end of current document
	hk move currentlines up
	hk move currentlines down
	hk select cursored word
	hk web search selected phrase
	hk set reminder, choose list or current line, set date/time/frequency
#### Ideal text navigation features
	all alterable in settings
	shift, ctrl shift standard
	ctrl up down start and end of line

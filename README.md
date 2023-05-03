# AlfreDo
An Alfred Workflow for [Todoist](https://todoist.com/)

<a href="https://github.com/giovannicoppola/alfreDO/releases/latest/">
<img alt="Downloads"
src="https://img.shields.io/github/downloads/giovannicoppola/alfreDo/total?color=purple&label=Downloads"><br/>
</a>

![](images/CreateTask.gif)

<!-- MarkdownTOC autolink="true" bracket="round" depth="3" autoanchor="true" -->

- [Motivation](#motivation)
- [Setting up](#setting-up)
- [Basic Usage](#usage)
- [Known Issues](#known-issues)
- [Acknowledgments](#acknowledgments)
- [Changelog](#changelog)
- [Feedback](#feedback)

<!-- /MarkdownTOC -->


<h1 id="motivation">Motivation ✅</h1>

- Quickly list, search, and act on your Todoist tasks 
- Add new tasks to Todoist through Alfred



<h1 id="setting-up">Setting up ⚙️</h1>

### Needed
- Alfred 5 with Powerpack license
- A [Todoist](https://todoist.com/) account
- Python3 (howto [here](https://www.freecodecamp.org/news/python-version-on-mac-update/))
- Download `AlfreDo` [latest release](https://github.com/giovannicoppola/alfredo/releases/latest)



## Default settings 
- In Alfred, open the 'Configure Workflow' menu in `AlfreDo` preferences
 	- set the Todoist API token (login into your account, then generate it [here](https://todoist.com/app/settings/integrations/developer))
- *Optional*:	
	- set the keyword (or hotkey) to show: 
		1. Tasks due today (default: `!1`)
		2. Overdue (default: `!2`)
		3. All tasks (default: `!3`)
	- set the keyword (or hotkey) to force-refresh (default: `todoist::refresh`)
	- set the keyword (or hotkey) to create a new task (default: `!!!`)
	- set refresh rate (in days). Default: `1`
		- Recommended `0` (refresh every time) or `1` if you use Todoist often from browser, mobile etc. 
		- Database is automatically refreshed when a task is created, completed, or rescheduled.
		- Refresh can be forced using a keyword (default: `todoist::refresh`) or hotkey.
	- show Karma daily and weekly goals? Default: `yes`


<h1 id="usage">Basic Usage 📖</h1>

## Searching your tasks 🔍
- launch with keyword or custom hotkey. You can start from 1) tasks due today, 2) tasks overdue, or 3) all tasks
- Use multiple strings, or label/projects to refine search. Use `@` to enter one or more labels, `#` to enter a project. 
- Once a task is selected, you can do one of three things: 
	- `enter` ↩️ will open the task on [Todoist](https://todoist.com/)
	- `shift-enter` ⇧↩️ will complete the task
	- `ctrl-enter` ^↩️ will open a menu to reschedule the task. Choose one of the options, or enter a number of days. You can also use `w` or `m` after the number to enter weeks and months, respectively (e.g. `10w` will reschedule in 10 weeks)
	

## Creating new tasks ⭐
- launch with keyword (default: `!!!`) or hotkey. Use `@` to enter one or more labels, `#` to enter a project (`Inbox` will be used if none entered), `due:` to enter a due date. As in reschedule, choose one of the options, or enter a number of days. You can also use `w` or `m` after the number to enter weeks and months, respectively (e.g. `10w` will set a due date in 10 weeks)  
- Universal Action: new highlights can be created by selecting text in any app, then launching Universal Actions and selecting `Create a new Todoist task`. 


## Database refresh 🔄
- will occur according to the rate in days set in `AlfreDo` preferences, after a task is created, completed, or rescheduled, or...
	- `todoist::refresh` to force database refresh


<h1 id="known-issues">Limitations & known issues ⚠️</h1>

- None for now, but I have not done extensive testing, let me know if you see anything!



<h1 id="acknowledgments">Acknowledgments 😀</h1>

- Thanks to the [Alfred forum](https://www.alfredforum.com) community!
- Icons from [Flaticon](https://www.flaticon.com/): 
	- https://www.flaticon.com/free-icon/overdue_6534474
	- https://www.flaticon.com/free-icon/calendar_6816638
	- https://www.flaticon.com/free-icon/project-management_4844342
	- https://www.flaticon.com/free-icon/task_2098402
	
	
<h1 id="changelog">Changelog 🧰</h1>

- 05-03-2023: version 0.1


<h1 id="feedback">Feedback 🧐</h1>

Feedback welcome! If you notice a bug, or have ideas for new features, please feel free to get in touch either here, or on the [Alfred](https://www.alfredforum.com) forum. 

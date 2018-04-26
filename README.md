![Built with love](http://forthebadge.com/images/badges/built-with-love.svg)
# Tusker
A dead simple todo manager in *less than 100 lines* of Bash.  
For those who live in the terminal.

### Installation
Just download the executable from [releases](https://github.com/coderick14/tusker/releases) and put it in your `$PATH`. Period.  
Type `tusker help` to get started.

### Usage
- Add a task
```
tusker add "The task that I would've forgotten"
```
- Show current tasks *[ID, Status, Description, CreatedAt]*
```
tusker show
     1	❌      Collect laundry                  25 April 2018 11:53:21
     2	❌      Collect NOC certificate          25 April 2018 11:53:23
     3	❌      Fill rems                        25 April 2018 11:53:25
```
- Mark a task as done
```
tusker check 1
tusker show
     1	✓      Collect laundry                  25 April 2018 11:53:21
     2	❌      Collect NOC certificate          25 April 2018 11:53:23
     3	❌      Fill rems                        25 April 2018 11:53:25
```
- Mark a task as undone
```
tusker uncheck 1
tusker show
     1	❌      Collect laundry                  25 April 2018 11:53:21
     2	❌      Collect NOC certificate          25 April 2018 11:53:23
     3	❌      Fill rems                        25 April 2018 11:53:25
```
- Delete a task from the list
```
tusker del 2
tusker show
     1	❌      Collect laundry                  25 April 2018 11:53:21
     2	❌      Fill rems                        25 April 2018 11:53:25
```

### Tip
Add `tusker show` at the end of your `.bashrc`, `.zshrc` or `config.fish` to get reminded about your pending tasks whenever you fire up a terminal.

### Why tusker?
- No dependencies. Seriously.
- Simple. So that you can focus on what's important, which is **finishing your tasks**.

### Features and contributions
`tusker` was written the night before my semester examination because I kept forgetting the topics I had skipped. So if you'd like to report a bug or add a feature, feel free to raise an issue or send a pull request!!

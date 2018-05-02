![Built with love](http://forthebadge.com/images/badges/built-with-love.svg)
# Tusker
A dead simple todo manager in *less than 100 lines* of code.  
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

- Delete multiple tasks from the list
```
tusker del 1 3
tusker show
     1	❌      Collect NOC certificate          25 April 2018 11:53:23
```
### What's the difference between `check` and `del`?
Use `del` if you'd *never* like to look back at a completed task.  
Use `check` if you want the satisfaction of seeing the ✓  beside your completed task for a while.
Also, you can `uncheck` it anytime, in case you missed out on something :(

### Tip
Add `tusker show` at the end of your `.bashrc`, `.zshrc` or `config.fish` to get reminded about your pending tasks whenever you fire up a terminal.

### Why tusker?
- No dependencies. Seriously.
- Simple. So that you can focus on what's important, which is **finishing your tasks**.

### Features and contributions
`tusker` was written a couple of nights before my semester examination because I kept forgetting the topics that I had skipped. So if you find a bug or you'd like to add a feature, feel free to raise an issue or send a pull request!!

### Note
I've tried to make the script *POSIX compatible*. However, if you do face an issue regarding that, please raise an issue. Or send a PR *(even better)*!!

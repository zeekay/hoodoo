# hoodoo
Command line todo.

```
description
  hoodoo is a task management app. tasks can be tagged, searched, sorted.

commands available
  add <name> #<tag>    add a new task
    alias: +
    opt: created=<date> due=<date> done=True/False, tags

  edit <index>         edit a task
    alias: e
    opt: name=<name> created=<date> due=<date> done=True/False, tags

  del <index>          delete a task
    alias: rm, -

  done <index>         mark task as done
    alias: x

  list                 list tasks
    alias: ls

  search <query>       search through tasks by name or tag
    alias: default action if arguments do not match options

  set <name>           switch to another set, if it does not exist create it

  sets                 list sets

notes:
  to be able to tag without quotes with most shells you will
  probably need to disable globbing. for zsh add this alias:
  alias hoodoo='noglob python path/to/hoodoo.py'
```

### ZSH
Autocompletion available for ZSH see: [zsh/_hoodoo](zsh/hoodoo).

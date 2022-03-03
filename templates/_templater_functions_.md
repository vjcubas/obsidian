---
title: _templater_functions_
---
## Internal Functions
### Config Module
tp.confg.active_file: **<% tp.config.active_file %>**
tp.config.run_mode: **<% tp.config.run_mode %>**
tp.config.target_file: **<% tp.config.target_file %>**
tp.confit.template_file: **<% tp.config.template_file %>**
### Date Module
tp.date.now(): **<% tp.date.now() %>**

tp.date.now() *with format*: **<% tp.date.now("MMMM Do, YYYY") %>**

tp.date.now() *with format ISO-8601*: **<% tp.date.now("YYYY-MM-DD") %>**

tp.date.now() *-n days*: **<% tp.date.now("MMMM Do, YYYY", -3) %>**

tp.date.now() *+n days*: **<% tp.date.now("MMMM Do, YYYY", 3) %>**

tp.date.now() *n weeks back*: **<% tp.date.now("MMMM Do, YYYY", "P-1W") %>**

tp.date.now() *n weeks forward*: **<% tp.date.now("MMMM Do, YYYY", "P1W") %>**

tp.date.now() *n months back*: **<% tp.date.now("MMMM Do, YYYY", "P-1M") %>**

tp.date.now() *n months forward*: **<% tp.date.now("MMMM Do, YYYY", "P1M") %>**

tp.date.now() *n years back*: **<% tp.date.now("MMMM Do, YYYY", "P-1Y") %>**

tp.date.now() *n years forward*: **<% tp.date.now("MMMM Do, YYYY", "P1Y") %>**

tp.date.tomorrowl(): **<% tp.date.tomorrow("MMMM Do, YYYY") %>**

tp.date.yesterday(): **<% tp.date.yesterday("MMMM Do, YYYY") %>**

tp.date.weekdayl() *Monday*: **<% tp.date.weekday("MMMM Do, YYYY",  0) %>**

tp.date.weekdayl() *Sunday*: **<% tp.date.weekday("MMMM Do, YYYY",  6) %>**

tp.date.weekdayl() *next week's Monday*: **<% tp.date.weekday("MMMM Do, YYYY",  7) %>**

### Moment Object
moment().format() *today is *: **<% moment().format("[Today is] dddd") %>**

### File Module
File title: **<% tp.file.title %>**
## Dynamic Commands
**Last modified date:** <%+ tp.file.last_modified_date() %>
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
```ad-example
title: tp.date.now()
collapse: close
<span style="color:cyan">Examples:</span>
1. **tp.date.now():** <% tp.date.now() %>
1. **tp.date.now("MMMM Do, YYYY"):** <% tp.date.now("MMMM Do, YYYY") %>
1. **tp.date.now("YYYY-MM-DD") *ISO-8601*:** <% tp.date.now("YYYY-MM-DD") %>
1. **tp.date.now("MMMM Do, YYYY", 3:):** <% tp.date.now("MMMM Do, YYYY", 3) %>
1. **tp.date.now("MMMM Do, YYYY", -3:):** <% tp.date.now("MMMM Do, YYYY", -3) %>
1. **tp.date.now("MMMM Do, YYYY", "P1W"):** <% tp.date.now("MMMM Do, YYYY", "P1W") %>
1. **tp.date.now("MMMM Do, YYYY", "P-1W"):** <% tp.date.now("MMMM Do, YYYY", "P-1W") %>
1. **tp.date.now(tp.date.now("MMMM Do, YYYY", "P1W") ):** <% tp.date.now("MMMM Do, YYYY", "P1W") %>
1. **tp.date.now(tp.date.now("MMMM Do, YYYY", "P-1W") ):** <% tp.date.now("MMMM Do, YYYY", "P-1W") %>
1. **tp.date.now(tp.date.now("MMMM Do, YYYY", "P1M") ):** <% tp.date.now("MMMM Do, YYYY", "P1M") %>
1. **tp.date.now(tp.date.now("MMMM Do, YYYY", "P-1M") ):** <% tp.date.now("MMMM Do, YYYY", "P-1M")  %>
1. **tp.date.now(tp.date.now("MMMM Do, YYYY", "P1Y") ):** <% tp.date.now("MMMM Do, YYYY", "P1Y") %>
1. **tp.date.now(tp.date.now("MMMM Do, YYYY", "P-1Y") ):** <% tp.date.now("MMMM Do, YYYY", "P-1Y")  %>
```
```ad-example
title: tp.date.tomorrow()
collapse: close
<span style="color:cyan">Examples:</span>
1. **tp.date.tomorrow("MMMM Do, YYYY"):** <% tp.date.tomorrow("MMMM Do, YYYY") %>
```
```ad-example
title: tp.date.yesterday()
collapse: close
<span style="color:cyan">Examples:</span>
1. **tp.date.yesterday("MMMM Do, YYYY"):** <% tp.date.yesterday("MMMM Do, YYYY") %>
```
```ad-example
title: tp.date.weekday()
collapse: close
<span style="color:cyan">Examples:</span>
1. **tp.date.weekday("MMMM Do, YYYY", 0):** <% tp.date.weekday("MMMM Do, YYYY", 0) %>
1. **tp.date.weekday("MMMM Do, YYYY", 1):** <% tp.date.weekday("MMMM Do, YYYY", 1) %>
1. **tp.date.weekday("MMMM Do, YYYY", 2):** <% tp.date.weekday("MMMM Do, YYYY", 2) %>
1. **tp.date.weekday("MMMM Do, YYYY", 3):** <% tp.date.weekday("MMMM Do, YYYY", 3) %>
1. **tp.date.weekday("MMMM Do, YYYY", 4):** <% tp.date.weekday("MMMM Do, YYYY", 4) %>
1. **tp.date.weekday("MMMM Do, YYYY", 5):** <% tp.date.weekday("MMMM Do, YYYY", 5) %>
1. **tp.date.weekday("MMMM Do, YYYY", 6):** <% tp.date.weekday("MMMM Do, YYYY", 6) %>
1. **tp.date.weekday("MMMM Do, YYYY", 7):** <% tp.date.weekday("MMMM Do, YYYY", 7) %>
1. **tp.date.weekday("MMMM Do, YYYY", 8):** <% tp.date.weekday("MMMM Do, YYYY", 8) %>
```
### Moment Object
```ad-example
title: moment().format()
collapse: close
<span style="color:cyan">Examples:</span>
1. **moment().format("[Today is] dddd"):** <% moment().format("[Today is] dddd") %>
1. **moment("01-2022", "MM-YYYY").daysInMonth():** <% moment("01-2022", "MM-YYYY").daysInMonth() %>
```

### File Module
```ad-example
title: tp.file.*
collapse:close
<span style="color:cyan">Examples:</span>
1. **tp.file.title:** <% tp.file.title %>
1. **tp.file.creation_date("MMMM Do, YYYY"):** <% tp.file.creation_date("MMMM Do, YYYY") %>
```
File title: **<% tp.file.title %>**
## Dynamic Commands
**Last modified date:** <%+ tp.file.last_modified_date() %>
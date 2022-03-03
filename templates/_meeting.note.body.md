<%
let qcFileName = await tp.system.prompt("Note Title")
let qcTopic = await tp.system.prompt("Topic")
titleName = qcFileName + " " + tp.date.now("YYYY-MM-DD")
await tp.file.rename(titleName)
await tp.file.move("/meetings/" + titleName);
-%>
---
title: <% qcFileName %>
date: <% tp.file.creation_date("YYYY-MM-DD HH:mm:ss") %>
tags: [meeting, ]
topic: <% qcTopic %>
---

<% tp.file.cursor() %>
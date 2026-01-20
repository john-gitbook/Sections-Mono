---
title: code blocks
---

Task Reminder

{% if page.vars.code === 'task_reminder' %}
```javascript
try {
  let data = await $schedule.create({
    name: "task_reminder",
    data: {
      task_id: 100001
    },
    schedule_at: "2018-06-10T07:00:00.860Z",
  });
}
catch (error) {
  console.log(error)
}
```
{% endif %}

Ticket Reminder

{% if page.vars.code === 'ticket_reminder' %}
```javascript
try {
  let data = await $schedule.create({
    name: "ticket_reminder",
    data: {
      ticket_id: 100001
    },
    schedule_at: "2018-06-10T07:00:00.860Z",
  });
}
catch (error) {
  console.log(error)
}
```
{% endif %}




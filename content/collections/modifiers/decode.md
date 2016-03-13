---
types:
  - utility
id: 1fd780fd-ae92-4e73-9513-2b9c845976e9
---
Convert all HTML entities to their applicable characters via PHP's [html_entity_decode()][decode] function. Will convert both double and single quotes. This is the opposite of the [entities](#entities) modifier.

```.language-yaml
string: "I'll \"eat\" the <b>bacon</b> now";
```

```
{{ string | decode }}
```

```.language-output
I'll "eat" the <b>bacon</b> now
```

[decode]: http://php.net/manual/en/function.html-entity-decode.php
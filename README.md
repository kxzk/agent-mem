<h3 align="center">🧠 agent mem</h3>

<br>
<br>

```text
mem – manage agent task / note memory

[usage]
  mem -a "<task text>"           add new task
  mem -n "<note text>"           add new note
  mem -l task|note|done          list entries by type
  mem -d <id>                    mark task <id> as done
  mem -r <id>                    remove note <id>
  mem -s <pattern>               search open tasks for text
  mem -h                         show this help

[details]
  • ids auto-increment from the highest existing id per type
  • all writes are wrapped in flock(1) so concurrent agents cannot corrupt
    the file

[examples]
  mem -a "write allocator benchmark"
  mem -d 7
  mem -l task
  mem -s zig
```

<br>
<br>

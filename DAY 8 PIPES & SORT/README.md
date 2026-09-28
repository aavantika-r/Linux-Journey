# Linux Pipes (`|`)

Part of my **Linux Administration + Cloud + DevOps** learning journey.

## What I Learned

### Pipe `|`

Used to pass the output of one command to another command.

```bash
command1 | command2
```

Example:

```bash
cat app.log | grep "ERROR"
```

### Multiple Pipes

Commands can be chained together:

```bash
cat app.log | grep "ERROR" | head
```

### `sort`

Sorts text output:

```bash
sort file.txt
```

### `sort -u`

Sorts and removes duplicate lines:

```bash
sort -u servers.txt
```

### `sort -r`

Sorts in reverse order:

```bash
sort -r servers.txt
```

### `sort -n`

Sorts numerical values correctly:

```bash
sort -n numbers.txt
```

Example:

```text
Input:
20
5
100
2
50

Output:
2
5
20
50
100
```

## Mini Lab — Disk Usage Sorting

Simulated a Linux server monitoring output containing disk-usage percentages:

```text
75
12
95
40
8
100
```

Used:

```bash
sort -n disk-usage.txt
```

Output:

```text
8
12
40
75
95
100
```

### Troubleshooting Tested

Incorrect:

```bash
sort disk-usage.txt
```

Correct:

```bash
sort -n disk-usage.txt
```

**Reason:** Default `sort` compares values as text; `-n` performs numerical sorting.

## DevOps Relevance

Pipes are useful for:

* Filtering application logs
* Processing Linux command output
* Investigating server issues
* Organizing monitoring data
* Building command pipelines for automation

## Key Takeaways

* `|` passes command output to another command.
* `grep` filters text.
* Multiple pipes can create processing pipelines.
* `sort -u` removes duplicates.
* `sort -r` reverses sorting.
* `sort -n` sorts numerical values correctly.

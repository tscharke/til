# Using awk

In many situations, I need some tools to make my life easier. On this page I describe `awk` or better some case I needed awk for.

## What is awk

It's a scripting language for editing and analyzing texts. Input data is always processed line by line.

## What a name

The name is derived from the initials of the developers

- Alfred V. **A**ho
- Peter J. **W**einberger and
- Brian W. **K**ernighan

## Cases

Give is a string, separated by new lines with a tuple of values (e.g. ColumnX, ValueX, etc.).

| No# |     |     |     |
| --- | --- | --- | --- |
| 1   | C1  | C2  | C3  |
| 2   | V1  | V2  | V3  |
| 3   | 1   | 2   | 3   |
| 4   | A   | B   | C   |

### Print values of the 2. column

To print out the value of the second columns only:

```bash
echo "C1 C2 C3\nV1 V2 V3\n1 2 3\nA B C" | awk '{ print $2 }'

C2
V2
2
B
```

Changing the paramater `$2` (e.g. to `$1`, `$3`) prints out the _first_ or the _third_ column.

### Print values of the 2. column and 2. row

What I describe as a row named the oficial documentation **record**.

To print out a value of a specific record (e.g. the second), we can use `NR` (**N**umber of **R**ecords) like this:

```bash
echo "C1 C2 C3\nV1 V2 V3\n1 2 3\nA B C" | awk 'NR==2 { print $2 }'

V2
```

# 🚀 `run $command`

Test Function or Command Output.

---

Download the [latest version](https://github.com/bx-sh/run.sh/archive/v0.2.0.tar.gz)

```sh
$ source "run-command.sh"
```

---

#### `run`

The `run` function returns the underlying command or function's exit or return code

```sh
$ run ls

$ echo $?
0
```

The command does not run in a subshell. If you would like to run the command in a subshell:

```sh
$ run -- ls

$ echo $?
0
```

#### `$EXIT_CODE`

The command or function's return code is put into an `$EXIT_CODE` variable

```sh
$ echo "$EXIT_CODE"
0
```

#### `$STDOUT`

The command or function's output is put into a `$STDOUT` variable

```sh
$ echo "$STDOUT"
foo
bar
```

#### `$STDERR`

The command or function's standard error is put into a `$STDERR` variable

```sh
$ echo "$STDERR"
```

#### `$OUTPUT`

The command or function's `STDOUT` and `STDERR` are both put into an `$OUTPUT` variable

```sh
$ echo "$OUTPUT
foo
bar
```

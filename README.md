# 🚀 `run $command`

Test Command Output.

---

```sh
$ source "run-command.sh"
```

The `run` function returns the underlying command's exit or return code

```sh
$ run ls

$ echo $?
0
```

The command or function's return code is put into an `$EXIT_CODE` variable

```sh
$ echo "$EXIT_CODE"
0
```

You can also get the return code by calling the `EXIT_CODE` function

```
$ EXIT_CODE
0
```

The command or function's output is put into a `$STDOUT` variable

```sh
$ echo "$STDOUT"
foo
bar

You can also get the output by calling the `STDOUT` function

```sh
$ STDOUT
foo
bar
```

The command or function's standard error is put into a `$STDERR` variable

```sh
$ echo "$STDERR"
```

You can also get the standard error by calling the `STDERR` function

```sh
$ STDERR
```

The command or function's `STDOUT` and `STDERR` are both put into an `$OUTPUT` variable

```sh
$ echo "$OUTPUT
foo
bar
```

You can also get the combined `STDOUT` and `STDERR` by calling the `OUTPUT` function

```sh
$ OUTPUT
foo
bar
```

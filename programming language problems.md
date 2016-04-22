# 1. Date Calculator

A command line calculator for simple date expressions.

```sh
$ dc "2016-04-22 + 7"
2016-04-29
```

With `-c` or `--calendar`, the computation is performed in the given calendar.

```sh
$ dc -c weekdays "2016-04-22 + 7"
2016-05-03
```

The calendar is one of "all", "weekdays", "weekends", or the path to a calendar file.

The expression grammar is as follows:

- `DATE` := an ISO 8601 date
- `OFFSET` := a signed integer offset in days
- `DATE-EXPR` := `DATE-EXPR + OFFSET` | `DATE-EXPR - OFFSET` 
- `DATE-DIFF` := `DATE-EXPR - DATE-EXPR`
- `DATE-RANGE` := `DATE-EXPR .. DATE-EXPR` | `DATE-EXPR ... DATE-EXPR`
- `EXPR` := `DATE-EXPR` | `DATE-DIFF` | `DATE-RANGE`

The output is a single date, or an offset, or a sequence of dates, one per line.


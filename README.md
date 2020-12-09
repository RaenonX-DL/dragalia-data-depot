# dragalia-data-depot

This stores all dumped and partially parsed Dragalia Lost data.

Data will be further parsed and processed by [dragalia-data-parse][parser] for the use of [DL info website][DL-info].

[DL-info]: http://dl.raenonx.cc
[parser]: https://github.com/RaenonX-DL/dragalia-data-parse

------

## Data updating procedure

1. Push the new data. The commit message should follow the [naming convention below](#commit-naming).

2. Add a tag for the cUpdate READMEommit (for easier access & searching). 
The tag name should follow the [naming convention below](#tag-naming).

------

# Conventions

## Commit naming

Commits should be named in the following format:

```
2020/11/23 12:00 AM - 08NV7KO9YyXMIlB2
```

## Tag naming

Tags should be named in the following format:

```
2020.11.23-08NV7KO9YyXMIlB2
```

> Note that the timezones for all the timestamps should be UTC +8 (Taipei Standard Time).

-------

# Notes

For pipeline, monitor the tag added/updated event instead, because it is possible that there are some commits for updating another non-asset files.
For example, update for the README.md, which creates a commit but will not create a tag.

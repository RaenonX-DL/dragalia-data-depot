# dragalia-data-depot

[![Depot-latest-tag]][Depot-tags]
![Depot-size]
[![Depot-deploy-workflow]][Depot-deploy-workflow-link]
[![Depot-deploy-repo]][Depot-deploy-repo-link]
[![Depot-deploy-push]][Depot-deploy-push-link]

This stores all dumped and pre-processed Dragalia Lost assets.

These assets will be further parsed and processed by [dragalia-data-parse][parser] for the use of [DL info website][DL-info].

[DL-info]: http://dl.raenonx.cc
[parser]: https://github.com/RaenonX-DL/dragalia-data-parse

[Depot-size]: https://img.shields.io/github/repo-size/RaenonX-DL/dragalia-data-depot
[Depot-deploy-workflow]: https://github.com/RaenonX-DL/dragalia-data-depot/workflows/Resource%20Deployment%20(Workflow%20Dispatch)/badge.svg
[Depot-deploy-workflow-link]: https://github.com/RaenonX-DL/dragalia-data-depot/actions?query=workflow%3A%22Resource+Deployment+%28Workflow+Dispatch%29%22
[Depot-deploy-repo]: https://github.com/RaenonX-DL/dragalia-data-depot/workflows/Resource%20Deployment%20(Repository%20Dispatch)/badge.svg
[Depot-deploy-repo-link]: https://github.com/RaenonX-DL/dragalia-data-depot/actions?query=workflow%3A%22Resource+Deployment+%28Repository+Dispatch%29%22
[Depot-deploy-push]: https://github.com/RaenonX-DL/dragalia-data-depot/workflows/Resource%20Deployment%20(Push)/badge.svg
[Depot-deploy-push-link]: https://github.com/RaenonX-DL/dragalia-data-depot/actions?query=workflow%3A%22Resource+Deployment+%28Push%29%22
[Depot-latest-tag]: https://img.shields.io/github/v/tag/RaenonX-DL/dragalia-data-depot?label=Manifest%20version
[Depot-tags]: https://github.com/RaenonX-DL/dragalia-data-depot/tags

------

## Data updating procedure

1. Push the new data. The commit message should follow the [naming convention below](#commit-naming).

2. Add a tag for the commit (for easier access & searching). 
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

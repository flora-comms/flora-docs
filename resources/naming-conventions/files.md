# File Naming Conventions

## Rely on File Heirarchy

Windows is silly and has a maximum path length of 256 bytes. This can cause issues especially when compiling software and committing to git.
Use the parent folder heirarchy as part of the name to minimize path length while optimizing file structure organization, where the level of "abstraction" for describing what the file is about decreases the deeper into the tree you go.

For example, the file name of this file is "file.md". That makes no sense out of context, but consider the full file path: 
"$ROOT/flora-docs/resources/naming-conventions/files.md"
Now the purpose of the file is self-evident. It is supplemental documentation for the FLoRa project (flora-docs/resources), and it describes the standard for naming files (naming-conventions/files).
It belongs to all the categories described by its parent folders.

***Note of caution***: Be careful that the number of parent folders doesn't get out of hand. Like any plant, pruning the file tree is an important part of keeping it healthy.

## kebab-case-format

All files and folders should be named using kebab-case, unless they require another naming format (eg. the preproom order form wants CamelCase_JoinedWithSnakeCase_Plus_OrderIdNumber)
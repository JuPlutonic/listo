# Listo

This is a command line tool that help you archive and show items.

Made with <3 by @olistik

## License

GNU General Public License (GPL) version 3

[gnu.org](https://www.gnu.org/licenses/gpl-3.0.txt)

## Requirements

This is a Ruby script, tested against the following interpreter version:

```
ಠ_ಠ ruby -v
ruby 2.3.1p112 (2016-04-26 revision 54768) [x86_64-darwin15]
```

## Install

Download the script and run its setup:

```shell
ಠ_ಠ ./listo --setup
The queue has been created at ~/.listo/queue.json
```

## Examples

```shell
ಠ_ಠ ./listo --push --content "https://www.youtube.com/watch?v=8ysFkNYwhAE"
Item #1 pushed.
```

```shell
ಠ_ಠ ./listo --push --content "https://www.smashingmagazine.com/2016/06/picking-the-best-prototyping-software-for-your-project/"
Item #2 pushed.
```

```shell
ಠ_ಠ ./listo --push --content "Hello World."
Item #3 pushed.
```

```shell
ಠ_ಠ ./listo --show --all
#3 (2016-06-29 16:22:59) Hello World.
#2 (2016-06-29 16:22:35) https://www.smashingmagazine.com/2016/06/picking-the-best-prototyping-software-for-your-project/
#1 (2016-06-29 16:20:02) https://www.youtube.com/watch?v=8ysFkNYwhAE
```

```shell
ಠ_ಠ ./listo --show
#3 (2016-06-29 16:22:59) Hello World.
```

```shell
ಠ_ಠ ./listo --show --id 1
#1 (2016-06-29 16:20:02) https://www.youtube.com/watch?v=8ysFkNYwhAE
```

```shell
ಠ_ಠ ./listo --show --size 2
#3 (2016-06-29 16:22:59) Hello World.
#2 (2016-06-29 16:22:35) https://www.smashingmagazine.com/2016/06/picking-the-best-prototyping-software-for-your-project/
```

```shell
ಠ_ಠ ./listo --show --head
#1 (2016-06-29 16:20:02) https://www.youtube.com/watch?v=8ysFkNYwhAE
```

```shell
ಠ_ಠ ./listo --show --tail
#3 (2016-06-29 16:22:59) Hello World.
```

```shell
ಠ_ಠ ./listo --show --tail --size 2
#3 (2016-06-29 16:22:59) Hello World.
#2 (2016-06-29 16:22:35) https://www.smashingmagazine.com/2016/06/picking-the-best-prototyping-software-for-your-project/
```

```shell
ಠ_ಠ ./listo --drop
Dropped the following item:
#3 (2016-06-29 16:22:59) Hello World.
```

```shell
ಠ_ಠ ./listo --drop --head --silent
ಠ_ಠ
```

```shell
ಠ_ಠ ./listo --show --all
#2 (2016-06-29 16:22:35) https://www.smashingmagazine.com/2016/06/picking-the-best-prototyping-software-for-your-project/
```

```shell
ಠ_ಠ ./listo --drop --all
Queue emptied.
```

```shell
ಠ_ಠ ./listo --show
The queue is empty.
```

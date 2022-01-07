# `good-cat`

__This cat hates pipes.__

`good-cat` is a `cat` that can't be piped. If you try, it refuses and exits with an error code. This way, no uses of `good-cat` are unnecessary [citation needed].

## Usage

For best results, set `alias cat="good-cat"` in your shell configuration file.

```sh
$ # A bad cat
$ cat /var/log/apache2/access.log | awk '{print $1}'
$ # A good cat
$ good-cat /var/log/apache2/access.log | awk '{print $1}'
$ # DOESN'T WORK!
$ # So you do this instead.
$ awk '{print $1}' /var/log/apache2/access.log
```

## Contributing

`good-cat` is maximally good and feature-complete [citation needed].

## License

`good-cat` is MIT licensed. See the `LICENSE.md` file for the license text.

## Explanation

Some people think all `cat`s should hate pipes, but the `cat`s on any
platform you find will go through pipes just fine. For people that can't stand
`cat`s in pipes, they can use `good-cat` instead.

Antipipeists will tell you that it creates a unneeded process, it stops the
piped-to process from getting random access to the contents of the file, and it
abuses the original purpose of `cat`. To those people I say: who cares?

If the random access vs. stream-of-bytes problem is measured as an actual issue,
then sure, change it. If your platform is actually having issues related to too
many processes because of excess of `cat`-into-pipe, then yeah stop doing that.
I wager that neither of these problems happen often.

But hey, if someone's really set on complaining, you can show them a `good-cat`
they'll love.

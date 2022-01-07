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

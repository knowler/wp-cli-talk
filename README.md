# Supercharge Your Workflow with WP-CLI

A talk on WP-CLI prepared for WordCamp YYC 2018.

## Resources

- [WP-CLI Website](//wp-cli.org)
- [WP-CLI Handbook](//make.wordpress.org/cli/handbook/)

## Packages demonstrated

- [`valet`](//github.com/aaemnnosttv/wp-cli-valet-command)
- [`login`](//github.com/aaemnnosttv/wp-cli-login-command)
- [`doctor`](//github.com/wp-cli/doctor-command)
- [`wp-sec`](//github.com/markri/wp-sec)

## When in doubt ask for `help`

General help:

```bash
wp --help
```

Specific help:

```bash
wp help <command>
```

## Jumping Around WordPress

### Jump to themes directory

```bash
cd `wp theme path`
```

### Jump to active theme

```bash
cd `wp theme path`/`wp option get stylesheet`
```

If you are using a theme like [Sage](//roots.io/sage), then you will need to account for the subdirectory (i.e. `sage/resources`).

```bash
cd `wp theme path`/`wp option get stylesheet | cut -d/ -f1`
```

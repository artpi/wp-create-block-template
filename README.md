# Create block template

This is a template for [@wordpress/create-block](https://github.com/WordPress/gutenberg/tree/master/packages/create-block).

## What does it modify?

It inherits from the [esnext](https://github.com/WordPress/gutenberg/tree/master/packages/create-block/lib/templates/esnext) template and adds following functionality:

- [Fixes webpack conflicts from this issue](https://github.com/WordPress/gutenberg/issues/23607#issuecomment-752010537)
- Adds `wp-env` to run a development server easily
- Automatically configures [a Github action for automatic submission of releases](https://github.com/10up/action-wordpress-plugin-deploy) to WordPress.org plugin repository
- Automatically sets up `phpcs` via `composer` to lint your PHP files.

## How do I use it?

For generating a new block, you can just

```
npx @wordpress/create-block --template @artpi/create-block-template
```

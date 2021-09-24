# js-beautify mirror

Mirror of js-beautify package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For js-beautify: see https://github.com/beautify-web/js-beautify

### Using js-beautify with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/chrissantamaria/mirrors-js-beautify
  rev: '' # Use the sha / tag you want to point at
  hooks:
    - id: js-beautify
```

By default, all files are passed to `js-beautify`, if you want to limit the
file list, adjust `types` / `files`:

```yaml
- id: js-beautify
  types: [javascript]
```

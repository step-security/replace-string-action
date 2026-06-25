[![StepSecurity Maintained Action](https://raw.githubusercontent.com/step-security/maintained-actions-assets/main/assets/maintained-action-banner.png)](https://docs.stepsecurity.io/actions/stepsecurity-maintained-actions)

# `replace-string` GitHub Action

Replaces strings with regular expressions.

## Inputs

### `pattern`

**Required** Regular expression to match.

### `string`

**Required** Input string.

### `replace-with`

**Required** String to use for replacement.

### `flags`

Flags to use when matching. Please refer to [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp) for more information.

## Outputs

### `replaced`

The replaced string.

## Example usage

```yaml
uses: step-security/replace-string-action@v2
with:
  pattern: 'Hello, (\w+)!'
  string: 'Hello, world!'
  replace-with: 'I greet you, $1!'
```

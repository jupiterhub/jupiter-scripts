# Alias for making conventional commit easier in cli

# add this into your ~/.bashrc or ~/.zshrc

# View the latest version @ https://github.com/jupiterhub/jupiter-scripts

```
gcm() {
  if [ "$#" -lt 2 ] || [ "$#" -gt 3 ]; then
    echo "Usage: gcm <conventional-type> <message> [<scope>]"
    echo "Example: gcm feat 'Your amazing work description' JIRA-123"
    return 1
  fi

  if [ "$#" -eq 3 ]; then
    git commit -m "$1($3): $2"
  else
    git commit -m "$1: $2"
  fi
}
```

# Sample usage and application:

## Without scope

`gcm "feat" "implemented new feature"`

Outputs: feat: Implement new feature

## Scoped

`gcm "feat" "Upgraded slf4j version" "commons"`

Outputs: feat(commons): Upgraded slf4j version

# Repo tag info

Extract tag information from release branch

## Outputs

### `tag`

tag name

### `tagnum`

tag number

### `majorver`

major version number

## Example usage

```yaml
- uses: nebula-actions/repo-tag-info
  id: tag

- name: Other step
  run: |
    echo ${{ steps.tag.outputs.tag }}
    echo ${{ steps.tag.outputs.tagnum }}
    echo ${{ steps.tag.outputs.majorver }}
```

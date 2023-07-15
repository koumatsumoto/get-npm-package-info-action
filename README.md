# koumatsumoto/get-npm-package-info-action

The Composite action to get npm package json information

## sample code

```yaml
- uses: koumatsumoto/get-npm-package-info-action@v1
  id: package_info

- run: |
    echo ${{ steps.package_info.outputs.package_name }}
    echo ${{ steps.package_info.outputs.package_version }}
    echo ${{ steps.package_info.outputs.git_commit_hash_short }}
```

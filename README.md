# spfx-1-15-0-beta-1

Demo project for issue at https://github.com/SharePoint/sp-dev-docs/issues/7826

## Error action

1. `yarn install`
1. `yarn gulp bundle`
1. `yarn gulp package-solution`

This will throw an error stating:

```
[10:25:03] Error - [package-solution] Error: File does not exist: <root>\sharepoint
ENOENT: no such file or directory, lstat '<root>\sharepoint'
```

## Workaround

1. Create folder structure `<root>\sharepoint\assets`
1. Re-run `yarn gulp package-solution`

This will correctly build the solution
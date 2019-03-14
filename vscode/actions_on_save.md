# Actions on save

In Visual Studio Code you can setup some **actions** running **on save** a file (or hitting ⌘ + S)

All you have to do is inserting this object to your `settings.json`:

```json
"editor.codeActionsOnSave": {
    // your actions
},
```

## Organize imports on save

To organize imports (e.g. remove unsued, aso.) on save, add the action `"source.organizeImports": true`.

```json
"editor.codeActionsOnSave": {
    "source.organizeImports": true,
},
```

## Prettier formatter on save

To format your code on save, add the action `"editor.formatOnSave": true`.

```json
"editor.codeActionsOnSave": {
    "editor.formatOnSave": true,
},
```

## Combine actions

For the sake of completeness. You can combine all **actions on save** by adding every single line of the examples from above together inside the object `editor.codeActionsOnSave`:

```json
"editor.codeActionsOnSave": {
    "source.organizeImports": true,
    "editor.formatOnSave": true,
},
```

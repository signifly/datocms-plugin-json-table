# DatoCMS plugin: JSON Table

**This DatoCMS plugin makes it possible to add/insert a key and value to output a simple JSON table. The plugin is build as a custom field editor for DatoCMS JSON fields.**

![](https://github.com/voorhoede/datocms-plugin-json-table/raw/main/docs/preview.gif)

When you input a key and value the output will be:
```json
{
  "key 1": "value 1",
  "key 2": "value 3",
  "key 3": "value 3"
}
```

## Features

* Add keys and values
* Output a simple JSON object
* Make individual entries mandatory
* Allow editor to add entries in the JSON table

For each entry in the JSON we show a key and value.

![](https://github.com/voorhoede/datocms-plugin-json-table/raw/main/docs/json-table-added.jpg)

## Configuration

First add this plugin via DatoCMS Settings > Plugins > Add (`/admin/plugins/new`).

### Plugin settings

#### Settings

There are two settings for configuration of the JSON table.

If the `Editor may add item` (Default: `true`), the button with `+ ADD ITEM` will be shown. If this button is set to `false`, the editor will not be able to add any items.

`Required/Optional fields` is a comma seperated list of keys that should be required or optional and non editable. By default every entry becomes a required key. Add a question mark (?) at the end of the key to make it optional. Example: `key1, key2?, key3`. Where `key1`, `key2` and `key3` are non editable and only `key2` is optional. When a key is added to this list it will show automatically as an entry in the JSON table.

![](https://github.com/voorhoede/datocms-plugin-json-table/raw/main/docs/json-table-required-fields.jpg)

#### Default values

To give keys a default value you can use the `Default value` tab of the JSON field. Inserting:
```json
{
  "key 1": "value 1",
  "key 2": "value 3",
  "key 3": "value 3"
}
```
will result in having the same keys and values as default.

![](https://github.com/voorhoede/datocms-plugin-json-table/raw/main/docs/json-table-default-values.jpg)

Adding the same keys to the `Required fields` will result in having default values for required fields where the editor is only allowed to edit values and not allowed to edit keys.

## Contributing

See [contributing.md](https://github.com/voorhoede/datocms-plugin-json-table/blob/main/contributing.md).

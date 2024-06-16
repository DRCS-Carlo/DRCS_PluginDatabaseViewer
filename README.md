PluginDatabaseViewer by DRCS-Carlo
================================
This simple tool is designed to scan your audio plugin pathes to create/expand an plugin overview database (for vst, vst3, clap).
The output of the tool is a SQLite database for which you can add notes/comments/links...

I recommend to use "DB Browser for SQLite" (https://sqlitebrowser.org/) for actually annotating/filtering/changing the database as it works better for these tasks.
Simply use PluginDatabaseViewer to scan your files and automatically create a database.

Currently Windows only.

How to use
-------------
![PluginViewer](https://github.com/DRCS-Carlo/DRCS_PluginDatabaseViewer/assets/169671915/cd78da6c-6263-4df5-8b3e-23fc03dd5983)

| Button/Field | Description | 
| --- | --- |
| Open DB      | Opens an existing plugindatabase (SQLite file ".db") |
| Create DB    | Creates a new, empty database with the fields "id", "name", "company", "type", "subtype", "path", "plugintype", "notes", "Source" and "link". |
| Scan Path    | <p>Scans a path for plugins. All files with the file endings ".dll", ".vst3" and ".clap" are added to the database. For simplicity it is assumed that ".dll" are vst files.  <br> If a file and its path is already in the database, it will not be added twice. <br> Newly found plugins are added and the fields "id", "name",  "path", and "plugintype" are filled out automatically. </p> |
| Dropdown     | Select the database within an SQLite file.|
| insert row   | Add a new row entry. |
| delete row   | Deletes the currently selected row entry. |
| find         | Find instances of the database matching the given string. |
| filter       | Filters the database based on the string provided in the "find" field. To unfilter, delete the string in the "find" field and click "filter" again. |

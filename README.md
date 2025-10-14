# Nouds Personal Scripts

These are some of my personal scripts which i use while developing on linux

## hexprint

Print any value to a hexadecimal value

## workspace

Open a workspace in vscode.

A csv file /home/USER/.workspace.csv needs to be present. This csv file should be in the following format:

```csv

<workspacename>,<workspacepath>

```

Where *workspacename* is the name of the workspace, and *workspacepath* is the path to open

### Example

the following CSV file:

```csv
bar,"/home/joe/my_projects/bar-project"
foo,"/home/joe/my_projects/foo-project"
secret-foo,"/home/joe/.my_secrest_projects/foo-project"
```

with the command:

```bash
workspace foo
```

will result in the following command being executed by the script

```bash
code /home/joe/my_projects/foo-project
```
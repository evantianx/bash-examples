## Bash

### Basics

- `cd`

  `cd -` go back to last directory

- `ls`

  - `ls -a` list everything include hidden files
  - `ls -aF` and label the folders or execution files

- `cp`

  - `cp x y` copy a file x and rename it as y
  - `cp x y z folder_path` copy file x, y, z into a folder
  - `cp -i x folder_path` copy file and ask overwrite or not if it's exist
  - `cp -r folder1_path folder2_path` copy a folder into another folder (`r` means recursive)
  - `cp -v ...` give us a verbose info

- `cat`

  - `cat n x` show content of x with line number
  - `cat x y z` show content of x y z one by one
  
- `more x` / `less x`

  `more x` to show content of x and start from beginning;
  `less x` to show content of x in an screen and quit without anything leave

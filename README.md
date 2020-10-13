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

- `touch`

  can modify the last edited time of one exist file
  
  - `touch -c blabla` just touch one file only it exists
  
- `mkdir`

  - `mkdir -p new_parent_folder/new_child_folder` create both `new_parent_folder` and `new_child_folder`
  
- wild card

  - `*` means any charactors
  - `?` means any single charactor
  - `[abc]` means a or b or c
  - `[!abc]` means any charactor that is not a, b or c
  - `[[:alpha:]]` means only (one) letter; `[[:digit:]]` means only (one) number; `[[:lower:]]` means only (one) lowercase letter; `[[:upper:]]` means only (one) uppercase letter;
  
- variables

  how to set / unset variables in shell?
  
  ```bash
  # mind that there is no spaces!
  name=evan
  
  # unset
  unset name
  ```
  
  how to get value of variables?
  
  ```bash
  ${name}
  ```
  how to get variables length?
  
  ```bash
  ${#name}
  ```
  
  how to get part of variables?
  
  ```bash
  # from the second one to the end
  ${name:2} 
  
  # from the second one, and the length is 1
  ${name:2:1}
  
  # froom the last third one to the end
  # mind the space
  ${name: -3}
  
  # froom the last third one, and the length is 2
  # mind the space
  ${name: -3:2}
  ```

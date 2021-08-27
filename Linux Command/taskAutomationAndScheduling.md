## Automation using Bash Script

- Instead normally writing many command repeatedly you can write those command into a text file knows as `Bashscript` then just run the script.

- When you run the script all command in this file will be execute one after the other from top to bottom.

- You can schedule run bashscript by using schedule program called `Cron`

## Creating Bashscript

- make a text file with the tail `.sh`

- The most important thing is tell the file is a special file , not normal file. It need to read by using a certain `interpreter`.

```
#!/bin/bash 
//1st line is Shabangu and path to BASH interpreter to tell this is't a normal text file. It's must bt stay on the 1st line and don't have any space in this line

```

**Example**:

```
To print Hello world to command

#!/bin/bash

echo "Hello world!"
```

- To run `bash script` go to terminal and type : bash + your_file_name

```
#!/bin/bash

mkdir /home/long/magic
cd /home/long/magic
touch file{1...100}
ls -lh /home/long/magic > /home/long/magic.log

```

- `schedule` command and bash scripts to run using `cron`. It help `Automate your workflow` by scheduling your script tp run whenever you want!

- `Cron` is a commandln e based program that is used to schedule task

- `crontab -e` to show crontab and you can modify it to schedule

- First 5 columns in `cron` file are scheduling information adn final sixth column is the command or script.

```
// print hello world and save to hello.txt every minute, every hour, every day, month
#  m   h  dom  mon dow   command
  *   *   *   *   *     echo "hello world" >> /home/long/hello.txt
```

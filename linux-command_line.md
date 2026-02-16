# Basic Linux Command Line Tutorial

Before we get started on Git and Github, let's first get farmiliar with the _Linux Command Line_. While modern graphical interfaces (GUIs) are great, the Linux command line (often called the **Terminal** or **Shell**) is where the real power lies. It allows you to talk directly to your computer using text commands.

Here is a beginner’s guide to navigating and controlling your system. 

---

### 1. Understanding the Interface

When you open your terminal, you will see a **Command Prompt**. It usually looks something like this:

`user@computername:~$`

* **`user`**: Your username.
* **`computername`**: The name of your machine.
* **`~`**: This symbol (tilde) represents your **Home Directory** (your personal folder).
* **`$`**: This is where you type.

### 2. Navigation: Finding Your Way Around

In Linux, folders are called **directories**. You are always "inside" one directory at a time.

* **`pwd` (Print Working Directory):**
    Asks the computer: *"Where am I right now?"*
    ```bash
    pwd
    # Output example: /home/username
    ```

* **`ls` (List):**
    Asks the computer: *"What files are in this folder?"*
    ```bash
    ls
    # Output: Documents Downloads Music Pictures
    ```

* **`cd` (Change Directory):**
    Used to move between folders.
    * To go into a folder: `cd Downloads`
    * To go back one level (up): `cd ..`
    * To go back home: `cd ~`

### 3. Creating and Managing Files

Once you are in the right place, you can start organizing.

* **`mkdir` (Make Directory):**
    Creates a new folder.
    ```bash
    mkdir MyProject
    ```

* **`touch`:**
    Creates an empty file (useful for starting scripts or notes).
    ```bash
    touch notes.txt
    ```

* **`cp` (Copy):**
    Copies a file from one place to another.
    * *Structure:* `cp [original_file] [new_copy]`
    ```bash
    cp notes.txt notes_backup.txt
    ```

* **`mv` (Move):**
    Moves a file. This is also how you **rename** files in Linux.
    * *To move:* `mv notes.txt Documents/`
    * *To rename:* `mv notes.txt meeting_notes.txt`

* **`rm` (Remove):**
    Deletes a file.
    > **⚠️ Warning:** There is usually **no Trash Bin** in the command line. When you `rm` a file, it is gone forever.
    ```bash
    rm old_file.txt
    ```

### 4. Viewing File Content

You don't always need to open a text editor to see what's inside a file.

* **`cat` (Concatenate):**
    Dumps the entire content of a file onto your screen. Good for short files.
    ```bash
    cat meeting_notes.txt
    ```

* **`less`:**
    Lets you scroll through a long file one page at a time.
    * Press `q` to quit and return to the prompt.
    ```bash
    less long_log_file.txt
    ```

### 5. Two "Superpowers" for Beginners

These two tricks will make you look (and feel) like a pro immediately:

1.  **Tab Completion:**
    Start typing a filename or directory (e.g., `cd Doc`) and hit the **Tab** key. The system will automatically finish the word for you (`cd Documents/`). This saves time and prevents spelling errors.
2.  **History:**
    Press the **Up Arrow** key on your keyboard. This cycles through commands you previously typed. You don't have to type the same long command twice!

---

### Quick Reference Table

| Command | Action | Meaning |
| :--- | :--- | :--- |
| `pwd` | Check location | "Where am I?" |
| `ls` | List files | "What is here?" |
| `cd` | Change folder | "Go there." |
| `mkdir` | Create folder | "Make directory." |
| `clear` | Clear screen | "Clean up the mess." |
| `man [command]` | Manual | "Help me with [command]." |

## 1 · Where am I?
1. The pwd command prints the absolute path of your current working directory "/Users/avadhiii"
2. "ls -a "list all the files including the hidden ones too and ls showed all the users profile folders 
3. "drwx------@  6 avadhiii  staff    192 27 Aug 15:53 Desktop"
For my hello file, -rwxr-xr-x@ means: it's a regular file, I can read/write/execute it, others can only read/execute, and the @ shows it has extra metadata.

## 2 . Build the Folder
4. `coding-cafe/week02` works because I'm standing in my home folder, and it just walks down from there — that makes it a **relative path**, not absolute (absolute would start with `/`, like `/Users/avadhiii/coding-cafe/week02`).

## 3 · Move, copy, rename, delete
5. `mv` moved my file into `week01/` (relocating it), then renamed it to `old-readme.md` (same folder, new name). So `mv` does both moving and renaming, depending on what I give it.

## 4 · Where does the shell find things?
6. Counting by `:`, my `PATH` has 17 folders on it.
7. My `python3` lives at `/opt/anaconda3/bin/python3` — confirmed by `which python3`.
8. Comparing with the person next to me, our paths were different — mine goes through `/opt/anaconda3/bin` since I'm using Anaconda, so if they installed Python a different way, theirs is probably pointing somewhere like `/usr/local/bin` instead.
9. The shell said `zsh: command not found: pyton3`. That means it searched every one of the 17 folders in `PATH`, in order, and none of them had a file named `pyton3` — so it gave up and threw the error.

## 5 · A box of your own
10. `.venv` didn't show up with plain `ls` because it starts with a dot, which makes it a hidden file — I only saw it once I ran `ls -a`, which shows hidden files too.
11. My prompt changed — it now starts with (.venv) right before (base) avadhiii@..., showing I'm inside the virtual environment.
12. It's different — `which python3` now points to `/Users/avadhiii/Desktop/PLAKSHA/Coding-cafe/labs/.venv/bin/python3`, not my anaconda3 path from before. That tells me `activate` didn't change what Python is installed anywhere — it just edited my `PATH` so this folder's own `.venv/bin` gets checked first.
13. The second list had `requests`, plus the packages it needed along with it — `certifi`, `charset-normalizer`, `idna`, and `urllib3` — none of which were there in the first `pip list`, which only had `pip` itself.
14. After `deactivate`, `which python3` points back to `/opt/anaconda3/bin/python3` — my regular anaconda Python, not the `.venv` one anymore.

## 6 · Read a manual
15. `ls -h` makes file sizes human-readable — instead of showing raw byte counts, it shows them in KB, MB, GB, etc. I'd usually pair it with `-l`, like `ls -lh`, to actually see it in action.

## 7 · Work faster
16. `Ctrl + C` interrupted whatever was running at that moment inside the `>>>` prompt (like it would stop a script that's stuck in a loop), but it kept me inside the Python REPL. `Ctrl + D`, on the other hand, actually closed the REPL and dropped me back to my normal shell prompt — a cleaner exit than `Ctrl + C`.





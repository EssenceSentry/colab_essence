# colab_essence
Google Colaboratory utilities.

### Google Drive utilities

- `mount_drive()`

Mount Google Drive to Colab.

- `to_drive(file_location, path="")`

Move file from the local Colaboratory hard disk to your Google Drive storage.

### Github utilities

- `github_id()`

Identify yourself to GitHub.

- `clone_repo(repo_name, secret=False, user=None)`

Clone a public or private GitHub repository.

### Download utilities

- `download(url, load_cookies=False, save_cookies=False)`

Download a file from a URL. Save or load cookies for more involved downloads.

- `big_drive_file(link)`

Download Google Drive files (publicly shared with a link) that cannot be downloaded directly without confirmation because of their size (Google does not perform antivirus analysis on them).

### Function utilities

- `curry(func)`

Create a curried version of a function that returns as soon as all the required arguments are passed.

- `F(expr)`

Given an expression as a string, it returns a curried function that when  passed the needed arguments in alphabetical order, returns the result of the expression. Any variable used in the expression is a local argument of the function, unless the variable is in the global scope.

### Run Visual Studio Code

- `run_vscode()`

Prepare the environment and run Visual Studio Code.

### Other utilities

- `env_vars("GITHUB_NAME", "GITHUB_PASSWORD", set_environ=False, env_file_location=f"{DRIVE_PATH}.env")`

Return the value of the requested enviroment variables from a given .env file. If set_environ is True (False by default), load to `os.environ` and is available with `os.environ[var_name]` from anywhere in the current environment.

- `hash_file(file_location, hash_fns={"MD5": hl.md5, "SHA1": hl.sha1}, buffer_size=4*GB)`

- `uncompress(file_location)`

Extract compressed files (.zip, .tar, .tar.gz, .tar.bz2, .tar.lz, .tar.lzma, .tar.xz).


## Things to do:

- [ ] Visualization recommender system.
- [ ] See what other self-hosted services can be added.
- [ ] Improve download (local file system, Google Sheet, SQL, BigQuery)
- [ ] Add numpy, Sympy, LaTeX alternatives to F
- [ ] What about transformational programming like Bird-Meertens
- [ ] Ask or generate password if not present in .env file
- [ ] Input widgets for all functions
- [ ] Boilerplate for TPUs
- [ ] Keras + FastAI
- [ ] Original Jupyter through SSH
- [ ] Wrapping for mobile devices with text transformation and extra imput row.
- [ ] Try improving the autocompletion using Tabnine or Kite
- [ ] Add auto formatting, refactoring, debugging, profiling utilities
- [ ] Add property based testing with Hypothesis

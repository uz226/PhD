# PhD

This repository can act as a lightweight project wrapper now, and be connected to an existing folder later.

## Link to a preexisting folder later

When you are ready, create a symlink in this repository that points to your existing folder:

```bash
ln -s /absolute/path/to/existing-folder ./linked-folder
```

Then commit the symlink:

```bash
git add linked-folder
git commit -m "Link project to preexisting folder"
```

This keeps your existing folder in place while allowing this repository to reference it.

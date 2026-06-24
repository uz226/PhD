# PhD

This repository can act as a lightweight project wrapper now, and be connected to an existing folder later.

## Link to a pre-existing folder later

When you are ready, create a symlink in this repository that points to your existing folder:

```bash
ln -s /absolute/path/to/existing-folder ./linked-folder
```

Then commit the symlink:

```bash
git add linked-folder
git commit -m "Link project to pre-existing folder"
```

This keeps your existing folder in place while allowing this repository to reference it.

> Note: Git tracks the symlink itself, not the target folder contents. Symlink behavior can vary across platforms (especially on Windows), so confirm your team environment supports it before relying on this workflow.

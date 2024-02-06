Visit **[johannessonlab.org](https://johannessonlab.org)** 🚀

# Johannesson Lab

This repository hosts the source code and data for the [Johannesson lab web page](https://johannessonlab.github.io/). It was created from the [Lab website template](https://github.com/greenelab/lab-website-template/).

## Update the site

_Internal user guide for the johannessonlab administrator_

### Adding lab members
**Add new members** in the `_members` directory as new `.md` files. Simplest way is to copy a present member, change file name, and edit metadata. Add a photo in the `images` directory.

### Removing lab members
**Removing active lab members** is done by changing the group from `group: current` to `group: alum` in the member data.

### Adding publications
Add new publications by making new entries in `data/sources.yaml`. Only the DOI number is necessary, but an image can also be added. **Important**: after adding the DOI number in `sources.yaml`, auto-cite.py needs to be run. You will have to install some dependencies first. See [the lab website template documentations for details](https://greene-lab.gitbook.io/lab-website-template-docs/basics/citations).

Installing dependencies:
```bash
pip install importlib
pip install dict_hash
pip install --upgrade manubot
```
manubot defaults to install in `$HOME/.local/bin/`. You may have to add it to PATH:
```bash
export "PATH=$HOME/.local/bin/:$PATH" >> $HOME/.bashrc
```

### Make a news post
Make news posts by adding files in `_posts`. The files need to be named according to jekyll blog post format, i.e. with the date first. Easiest is to copy a previous post and edit the information.

After all changes are done in the source code, commit and push changes as per usual. Pushed changes are automatically updated by github-pages.

### Tags
Tags in news posts, research projects, publications, etc need to be indented by two spaces in the yaml front matter. Each tag on a new line, else spaces aren't included in the tag.

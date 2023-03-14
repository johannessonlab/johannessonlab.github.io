# Johannesson-lab

This repository hosts the source code and data for the [Johannesson lab web page](https://johannessonlab.github.io/). It was created from the [Lab website template](https://github.com/greenelab/lab-website-template/)

## Update the site

_Internal user guide for the johannesson-lab administrator_

### Adding/removing lab members
**Add new members** in the `_members` directory. Simplest way is to copy a present member and edit metadata. Add a photo in the `images` directory.
**Removing active lab members** is simply done by changing the group from `group: current` to `group: alum` in the member data.

### Adding publications
Add new publications by making new entries in `data/sources.yaml`. Only the DOI number is necessary, but an image can also be added. **Important**: after adding the DOI number in `sources.yaml`, auto-cite.py needs to be run. You will have to install some dependencies first. See [the lab website template documentations for details](https://greene-lab.gitbook.io/lab-website-template-docs/basics/citations).

### Make a news post
Make news posts by adding files in `_posts`. The files need to be named according to jekyll blog post format, i.e. with the date first. Easiest is to copy a previous post and edit the information.

After all changes are done in the source code, commit and push changes as per usual. Pushed changes are automatically updated by github-pages.
---
layout: post
section-type: post
category: etc
---

I made a script for simplifying creating new posts for this website.

From the project root directory:

`./scripts/new-post <title>`

This will a create a new file named `YYYY-MM-DD-<title>.md` in the `_posts` directory.
It sets some default values in the front matter block. 
It then opens the file in the editor specified by the environment variable, `$EDITOR`.

Specify a category in the front matter block.
Optionally, specify a title if you don't want the default extracted from filename.
Write the post contents below using Markdown. 
Save.
Test locally.
Commit.
Push.
GitHub will automatically build and deploy changes to live site.



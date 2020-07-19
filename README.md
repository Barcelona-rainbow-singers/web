# Barcelona rainbow singers

This repo contains the code and the content to generate the public website of Barcelona rainbow singers: https://barcelonarainbowsinglers.org

## How it works

### Content

Content is managed in plain files on this repo `/content` folder:

- `/content/page` where content pages are edited using markdown and then published over `/page-filename` at the public web and included at the page menu.
- `/content/show` is where our shows should be placed and will be published over `/show/show-filename` at the public web and will be listed at the menu and home page.

### Templates

### Build and deploy

Once you've finished adding/modifying content or templates you need to rebuild the web by running:

```
$ ./builder/builder.pl
```

It will create all needed files on the `docs/` folder so you are ready to deploy by commiting it to this repo:

```
$ git add .
$ cit ci -m 'Description of your changes'
$ git push
```

Once done, your changes should go live shortly.


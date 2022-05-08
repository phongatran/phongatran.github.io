# Irene Chen Research Website

## Source

Based on [demo website](http://ankitsultana.com/researcher).

## Deployment

Currently website is hosted on [Irene's CSAIL site](http://people.csail.mit.edu/iychen/). 

Once the site has been perfected, build the site
```jekyll build```

Then, copy the contents of `./_site` into the CSAIL folder according to

```scp /Users/irenechen/Documents/research-site/_site/* iychen@login.csail.mit.edu:/afs/csail.mit.edu/u/i/iychen/public_html/.```

## Customization

* You can edit the `.md` (markdown) files as you see fit. You can also add some other markdown file, say `foo.md` in the root directory of the repository. It will then be accessible like so `{{ url of your website }}/foo`.

* You can of course remove `contact.md` if you don't want it

* To set the heading, edit the `title` variable in `_config.yml`

* To edit the `links` mentioned on the navigation bar, edit the file `_data/nav.yml`

* You can change the accent (color of hyperlinks) by editing the `accent` variable in `_sass/vars.scss`

* You can setup google analytics, by setting `tracking_id` in `_config.yml`

* To add a profile picture, make sure to give the image tag the class `profile-picture`. In other words,do it like so:

```html
<img class="profile-picture" src="sherlock.jpg">
```

**Note:** Customizing the accent color might cause merge conflicts if you later try to merge from `bk2dcradle/researcher` to fetch updates/patches etc. (applicable only if you have forked).

### License

[GNU GPL v3](https://github.com/bk2dcradle/researcher/blob/gh-pages/LICENSE)



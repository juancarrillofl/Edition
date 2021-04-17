# Edition

A bootstrapped theme from the newsletter theme for [Ghost](https://github.com/TryGhost/Edition). This version was modified for my personal needs, but it could help you too because of some problems that I encountered (maybe I should do a Pull Request with some fixes later on the original repo, who knows).

## Major Changes

* Add major social media icons as partials for personal use, based on SVG Graphics that I encountered on the Web (this list can change overtime). These partials are:

    * GitHub
    * GitLab
    * Instagram
    * Linkedin
    * YouTube
    * Twitch
    * Pinterest
    * TikTok
    * Dribbble
    * Codepen

* Force expanded content view for the home page and tagged content. Ignores giving the user the option to switch.

* Change secondary text color to a darker tone *(#666)* for better accessibility. This text is used in sections like the secondary navigation bar on the footer. **(Important)**.

* Add an aria-label to cover-arrow item for better accessibility.

* Increment menu-item and copyright font size and font weight for better accessibility/SEO.

* Add my name on the footer instead of Ghost for better branding **(if you are going to use this bootstrapped theme, remember to change this too!)**

* Hard code my GitHub and Linkedin using partials mentioned above to show on the header and footer of my website. If you know of a better way to do this, please let me know! **(Also, if you are going to use this bootstrapped theme, remember to change this too, again!)**

* Change login button to subscribe button by default.

* Feature image on tags (or categories, however you called them) is now an horizontal image by default like in the [Dawn Theme](https://github.com/TryGhost/Dawn)

* Suggest other tags on the top of tag pages, like in the Dawn Theme.

* Classify post more simply, without using "tag" on the `routes.yaml` file. To have a cleaner url. **(REMEMBER: you have to upload the routes.yaml manually on your instance or modify it directly on that same instance. This file does not change when you make an update on your repository!)**

Everything else stays the same on the theme and other major changes on my website are made directly on Ghost CMS.

## Development

Edition styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
yarn zip
```

## PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.

## Copyright & License

Copyright (c) 2013-2021 Ghost Foundation - Released under the [MIT license](LICENSE).

# W3RL Web Page

## TODOs (desc. relevance)
 - Add missing content
 - Fix layout
 - Replace favicon
 - Change baseurl
 - Configure domain

## Tech stack
The page is built with [Hugo](https://github.com/gohugoio/hugo), a Go based fast and modern static site generator. Currently the [Elate template](https://github.com/saey55/hugo-elate-theme/) is being used to style the aestethics and content of the website. The deployment to S3 is based on the [hugo-s3-action](https://github.com/plopcas/hugo-s3-action).

## Authoring

### Local Hugo Setup
To preview larger changes please install [Hugo](https://gohugo.io/installation/) and a Git client like [Sourcetree](https://www.sourcetreeapp.com/) or [Github Desktop](https://desktop.github.com/) if you're new to Git(hub). After pulling the WWW3RL repository, you can then start `hugo server` in a terminal to [develop and test the site](https://gohugo.io/getting-started/usage/#develop-and-test-your-site). A local version should be available at `localhost:1313`.

### Pictures
For now all pictures need to be placed in the [static/images folder](./static/images) to be accessible when adding content.

### Text
All text content is simply added to the [config.toml](./config.toml) in the root of the project. To add an item simply copy an existing item and change it to fit your needs.

### TUM Style
To fit in with the visuals used by TUM we created a [TUM.css](./themes/hugo-elate-theme/static/css/tum.css) that holds the design. Please use the predefined colors:

 - TUMlochmara
 - TUMroyalblue
 - TUMnightrider
 - TUMwhite

## Deployment
The main branch is automatically made available online via Github Actions and AWS. To make larger changes [please create a new branch in this Github repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) and [review your changes before merging them](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

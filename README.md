# Center for PT website

This website is built using the [jekyll][jekyll] static generator and deployed to [Github Pages](https://pages.github.com/).

## Running Locally

You can [follow jekyll's quick start docs](https://jekyllrb.com/docs/) to get running locally.

## Directory Structure

## `layouts`

Layouts are the markup around your pages content.
When authoring a page, you can declare which layout it uses via the page's [front matter](https://jekyllrb.com/docs/front-matter/).

### `assets`

Home to static assets used by layouts and pages (e.g images, css, js).
These are typically referenced in templates via `{{ '/assets/path/to/asset' | relative_url }}`.

### `_data`

This is the [jekyll data files](https://jekyllrb.com/docs/datafiles/) directory.

It houses data files that are used on pages, but don't have pages of their own.
The idea here is that it should be straight-forward to update these data files without mucking around too much with the templates that use them.

### `_staff_members`

Similar to `_data`, this directory houses files with accompanying data.
However, unlike the data in `_data`, each of the entries also gets its own page.
This directory is an example of a [jekyll collection](https://jekyllrb.com/docs/collections/).

The content here is lifted from the existing website, which I expect to change.

## Deployment

Deployment to Github Pages happens on pushes to main via the [jekyll-github-pages][deployment-workflow] workflow.

Deployed changes should appear at https://center-for-pt.github.io.

## Current Status / Future Enhancement

### Known Development Shortcomings

* Style the other pages (stopped at homepage)
* Use real images / optimize images for web
* Should this go live, we'd need to [point the production domain to this site][dns-docs] and update the github pages settings.

### Known Content Shortcomings

* Review data files content
* Review staff member content

## Helpful Links

* [jekyll docs][jekyll]
* [github pages docs][github-pages]
* [webpage insights][webpage-insights] - good resource for improvements to make prior to launch.

[jekyll]: https://jekyllrb.com/
[github-pages]: https://pages.github.com/
[webpage-insights]: https://pagespeed.web.dev/
[dns-docs]: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
[deployment-workflow]: https://github.com/center-for-pt/center-for-pt.github.io/blob/main/.github/workflows/jekyll-gh-pages.yml](https://jekyllrb.com/docs/)https://jekyllrb.com/docs/https://jekyllrb.com/docs/

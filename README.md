# Hexo + netlify CMS

> ⚠️ **Deprecation Notice** 🏳
>
> We are focusing our resources on building new templates that help you build a better web, because of that we're deprecating this template. We care about the community so we propose if anyone wants to maintain or take stewardship over the project please contact us at [devexperience@netlify.com](mailto:devexperience@netlify.com). If you want to share anything with the team about this template, you can also fill out [this form](https://template-feedback.netlify.app/).

This is a simple example of how to integrate netlify CMS with a hexo based site.

It's based on Brian Rinaldi's great [Static Site Samples](https://github.com/remotesynth/Static-Site-Samples) and meant as a simple example of how to hook netlify CMS up with a hexo based site.

## Setting up

Make sure to install the [netlify-git-api](https://github.com/netlify/netlify-git-api) before you start.

Then:

```bash
git clone https://github.com/netlify-templates/hexo-cms-example.git
cd hexo-cms-example
netlify-git-api users add
netlify-git-api serve
```

Open a separate terminal window and run:

```bash
npm install
hexo server
```

## Using

Visit [localhost:4000](http://localhost:4000/) to browser the site.

Visit [localhost:4000/admin](http://localhost:4000/admin) to use the CMS.

To run against the GitHub API in production, edit the production backend settings for `admin/index.ejs` with the correct repository and branch.

Then run:

```bash
CMS_ENV=production hexo server
```

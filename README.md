[![build status](https://gitlab.com/librehealth/librehealth.io/badges/master/build.svg)](https://gitlab.com/librehealth/librehealth.io/commits/master)

---

This repo contains the LibreHealth website [librehealth.io](https://librehealth.io), built using [Hugo](https://gohugo.io/overview/introduction/). The website is a set of markdown files that are styled into HTML. To contribute to the website, you only need a text editor and some good content.
Hugo a general-purpose static site generator written in the Go programming language. The site is compiled by the GitLab CI on every commit and then posted to librehealth.io

---
**Table of Contents**
- [Contributing changes](#contributing-changes)
- [Building locally](#building-locally)
- [Troubleshooting](#troubleshooting)

## Contributing changes
 1. Create an issue describing the change you are making to the website
 2. Fork this repo in GitLab and make changes in your fork by referring to the issue
 3. Submit a merge request with the change and title it with the issue number
 4. The maintainer of this repo will merge the change and then it will be built and deployed

## Building locally
Ideally, you should just edit and commit the pages on GitLab, so that it can build and deploy the updated site. But if you want to build and test locally, you can do the following:
 1. Fork, clone or download this project
 2. [Install](https://gohugo.io/overview/installing/) Hugo
 3. Preview your project: `hugo server` , then point your browser to [localhost:1313/librehealth.io/](https://localhost:1313/librehealth.io/)
 4. Add content
 5. Generate the website: `hugo` (optional)

Read more at Hugo's [documentation](https://gohugo.io/overview/quickstart/).

## Using the hugo-universal-theme
We are using the hugo-universal-theme for the website.

## Troubleshooting

1. CSS is missing! That means two things:

    Either that you have wrongly set up the CSS URL in your templates, or
    your static generator has a configuration option that needs to be explicitly
    set in order to serve static assets under a relative URL.

# tomesh.net

Website for [Toronto Mesh](https://www.tomesh.net/) ([https://www.tomesh.net/](https://www.tomesh.net/)), built with [Jekyll](https://jekyllrb.com/), [Font Awesome](http://fontawesome.io/) icons, and [Skeleton](http://getskeleton.com/) CSS.

Copyright (C) 2016 Toronto Mesh contributors.

All tomesh.net **code** at <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/tomeshnet/tomesh.net/" property="cc:attributionName" rel="cc:attributionURL">github.com/tomeshnet/tomesh.net</a> is licensed under a <a rel="license" href="https://www.gnu.org/licenses/gpl.html">GNU General Public License v3.0</a>, the text of which is included in the repository [here](https://github.com/tomeshnet/tomesh.net/blob/master/LICENSE.md).

<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Tomesh.net website</span> **content and documentation** is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

## Getting Involved
We are still in the early stages and would love involvement from more people!
If you notice any errors or would like to submit changes or add content to our website please see our [Contributing Guidelines](https://github.com/tomeshnet/documents/blob/master/CONTRIBUTING.md).

In addition, you can provide feedback by:
* adding a comment to the [issue tracker](https://github.com/tomeshnet/tomesh.net/issues).
* emailing us at [hello@tomesh.net](mailto:hello@tomesh.net)
* speaking with us on the `#tomesh` channel in [CivicTechTO](http://civictech.ca/)'s slack ([get an invite](https://civictechto-slack-invite.herokuapp.com/))

## Development

### 1. Install Dependencies

Install the Jekyll gem:

```bash
$ gem install jekyll
```
**Windows users:** [Run Jekyll on Windows](http://jekyll-windows.juthilo.com/)

### 2. Running Locally

```bash
$ jekyll serve
```

A development server will run at `http://localhost:4000/`

## Deployment

Commits and merges into `master` will be deployed automatically to the production web server through webhook posts from GitHub.

[jekyll-hook](https://github.com/developmentseed/jekyll-hook) listens for incoming webhook posts from GitHub and runs `jekyll build`.

### Daily Builds

A cron task runs `jekyll build` daily at midnight, Eastern Standard Time. The build task can be found in the [scripts directory](scripts/tomesh-build.sh). The cron task can be edited with `sudo crontab -e`

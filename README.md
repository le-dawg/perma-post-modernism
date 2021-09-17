# ✨ App Nextjs Theme ✨

This is an "App" theme landing page built with [Next.js](https://nextjs.org/) and
powered by content stored in files.

The theme can be used to create a static website that is hosted by a serverless
deployment platform such as [Netlify](https://www.netlify.com). The contents of
the website are stored in git with the rest of the site's code.

When deploying the website, [Sourcebit](https://github.com/stackbithq/sourcebit)
reads the site's contents from files and provides it to Next.js. Once Next.js
finishes generating the static website, [Netlify](https://www.netlify.com) pushes
the static files to its CDN.

[Sourcebit](https://github.com/stackbithq/sourcebit) and its plugins, specifically
[`sourcebit-source-filesystem`](https://github.com/stackbithq/sourcebit-source-filesystem)
and [`sourcebit-target-next`](https://github.com/stackbithq/sourcebit-target-next),
are used to read the site's contents from files, normalize it, and provide it to
Next.js pages. It also sets up live updates in development mode allowing you to
update the content files and instantly see your updates in the browser.


## Quick Start 🏎


## Develop Locally

1. [Create a site](https://app.stackbit.com/create?theme=https://github.com/stackbit-themes/app-nextjs&utm_source=theme-readme&utm_medium=referral&utm_campaign=stackbit_themes) from this theme using Stackbit.

1. Once finished, you will be redirected to Stackbit Studio where you will be
   able to edit the content using the free on-page editing experience, and
   publish new versions of your site.

1. To further develop your site, clone the generated repository.

1. Install dependencies

       run npm install

1. Start the Next.js local development server:

        npm run develop

1. Open [http://localhost:3000/](http://localhost:3000/) in the browser to see
   your site. You can now edit the site contents, and the browser will
   live-update your changes. 🎉


## Building for production 🏗

To build a static site for production, or test locally how it worls, run the
following command:

    npm run build

The exported site will be written to `out` folder. The contents of this folder
can be deployed by serverless deployment platform such as [Netlify](https://www.netlify.com).
You can start a local server serving the static files from the `out` folder, for
example by installing and running `http-server`:

    npm install http-server -g
    http-server out

## Install

* <code>git clone</code> into a directory
* <code>git checkout gh-pages</code>
* <code>bundle install --path vendor</code>

## Development Server

Run locally using Jekyll & Foreman:

<code>$ ./devserver</code>

## Push to production 

This project consists of two branches, <code>gh-pages</code> and <code>master</code>.  The <code>gh-pages</code> branch is where all the design and dev files are that serve the website on Github pages. 

The <code>master</code> branch is a nodejs webserver with a github webhook attached so that when the <code>gh-pages</code> branch is updated on Github it checks out the codebase, builds it and publishes it in a static folder served by Express for node.

To publish changes to the design files, checkout and use the <code>gh-pages</code> branch.

<code>$ git push origin gh-pages</code>
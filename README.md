### After cloning

Install the theme as a git submodule

``` sh
git submodule update --init --recursive
git submodule update --recursive --remote
```
### Deployment

Deployed via netlify.com (just push to master and netlify will automatically build the project)

For local development:

    docker run --rm -it -v $(pwd):/src -p 1313:1313 klakegg/hugo:0.48 server -D

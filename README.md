commitify
============

browserify transform for appending the latest git commit SHA

Usage
-----
Simply add 'commitify' to your browserify transforms in your package.json
```js
{
    "browserify": {
        "transform": [
            "commitify"
        ]
    }
}
```

In your browser console, you will have two global variables which contain the build time and the latest git commit:
```js
__BROWSERIFY_META_DATA__CREATED_AT
// "Sun Feb 15 2015 17:18:10 GMT-0500 (PET)"

__BROWSERIFY_META_DATA__GIT_VERSION
// 75bf4ee
```

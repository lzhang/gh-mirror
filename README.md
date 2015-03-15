gh-mirror is a simple way to mirror an org's GitHub repositories locally,
maintaining the upstream repository metadata, and keep them updated easily. See
[the blog post I wrote it for][blog] to get more information about how to use
it in a useful way. For private repositories, ensure that the user running
gh-mirror has a sufficient .netrc file for github api and repository access.

```
$ gh-mirror exampleorg
Cloning into bare repository 'foo.git'...
remote: Counting objects: 7, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 7 (delta 0), reused 6 (delta 0)
Receiving objects: 100% (7/7), done.
Checking connectivity... done.
Cloning into bare repository 'bar.git'...
[...]
```

[blog]: https://chrisdown.name/2013/07/05/setting-up-local-github-mirror-with-cgit-git-daemon.html

## Testing

[![Build status][travis-image]][travis-builds]

    $ pip install nose
    $ nosetests

[travis-builds]: https://travis-ci.org/lzhang/gh-mirror
[travis-image]: https://travis-ci.org/lzhang/gh-mirror.png?branch=master

## License

gh-mirror is [ISC licensed][isc]. See the LICENSE file for full details.

[isc]: http://en.wikipedia.org/wiki/ISC_license

# Good First Bug Template for SpiderMonkey

The following is a template for opening a new bug, aimed at attracting and oboarding new contributors.

It has a few properties that I think are imporant to onboarding new contributors:

1. It clearly lays out the pre-requisites: The absolute bare minimum amount of knowledge a new contributor would need to be successful at solving a bug.
2. It clearly lays out a set of success criteria: these are the things the contributor is trying to accomplish in a checklist form.
3. It points out where the new contributor can get help.
4. It has pointers to techniques and tools that new contributors would find useful in tackling their first bug.

```
<Bug Description>

## Prerequisites
 
Before getting started, you'll want to

* Have a checkout of the Firefox source code
* Make sure you can build [SpiderMonkey](https://firefox-source-docs.mozilla.org/js/build.html)
* Understand [the basics of using Mercurial](https://mozilla-version-control-tools.readthedocs.io/en/latest/hgmozilla/firefoxworkflow.html)
* Understand [how to submit a patch](https://docs.firefox-dev.tools/contributing/making-prs.html)
* Read [this walkthrough](https://moz-conduit.readthedocs.io/en/latest/walkthrough.html) about how development works in Firefox.


## Success Criteria

* < Goal of Bug is achived >
* After < Goal of Bug is achived >, the engine compiles, and passes the shell tests (run `mach jit-test` and `mach jstests`).

## Questions

If you have questions, feel free to visit us on in the [SpiderMonkey room on Matrix](https://matrix.to/#/!CZEbuMfGYVdQMIBKeP:mozilla.org?via=mozilla.org&via=igalia.com&via=matrix.org_), or post questions here.

## Tips and Tricks: 

* [SearchFox](https://searchfox.org/mozilla-central/source) indexes the Firefox codebase, and allows you to easily find functions, definitions, and more. It's a powerful tool!
* If you're looking at some code in SpiderMonkey, and are trying to figure out how it gets triggered, one of the easiest ways to do this is to inject a crash by putting `MOZ_RELEASE_ASSERT(false);` into the code, then running the tests. They will fails when they trigger that line.
```


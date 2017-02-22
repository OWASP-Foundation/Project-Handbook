# OWASP Project Handbook

This is a working copy of the OWASP Project Handbook using the 2014 version as the intial commit and is the location where changes are made before publishing a final version on the OWASP wiki.

The OWASP Project Handbook hasn't had any major revisions since 2014.  In order to start this process while updating how it is presented on the OWASP wiki, the content of the Handbook has been moved off the wiki into the cleverly named "original-2014-wiki-content" directory.  During the reorganization of the wiki content, the current project handbook pages are being 'protected' disallowing wiki accounts from editing them during the transition.

However to start the updates as soon as possible and in a easy to track and version method, the Project Handbook content has been converted to Markdown and placed in this GitHub repo.  This allows updating of the content while the wiki is being cleaned up.  It has the added benefit of providing a place to track additions and the reasons for them plus versioning the Project Handbook.

So, please feel free to contribute and provide feedback on this repo by:

* Submitting an issue in this repo with your feedback
* Forking the repo and providing PRs for any changes you'd like to see (simpliest and most direct)
* Requesting commit access.  We're happy to provide that but will require sensible commit messages so changes can be tracked/documented. NOTE: Bad commit messages is how you ask to have your commit privileges revoked.

Why convert to Markdown when the wiki will handle versions for us?

* We can use GitHub and git which is familiar to our project leaders already. We can track changes with commit messages and version the project handbook going forward. 
* Contributors are more likely to know Markdown then MediaWiki syntax
* We can update the content while making organizational changes to the wiki without disturbing the work on the content.  Doing things in parallel for the win!
* Edits can happen here and after being finalized in a new version, moved over to the wiki.  This allows for 'live and ever changing' content in GitHub with reviewed versions being the official policy as published on the OWASP wiki.
* Using the wonderful [pandoc program](http://pandoc.org/), conversion to markdown and back to MediaWiki markup is simple.
* We can also use [pandoc](http://pandoc.org/) to produce a downloadable PDF version with a single command
* All the cool kids are on GitHub and use Markdown

Repo structure:

```
Project-Handbook/
├── original-2014-wiki-content
│   ├── 01_overview.mediawiki
│   ├── 02_project-requirements.mediawiki
│   ├── 03_project-leader-expectations.mediawiki
│   ├── 04_owasp-project-lifecycle.mediawiki
│   ├── 05_owasp-project-stage-benefits.mediawiki
│   ├── 06_project-reviews.mediawiki
│   ├── 07_appendix.mediawiki
│   └── 08_acknowledgements.mediawiki
├── Project-Handbook_01_Overview.md
├── Project-Handbook_02_Project-Requirements.md
├── Project-Handbook_03_Project-Leader-Expectations.md
├── Project-Handbook_04_OWASP_Project-Lifecycle.md
├── Project-Handbook_05_OWASP_Project-Stage-Benefits.md
├── Project-Handbook_06_Project-Reviews.md
├── Project-Handbook_07_Appendix.md
├── Project-Handbook_08_Acknowledgements.md
└── README.md
```

Files with .mediawiki are copy/paste versions of the original content of the project handbook.  Files with .md are Markdown files converted by pandoc using the .mediawiki files as input.

An example of a command used to do the conversion from MediaWiki markup to Markdown

> $ pandoc 01_overview.mediawiki -f mediawiki -t markdown -o Project-Handbook_01_Overview.md

Once we're ready to move back to the wiki, we can pull the repo and use the inverse:

> $ pandoc Project-Handbook_01_Overview.md -f markdown -t mediawiki -o 01_overview.mediawiki

If you have problems with this repo or to request commit access, please use the [Contact Us Form](https://www.tfaforms.com/308703) and select "projects" as the area you need help with.

Thanks your project team Matt & Claudia

# Projects

A website that showcases projects! **If you want to use it and it's not exactly
fitting your purpose, please do make upstream changes. We expect this project
to be of use to others and we're happy to make it more generic so it's easier
to adapt to other organizations.** This was built by coala community, to view
live projects visit [projects.coala.io](https://projects.coala.io)

(It'd be nice to have an organization YML or so e.g.)

## Usage

To clone the repository and run this website on your local machine, [install Jekyll](https://jekyllrb.com/docs/installation/) for your OS and type the following commands:
				
    $ sudo gem install jekyll bundler
    $ git clone https://github.com/coala/projects.git
    $ cd projects
    $ bundle install
    $ bundle exec jekyll serve


Then you can simply go to either of the following addresses in your browser to access the site:

    127.0.0.1:4000
    localhost:4000

## Deploying & Contributing

1. make changes
2. run `bundle exec jekyll build` 
3. this builds to /docs folder
4. commit and push all files

NOTE: Template paths in app.js are relative to domain. (currently nemaniarjun.js.org) so template paths should match accordingly.

## Defining Projects

Mentors and admins can define projects in markdown using the following structure and save it in the _projects folder with a relevant filename:

```
---
name: "Write Project Name Here"
desc: "Write a one line Description of Project here."
requirements:
 - "The applicant has to fulfill this to get started."
difficulty: "low|medium|high"
issues:
 - "https://github.com/coala/coala/issues/####"
mentors:
 - sils
 - sims1253
initiatives:
 - GSoC
tags:
 - Plugins
 - CI
collaborating_projects:
 - "Add umbrella and sub-orgs here"
---

This space is for the main description. Use it wisely. 

#### Milestones

##### GSOC 2017 COMMUNITY BONDING

* Conceptual work should be finished.
* The student have a repository, know how to work with the community.
* The applicant should know the community.

##### GSOC 2017 MIDTERM

* Everything listed here has to be reviewed and merged by midterm.
* No exceptions to that. Changing the goals is possible together with mentors.
* Yes, that includes tests and documentation.

##### GSOC 2017 FINAL

* Everything has to be reviewed and merged.
* Including tests and docs, again.

```

## Defining FAQs

Users can also add FAQs by simply creating a markdown file in _faq folder.

Format for faq markdown file is as follows: 
```
---
Question: <Write the question here>
---

Answer
```

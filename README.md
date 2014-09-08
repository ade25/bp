# Introduction

## Blueprint buildout to kickstart new Plone or Pyramid projects

This buildout is best downloaded and cloned to a new and dedicated project
repository.

When in doubt you can always return to the blueprint/boilerplate buildout for
enhancements and inspiration concerning the latest "best practice" of
ade25 development and buildout scaffolding in general.

Note: this project is slowly developing into a basic development environment and is therefore a moving target. Do not use this new setup in projects yet.

## Buildout

This buildout is intended to be used via the development profile to provide
a ready to work on setup. Asuming you have cloned the buildout to a new
repository called 'my_project' the relevant steps to get started with a new
development environment would be:

``` bash
$ virtualenv-2.7 my_project
$ cd ./my_project
$ git clone gitlgithub.com:username/my_project.git buildout.my_project
$ cd ./buildout.my_project
$ python bootstrap.py -c development.cfg
$ bin/buildout -Nc development.cfg
```

*Note:* the hard requirement for Python 2.7.x for Plone development can of
course be skipped for Pyramid

## Development Packages

Project specific code is usually added as Python development eggs in the 'src'
directory and added to the auto-checkout part of *mr.developer*.


### Diazo Theme development

In order to start theme resource development it is required to initialize a
directory via yeoman generator. Follow the instructions found here:

https://github.com/ade25/generator-diazotheme



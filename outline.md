Setting up a Travis-CI Continuous Integration Environment for Your Drupal Module.
====

This session will focus on the use and benefits of a continuous integration environment.  We will walk through how to set up a continuous integration environment for a Drupal project using the hosted service called Travis-CI.

-----

## Intro
  - Who I am?
  - Summary of what we will cover.
    - A little about CI/CD
      - It all boils down to automating as much as possible.
      - There is a log to consider.
      - This talk will mostly deal with automated testing and some deployment.

    - Configure Travis-CI for a Drupal module project using pull requests strategy.
    - Configure Travis-CI Deployment for a OpenShift Drupal project.
    - A little on the near future of deployment.


## Continuous integration is complex:
   - Baby steps
   - Travis-CI is an easier way to get started in this world compared with JenkinsCI.

## The typical work flow.
  - Issues.
  - Developing code and adding features or fixes.
  - Testing & staging.
  - Merging accepted features.
  - Deploying changes.
    - There is a lot to something to consider at every step which is why it is complex.
  
## Travis-CI is a continuous integration service for GitHub projects.
  - i.e. Your project needs to be on GitHub for this to work.
  - Travis-CI lowers the bar for getting started in this world (tht is a good thing.)
  - TraviscI and GitHub are cool.
  - Compared to JenkinsCI, Travis does not give you as much control. But that just means less headaches.

## Drupal modules vs. Drupal projects.
  - Simply drupal projects will require a different setup than drupal modules (this should be obvious).


## Demo Drupal module
  - Travis-CI is configured via  .travis.yml file.
  - The easiest thing to do is just copy a working file.
  - For the purpose of the demo do this stepwise via pull requests.
    - Add .travis.yml to project. via pull requests.
    - Enable Travis project.
    - Edit README and push.
    - Done.

## Demo Drupal Project on OpenShift.
  - Main point of this is to demonstrate deployment.
    - Add .travis.yml
    - configure using travis gem.
    - Enable Travis-CI for project.
    - Edit README and push.
    - Done.


## A little prognostication about OpenShift and Docker.
 - RedHat has partnered with dotCloud to bring Docker to OpenShift.
   - Deployment will become trivial.

## Questions

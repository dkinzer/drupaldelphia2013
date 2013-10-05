Setting up a Travis-CI Continuous Integration Environment for Your Drupal Module.
====

This session will focus on the use and benefits of a continous integration environment.  We will walk through how to set up a continuous integration environment for a Drupal project using the hosted service called Travis-CI.

-----

## Intro
  - Who I am?
  - Summary of what we will cover.
    - A little about CI/CD
      - It all boils down to automating as much as possible.
      - There is a log to consider.
      - This talk will mostly deal with automated testing and some deployment.

    - Configure TravisCI for a Drupal module project using PUll Request stratgety.
    - Configure TravisCI Deployment for a Openshift Drupal project.
    - A little on the near future of deployment.


## Continuous integration is complex:
   - Babay steps
   - Travis-CI is an easier way to get started in this world compared with JenkinsCI.
   

## How I got here & Am I doing it wrong?
   - I made a big mistake that forced me to reconsider how I deployed to live.
   - Thinking about and doing this stuff will help you better understand and appreciate your stack.
    

## The typical workflow.
  - Issues.
  - Developing code and adding features or fixes.
  - Testing & staging.
  - Merging accepted features.
  - Deploying changes.
    - There is a lot to something to consider at every step which is why it is complex.
  
## Travis-CI is a continuous integration service for GitHub projects.
  - i.e. Your project needs to be on GitHub for this to work.
  - Be warned, there is some controversy here
    - see https://groups.drupal.org/node/313068
    - But despite the controversy some projects are already hosted on Drupal.
  - TravisCI lowers the bar for getting started in this world (tht is a good thing.)
  - TraviscI and GitHub are cool.
  - Compared to JenkinsCI, Travis does not give you as much control. But that just means less headaches.

## Drupal modules vs. Drupal projects.
  - Simply drupal projects will require a different setup than drupal modules (this should be obvious).


## Demo Drupal module
  - TravisCIs is configured via  .travis.yml file.
  - The easiest thing to do is just copy a working file.
  - For the purpose of the demo do this stepwise via pull requests.
    - Add travis.yml to project. via pull requests.
    - Enable travis project.
    - Edit README and push.
    - Done.

## Demo Drupal Project on OpenShift.
  - Main point of this is to demonstrate deployment.
    - Add travis.yml
    - configure using travis gem.
    - Enable travisci for project.
    - Edit README and push.
    - Done.


## A little prognostication about OpenShift and Docker.
 - RedHat has partnered with dotCloud to bring Docker to OpenShift.
   - Deployment will become trivial.

## Questions

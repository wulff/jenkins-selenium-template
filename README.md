Jenkins Selenium template
=========================

A basic template for setting up Selenium jobs in Jenkins.


Installation
------------

1. Copy this directory to `/var/lib/jenkins/jobs/selenium-template`.
2. Create a new job and select *Copy existing job*, enter `selenium-template` in the *Copy from* field.
3. Uncheck the *Disable Build* checkbox
4. Configure the *Source Code Management* build step to check out a copy of the repository containing your Selenium tests.
5. Modify the *SeleniumHQ htmlSuite Run* build step to match the location of your tests plans and to add any additional arguments to JMeter.


Requirements
------------

To use this template in Jenkins you must install the *Hudson Seleniumhq* plugin.

The *X virtual framebuffer* package (xvfb)  must be installed on the Jenkins server.
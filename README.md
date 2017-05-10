Showcase Insurance Application with Document Management System
======================

This project has been generated by the Maven archetype
[camunda-archetype-ejb-war-7.2.2-SNAPSHOT](http://docs.camunda.org/latest/guides/user-guide/#process-applications-maven-project-templates-archetypes).


How does it work?
-----------------
This showcase uses Apache Chemistry (available with a inmemory repository) as Document Management System to store and show documents uploaded by the customers.

The changes to the standard demo are in Document-Request-Process. In a user task the applicant can login and upload the document.

The clerk has to check the documents and they are visibile in the decide-task, too.

Install Apache-Chemisty in a separate server (or in the appserver, if you want to) and use the frontend to see the documents.

This demo is inspired by the invoice-cmis-example: [https://github.com/camunda/camunda-consulting/tree/master/snippets/ecm-integrations/invoice-cmis](https://github.com/camunda/camunda-consulting/tree/master/snippets/ecm-integrations/invoice-cmis)

Here is a video to see the invoice example in action: [https://vimeo.com/193860956](https://vimeo.com/193860956) or the german version [https://vimeo.com/193861217](https://vimeo.com/193861217)    

How to use it?
--------------

You can use `ant` to build and deploy the example to an application server.
For that to work you need to copy the file `build.properties.example` to `build.properties`
and configure the path to your application server inside it.
Alternatively, you can also copy it to `${user.home}/.camunda/build.properties`
to have a central configuration that works with all projects generated by the
[Camunda BPM Maven Archetypes](http://docs.camunda.org/latest/guides/user-guide/#process-applications-maven-project-templates-archetypes).

Once you deployed the application you can run it using
its [web interface](http://localhost:8080/versicherungsneuantrag/online).
The use
[Camunda Tasklist](http://docs.camunda.org/latest/guides/user-guide/#tasklist)
to work on user tasks and inspect it using
[Camunda Cockpit](http://docs.camunda.org/latest/guides/user-guide/#cockpit).

In the file `src/main/webapp/app.js` you can switch between the two process versions.

Alternatively, you can also have a look at `NeuantragProcessTest`,
but before running it set your email address in `DemoData`.  

Environment Restrictions
------------------------

Built and tested against Camunda BPM version 7.2.0.


Known Limitations
-----------------


Improvements Backlog
--------------------


License
-------

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

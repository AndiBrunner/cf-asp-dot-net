Cloud Foundry ASP.Net Buildpack
===============================


The cf-asp-dot-net <code>buildpack</code> is a <a href="http://www.cloudfoundry.com" title="Cloud Foundry">Cloud Foundry</a> buildpack for running ASP.Net applications with <a href="http://www.mono-project.com" title="Mono">Mono</a>. Currently the status of the project is experimental. It deploys and automatically configures NginX and Mono to host your applications.


Instructions
------------


The build pack has some conventions for the format of your application. It expects a folder structure like this.

- www --> your application files & static resources</li>

Usage
-----

To use this buildpack specify the URI of the repository when pushing an application to Cloud Foundry:

		cd my-app-dir			 #top level directory for your project
		cf push myApp -b https://github.com/AndiBrunner/cf-asp-dot-net.git

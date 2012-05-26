Maven Repository
================
This is my public maven repository hosted on Github. I use this to host my own libraries, archetypes, and libraries that I use in my projects that aren't currently in a maven repo elsewhere. This means that I do not own everything in this repo.
	
Libraries
---------

Add the following to your .pom file to get access to the libraries:

	<repositories>
		[...]
		<repository>
			<id>nolat.org</id>
			<name>Nolat</name>
			<url>https://raw.github.com/Talon876/repo/master/releases </url>
		</repository>
	</repositories>
	
Current Libraries:

* [`toolkit`](https://github.com/Talon876/Toolkit) - A library that makes it easy to perform common mathematical functions, and adds a Vector2 class.

    

Development Commands
--------------------

Deploy a third party jar:
	
	mvn deploy:deploy-file -Durl=file:PATH_TO_LOCAL\repo\releases -Dfile=theirfile.jar -DgroupId=com.whatever -DartifactId=thing -Dversion=1.0 -Dpackaging=jar

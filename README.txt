
Granite Data Services for JDK 1.4 Port(http://www.graniteds.org) Source Code
----------------------------------------------------------------------------------

* Important

  Currently, only the Granite Data POJO and Spring Services have been ported to JDK 1.4.
  As such you can use only the POJO services or Spring Services in a JDK 1.4 environment

* Requirements:

  Eclipse 3.2+, JDK 5+, JDK 1.4. You MUST have the core graniteds project already
  installed.

* Installation:

  Right click in your Eclipse Package Explorer, choose "Import...", then
  "General" -> "Existing Projects into Workspace", choose "Select archive file",
  browse to graniteds-jdk14-***.zip and click on "Finish".

* Configuration:

  Open env.properties (WITH A SIMPLE TEXT EDITOR) and adjust the first
  2 variables (GRANITE_HOME AND JAVA_14_LIB).

* Full Build:

  Open an Ant view ("Window" -> "Show View" -> "Ant"), drag an drop build.xml
  from the "Package Explorer" view to the "Ant" view, expend "graniteds_jdk14" node
  and double click on "distrib.all". Please ensure that you have executed the Granite
  Data Services "distrib.all" before running this full build.

* Usage

  Copy lib/backport-util-concurrent-***.jar, lib/retrotranslator-runtime-***.jar,
  lib/test-backport.jar, build/graniteds-jdk14.jar and, optionally,
  build/graniteds-spring-jdk14.jar to the WEB-INF/lib directory of your web application.
  Now you can run GraniteDS Pojo Services or Spring Services in a jdk 1.4 environment.

* RetroTranslator

  The translation of Grantie Data Services to JDK 1.4 is achieved using RetroTranslator.
  (http://retrotranslator.sourceforge.net/). This distribution contains the required compile
  time and runtime retrotranslator files.

  The following are RetroTranslator related files:
  retrotranslator-runtime-***.jar
  retrotranslator-transformer-***.jar
  test-backport.jar --> A fix for ProcessBuilder translation in RetroTranslator



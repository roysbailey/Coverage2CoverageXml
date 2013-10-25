Coverage2CoverageXml
====================

CoverageXml files contain code coverage information regarding unit tests run from Visual Studio.  
Third party tools have popped up to generate "reports" and the like from these CoverageXML files, which is great when 
running tests as part of an automated build process.  Unfortunately, as of Visual Studio 2012, you can no longer 
generate "coverageXml" files from the command line.  

Instead, the new command line runner, vstest.console.exe produces a binary ".coverage" file.  This little tool fixes 
this issue, and can recursively look for ".coverage" files and convert them to the ".coverageXml" format, so you can 
still build your reports etc. as part of your automated build.

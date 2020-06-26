WebGoat is a test J2EE web application provided by the Open Web Application
Security Project (http://www.owasp.org). This directory contains the WebGoat
5.0 sources.

WebGoat java sources can be used directly for java vulnerability scanning 
via Fortify Source Code Analysis Engine. You can scan as follows:

$ sourceanalyzer -b WebGoat5.0 -clean
$ sourceanalyzer -b WebGoat5.0 -source 1.5 -cp "WebGoat5.0/WebContent/WEB-INF/lib/*.jar" WebGoat5.0/JavaSource WebGoat5.0/WebContent
$ sourceanalyzer -b WebGoat5.0 -scan -f WebGoat5.0.fpr

See the User Manual for full details on performing a scan.

Example output for a scan of this project is located under
Samples/basic/sampleOutput/WebGoat5.0.fpr

Important:
Please don't make this application accessible outside of your firewall or 
to people you don't trust. It contains planted vulnerabilities for testing.


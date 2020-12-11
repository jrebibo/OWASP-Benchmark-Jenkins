# OWASP Benchmark
The OWASP Benchmark Project is a Java test suite designed to verify the speed and accuracy of vulnerability detection tools. It is a fully runnable open source web application that can be analyzed by any type of Application Security Testing (AST) tool, including SAST, DAST (like <a href="https://owasp.org/www-project-zap">OWASP ZAP</a>), and IAST tools. The intent is that all the vulnerabilities deliberately included in and scored by the Benchmark are actually exploitable so its a fair test for any kind of application vulnerability detection tool. The Benchmark also includes scorecard generators for numerous open source and commercial AST tools, and the set of supported tools is growing all the time.

The project documentation is all on the OWASP site at the <a href="https://owasp.org/www-project-benchmark">OWASP Benchmark</a> project pages. Please refer to that site for all the project details.

The current latest release is v1.2. Note that all the releases that are available here: https://github.com/OWASP/Benchmark/releases, are historical. The latest release is always available live by simply cloning or pulling the head of this repository (i.e., git pull).

Personal Notes:

Requirements 
- Maven: https://maven.apache.org/  (Version: 3.2.3 or newer works.)
- Java: https://www.oracle.com/java/technologies/javase-downloads.html (Java 7 or 8) (64-bit)

$ cd benchmark
$ mvn compile   (compiles with maven)
- make sure $JAVA_HOME is pointed to java8 (JAVA_HOME=(/usr/libexec/java_home -v 1.8))
$ bash runBenchmark.sh/.bat   (bash script starts the 'web app')
- [talledLocalContainer] Tomcat 8.x

Available Categories Index:
Command Injection Category
Cryptographic Category
Weak Hashing Category
LDAP Injection Category
Path Traversal Category
Secure Cookie Category
SQL Injection Category
Trust Boundary Category
Weak Randomness Category
XPATH Injection Category
XSS (Cross-Site Scripting) Category
##Jmeter-Maven-Showcsae

Running the jmeter-maven-plugin

>mvn com.lazerycode.jmeter:jmeter-maven-plugin:1.4.1:jmeter

on any maven project that contain certain path `/src/test/jmeter/` 

will execute all the `*.jmx` Jmeter tests from this path.

Assuming we are having `src/test/jmeter/showcase-loadtest-plan.jmx` Jmeter descriptor

then after the launch we will got

Logs are available at: `target/jmeter/jmeter-logs/showcase-loadtest-plan.jmx.log`

CSV Report at: `target/jmeter/report/showcase-loadtest-plan-170921.jtl`

HTML Report `target/jmeter/report/showcase-loadtest-plan-170921.jtl-report.html`

In case will proceed with it in a regular bases, it may be formed in corresponded pom as follows:

then execution might be followed:

> mvn verify
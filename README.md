[![Apache Sling](https://sling.apache.org/res/logos/sling.png)](https://sling.apache.org)

&#32;[![Build Status](https://ci-builds.apache.org/job/Sling/job/modules/job/sling-org-apache-sling-contentparser-xml-jcr/job/master/badge/icon)](https://ci-builds.apache.org/job/Sling/job/modules/job/sling-org-apache-sling-contentparser-xml-jcr/job/master/)&#32;[![Test Status](https://img.shields.io/jenkins/tests.svg?jobUrl=https://ci-builds.apache.org/job/Sling/job/modules/job/sling-org-apache-sling-contentparser-xml-jcr/job/master/)](https://ci-builds.apache.org/job/Sling/job/modules/job/sling-org-apache-sling-contentparser-xml-jcr/job/master/test/?width=800&height=600)&#32;[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=apache_sling-org-apache-sling-contentparser-xml-jcr&metric=coverage)](https://sonarcloud.io/dashboard?id=apache_sling-org-apache-sling-contentparser-xml-jcr)&#32;[![Sonarcloud Status](https://sonarcloud.io/api/project_badges/measure?project=apache_sling-org-apache-sling-contentparser-xml-jcr&metric=alert_status)](https://sonarcloud.io/dashboard?id=apache_sling-org-apache-sling-contentparser-xml-jcr)&#32;[![JavaDoc](https://www.javadoc.io/badge/org.apache.sling/org.apache.sling.contentparser.xml-jcr.svg)](https://www.javadoc.io/doc/org.apache.sling/org.apache.sling.contentparser.xml-jcr)&#32;[![Maven Central](https://maven-badges.herokuapp.com/maven-central/org.apache.sling/org.apache.sling.contentparser.xml-jcr/badge.svg)](https://search.maven.org/#search%7Cga%7C1%7Cg%3A%22org.apache.sling%22%20a%3A%22org.apache.sling.contentparser.xml-jcr%22)&#32;[![contentparser](https://sling.apache.org/badges/group-contentparser.svg)](https://github.com/apache/sling-aggregator/blob/master/docs/groups/contentparser.md) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

Apache Sling Content Parser for Jackrabbit FileVault XML
====
This module is part of the [Apache Sling](https://sling.apache.org) project.

The Apache Sling Content Parser for Jackrabbit FileVault XML provides support for parsing XML files into Apache Sling resource trees, by implementing the 
API provided by the [`org.apache.sling.contentparser.api`](https://github.com/apache/sling-org-apache-sling-contentparser-api) bundle.

To obtain a reference to the Jackrabbit FileVault XML content parser just filter on the `ContentParser.SERVICE_PROPERTY_CONTENT_TYPE` service registration 
property:

```java
    @Reference(target = "(" + ContentParser.SERVICE_PROPERTY_CONTENT_TYPE + "=jcr-xml)")
    private ContentParser jcrXmlParser;
``` 

resource-filters
================

Resource filters allow resource providers to define which parts of
a resources they want to shared with a grantee.

One resource can be shared with multiple grantees, each with their own resource-filter.

Example usage:

    xsltproc filter.xslt --stringparam filter client_basic.xml example/resource1.xml
    saxon example/resource1.xml filter.xslt filter=client_basic.xml

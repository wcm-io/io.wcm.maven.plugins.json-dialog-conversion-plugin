About JSON Dialog Converter Plugin
=======================

Converts AEM Dialog Definitions in JSON Format with Rules from [Adobe AEM Dialog Conversion Tool](https://github.com/Adobe-Marketing-Cloud/aem-dialog-conversion).

[![Maven Central](https://maven-badges.herokuapp.com/maven-central/io.wcm.maven.plugins/json-dialog-conversion-plugin/badge.svg)](https://maven-badges.herokuapp.com/maven-central/io.wcm.maven.plugins/json-dialog-conversion-plugin)


### Documentation

* [Plugin Documentation][plugindocs]
* [Changelog][changelog]


### Overview

Execute on a maven project with

```
mvn io.wcm.maven.plugins:json-dialog-conversion-plugin:convert
```

Make sure you have a backup / SCM commit before executing the tool! You have to review the conversion in detail, it may need further manual adjustments.

Unfortunately the conversion removes all formatting and comments from the JSON files.

If you want to get an exact diff of the conversion in your SCM without all the reformatting noise, you can execute a reformat-only run first, commit it, and then start the conversion:

```
mvn io.wcm.maven.plugins:json-dialog-conversion-plugin:convert -Dconvert.formatOnly=true
```


[plugindocs]: plugin-info.html
[changelog]: changes-report.html
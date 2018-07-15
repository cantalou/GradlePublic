# GradlePublic

### bintray_2.gradle
It is used to public your project to jcenter. Working base on gradle 2.14.1 and gradle android plugin 2.1.3  
> 1. add build dependency config to root project build.gradle file
  classpath 'com.jfrog.bintray.gradle:gradle-bintray-plugin:1.7'
  
> 2. add follow to build.gradle file of library project  
  apply from : "https://raw.githubusercontent.com/cantalou/GradlePublic/master/bintray_2.gradle"  
  
> 3. add follow properties to gradle.properties of library project  
  BINTRAY_USER=****  
  BINTRAY_KEY****  
  PROJ_GROUP=****  
  PROJ_VERSION=****(format 1.0.1)  
  PROJ_NAME=****  
  PROJ_WEBSITEURL=****  
  PROJ_ISSUETRACKERURL=****  
  PROJ_VCSURL=****  
  PROJ_DESCRIPTION=****  
  PROJ_ARTIFACTID=****  
  DEVELOPER_ID=****  
  DEVELOPER_NAME=****  
  DEVELOPER_EMAIL=****  
  
> gradle aR bintray --info -PpublicType=all   
> publicType has three value : all , aar, jar

### keepResourcesId.gradle
It is used to make the generated resource id identical every time when build task runs.
Support:   
1.Resource add and delete  
2.Compile dependency and empty implement in release dependency  

### genTypeNameId.gradle
It is used to generate a file which contains line base text formating color and drawable resources by "type:name:id" into assets dir.

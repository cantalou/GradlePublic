# GradlePublic

### bintray_2.gradle
It is used to public you project to jcenter. Working base on gradle 2.14.1 and gradle android plugin 2.1.3  
> gradle aR bintray --info -PpublicType=all   
> publicType has three value : all , aar, jar

### keepResourcesId.gradle
It is used to make the generated resource id identical every time when build task runs.
Support:   
1.Resource add and delete  
2.Compile dependency and empty implement in release dependency  

### genTypeNameId.gradle
It is used to generate a file which contains line base text formating color and drawable resources by "type:name:id" into assets dir.

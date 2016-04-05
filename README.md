# appArchetype

Useage:

mvn archetype:generate \
        -DarchetypeGroupId=com.company.archetype \
        -DarchetypeArtifactId=appArchetype \
        -DarchetypeVersion=1.2-SNAPSHOT \
        -DarchetypeCatalog=local \
        -DinteractiveMode=false \
        -DgroupId=com.company \
        -DartifactId=$artifactName \
        -DappName=$appName

$artifactName and $appName can be the same value

I want the value passed into the -DappName parameter above to be inserted into the corresponding variable in logback.xml
The problem is that with both archetype.xml and archetype-metadata.xml present, the resources in archetype.xml do not get copied into the project generated. 

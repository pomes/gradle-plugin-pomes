# Gradle Props plugin

A very small plugin that reads in Java property files 
and adds the properties to the project under `project.propertyFiles`

To add a property file, just provide its name (no extension) in the
`propertyFiles` block. In the example below I read in the `secrets.properties`
file:

````
propertyFiles {
    secrets {}
}
````

To access the the property:

````
project.propertyFiles.secrets.properties.<property name>
````

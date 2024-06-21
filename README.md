This sample is to demo jackson-databind lib issue which is not able to add type details of root node while serializing a kotlin data class which extends an abstract class using jackson databind Polymorphic deseriazer activatedefaultTyping

Serialized payload miss type details of root node, example 

current:

{"lastInSeason":true,"synopsis":["java.util.ArrayList",["my synopsis1"]]}

Expected:

{"@class":"Movie","lastInSeason":true,"synopsis":["java.util.ArrayList",["my synopsis1"]]}

### jmapper
---
https://github.com/jmapper-framework/jmapper-core

https://jmapper-framework.github.io/jmapper-core/

```java
JMapperAPI jmapperAPI = new JMapperAPI()
  .add(mappedClass(Destination.class)
    .add(attribute("id")
      .value("id"))
    .add(attribute("destinationField")
      .value("sourceField")));


JMapper<Destination, Source> mapper;

mapper = new JMapper<>(Destination.class, Source.class);

mapper = new JMapper<>(Destination.class, Source.class, xml);

mapper = new JMapper<>(Destination.class, Source.class, jmapperAPI);

Source source = new Source("id", "sourceField", "other");
Destination destination = mapper.getDestination(source);

destination ["id", "sourceField", null]

class Destination {  class Source{
  @JMap
  private String id; private String id;
  @JMap("sourceField")
  private String destinationField; private String sourceField;
  private String destinationField; private String sourceField;
  private String other; private Stirng other;
}  }
```

```
```

```
```



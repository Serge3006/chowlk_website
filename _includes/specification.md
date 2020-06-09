## 2. Specification

### 2.1 Classes and Individuals

<table style="width:100%">
  <tr>
    <th>Diagram BLOCK</th>
    <th>OWL Element</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><img src="images/class.jpg" alt="Class block"></td>
    <td><code>owl:Class</code></td>
    <td>Block to represent classes within the ontology conceptualization. 
    The content of the block should be accompanied with the prefix and the name of the concept on order to fully identify it.</td>
  </tr>
  <tr>
    <td><img src="images/unnamed_class.jpg" alt="Unnamed block"></td>
    <td><code>owl:Class</code></td>
    <td>Block to represent an unnamed or anonynoums class. Used to declare a restriction over a named class.</td>
  </tr>
  <tr>
    <td><img src="images/individual.jpg" alt="Individual block"></td>
    <td><code>owl:Individual</code></td>
    <td>Block to represent individuals</td>
  </tr>
</table>

### 2.2 Universal Restriction for Object Properties

<table style="width:100%">
  <tr>
    <th style="width:45%">Diagram BLOCK</th>
    <th style="width:40%">OWL Element</th>
    <th style="width:35%">Description</th>
  </tr>

  <tr>
    <td><img src="images/universal_restriction_1.jpg" alt="Universal restriction block"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty1 ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Universal restriction form 1.</td>

  </tr>

</table>
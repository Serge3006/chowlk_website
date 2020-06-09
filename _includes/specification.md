## 2. Specification

### 2.1 Classes and Individuals

<table style="width:100%">
  <tr>
    <th style="width:20%">Diagram BLOCK</th>
    <th style="width:20%">OWL Element</th>
    <th style="width:60%">Description</th>
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

### 2.2 Universal Restrictions for Object Properties

<table style="width:100%">
  <tr>
    <th style="width:20%">Diagram BLOCK</th>
    <th style="width:45%">OWL Element</th>
    <th style="width:35%">Description</th>
  </tr>

  <tr>
    <td><img src="images/universal_restriction_1.jpg" alt="Universal restriction block" height="50%"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Form 1 of an universal restriction between 2 concepts. <code>Class1</code> is subclass of an anonymus concept which has an object property <code>objectProperty</code>, and all the individuals for this property shall come from <code>Class2</code></td>

  </tr>

  <tr>
    <td><img src="images/universal_restriction_2.jpg" alt="Universal restriction block" height="50%"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Form 2 of an universal restriction between 2 concepts.</td>

  </tr>

  <tr>
    <td><img src="images/universal_restriction_3.jpg" alt="Universal restriction block" height="50%"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Form 3 of an universal restriction between 2 concepts.</td>

  </tr>

</table>


### 2.3 Existential Restrictions for Object Properties

<table style="width:100%">
  <tr>
    <th style="width:20%">Diagram BLOCK</th>
    <th style="width:45%">OWL Element</th>
    <th style="width:35%">Description</th>
  </tr>

  <tr>
    <td><img src="images/existential_restriction_1.jpg" alt="Existential restriction block" height="50%"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty1 ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Form 1 of an existential restriction between 2 concepts. <code>Class1</code> is subclass of an anonymus concept which has an object property <code>objectProperty1</code>, and some the individuals for this property shall come from <code>Class2</code></td>

  </tr>

  <tr>
    <td><img src="images/existential_restriction_2.jpg" alt="Existential restriction block" height="50%"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty1 ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Form 2 of an existential restriction between 2 concepts.</td>

  </tr>

  <tr>
    <td><img src="images/existential_restriction_3.jpg" alt="Existential restriction block" height="50%"></td>
    <td><code>ns:Class1 rdf:type owl:Class ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:subClassOf [ rdf:type owl:Restriction ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:onProperty ns:objectProperty1 ;<br></code>
				&emsp;&emsp;&emsp;<code>owl:allValuesFrom ns:Class2 ] .</code></td>
    <td>Form 3 of an existential restriction between 2 concepts.</td>

  </tr>

</table>

### 2.3 Domain and Range for Object Properties

<table style="width:100%">

  <tr>
    <th style="width:20%">Diagram BLOCK</th>
    <th style="width:45%">OWL Element</th>
    <th style="width:35%">Description</th>
  </tr>

  <tr>
    <td><img src="images/no_domain_no_range_op_1.jpg" alt="Domain and Range" height="50%"></td>
    <td><code>ns:objectProperty rdf:type owl:ObjectProperty .</code></td>
    <td>Object property <code>ns:objectProperty</code> without domain and range form 1.</td>

  </tr>

  <tr>
    <td><img src="images/no_domain_no_range_op_2.jpg" alt="Domain and Range" height="50%"></td>
    <td><code>ns:objectProperty rdf:type owl:ObjectProperty .<br></td>
    <td>Object property <code>ns:objectProperty</code> without domain and range form 2.</td>

  </tr>

  <tr>
    <td><img src="images/yes_domain_yes_range_op_1.jpg" alt="Domain and Range" height="50%"></td>
    <td><code>ns:objectProperty rdf:type owl:ObjectProperty ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:domain owl:Class1 ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:range owl:Class2 .<br></code></td>
    <td>Object property <code>ns:objectProperty</code> with domain and range form 1.</td>

  </tr>

  <tr>
    <td><img src="images/yes_domain_yes_range_op_2.jpg" alt="Domain and Range" height="50%"></td>
    <td><code>ns:objectProperty rdf:type owl:ObjectProperty ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:domain owl:Class1 ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:range owl:Class2 .<br></code></td>
    <td>Object property <code>ns:objectProperty</code> with domain and range form 2.</td>

  </tr>

  <tr>
    <td><img src="images/yes_domain_no_range_op.jpg" alt="Domain and Range" height="50%"></td>
    <td><code>ns:objectProperty rdf:type owl:ObjectProperty ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:domain owl:Class1 .</code></td>
    <td>Object property <code>ns:objectProperty</code> with domain but without range.</td>

  </tr>

  <tr>
    <td><img src="images/no_domain_yes_range_op.jpg" alt="Domain and Range" height="50%"></td>
    <td><code>ns:objectProperty rdf:type owl:ObjectProperty ;<br></code>
        &emsp;&emsp;&emsp;<code>rdfs:range owl:Class2 .</code></td>
    <td>Object property <code>ns:objectProperty</code> with range but without domain.</td>

  </tr>


</table>
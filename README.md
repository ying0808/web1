# web1
<?xml version="1.0"?>
<rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
                xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#"
                xml:base="http://www.nfu.edu.tw/csie/11263114">

    <rdfs:Class rdf:ID="Stream">
        <rdfs:subClassOf rdf:resource="#NaturallyOccurringWaterSource"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="BodyOfWater">
        <rdfs:subClassOf rdf:resource="#NaturallyOccurringWaterSource"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="Brook">
        <rdfs:subClassOf rdf:resource="#Stream"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="River">
        <rdfs:subClassOf rdf:resource="#Stream"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="Tributar">
        <rdfs:subClassOf rdf:resource="#Stream"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="Lake">
        <rdfs:subClassOf rdf:resource="#BodyOfWater"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="Ocean">
        <rdfs:subClassOf rdf:resource="#BodyOfWater"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="Sea">
        <rdfs:subClassOf rdf:resource="#BodyOfWater"/>
    </rdfs:Class>

    <rdfs:Class rdf:ID="Rivulet">
        <rdfs:subClassOf rdf:resource="#Brook"/>
    </rdfs:Class>

    <rdf:Property rdf:ID="emptiesInto">
        <rdfs:domain rdf:resource="#River"/>
        <rdfs:range rdf:resource="#BodyOfWater"/>
    </rdf:Property>

    <rdf:Property rdf:ID="length">
        <rdfs:domain rdf:resource="#River"/>
        <rdfs:range rdf:resource="http://www.w3.org/2000/01/rdf-schema#Literal"/>
    </rdf:Property>

</rdf:RDF>

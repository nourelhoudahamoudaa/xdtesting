Test case ID: sq1.ttl
Test category: competency question verification test
Requirement: where was the musical composition performed?
Test: PREFIX mp: <https://w3id.org/polifonia/ontology/musical-performance/> PREFIX core: <https://w3id.org/polifonia/ontology/core/> SELECT DISTINCT ?place WHERE { ?composition mp:isInvolvedInMusicalPerformance ?performance . ?performance core:hasPlace ?place }"
Input test data: DatasetSQ.ttl
Expected result: {\"head\": {  \"vars\": [  \"place\" ] } ,  \"results\": {  \"bindings\": [ {  \"place\": {  \"type\":  \"uri\" ,  \"value\":\"https://raw.githubusercontent.com/polifonia-project/musical-performance/main/test/competency-question/toy-dataset/Florence\" } } ] } }
Actual result: Error Broken token (newline)
Executed on: Jan 18 2023
Environment: MacOS
Execution result: Fail
Execution comment:



Test case ID: iv1.ttl
Test category: inference verification test
Requirement: -
Test: PREFIX mp: <https://w3id.org/polifonia/ontology/musical-performance/> 
PREFIX td: <https://raw.githubusercontent.com/polifonia-project/musical-performance-ontology/main/test/inference/toy-dataset/ > 
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#> 
ASK { td:Session01 a mp:Session }"
Input test data: DatasetIV.ttl
Expected result: True
Actual result: Error Broken token (newline)
Executed on: Jan 18 2023
Environment: MacOS
Execution result: Fail
Execution comment:


Test case ID: ep1.ttl
Test category: error provocation test
Requirement: -
Test: -
Input test data: DatasetEP.ttl
Expected result: True
Actual result: Error - Could not parse ontology.
Executed on: Jan 18 2023
Environment: MacOS
Execution result: Fail
Execution comment:

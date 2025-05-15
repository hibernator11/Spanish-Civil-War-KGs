# Spanish-Civil-War-KGs
Extracting Knowledge Graphs as Collections as Data using the Spanish Civil War as main topic

### Introduction
This project intends to analyse the options and potential of Wikidata to extract Collections as Data from Wikidata using the Spanish Civil War and Exile as main topic.

### Artists from the Republic and Spanish Civil War

```
SELECT *
WHERE { 
    VALUES ?artist {
        wd:Q5593 wd:Q152384 wd:Q2447692 wd:Q235275 wd:Q5660510 
        wd:Q118936 wd:Q979226 wd:Q134644 wd:Q921933 wd:Q5994858 
        wd:Q1042706 wd:Q3398317 wd:Q51545 wd:Q467712 wd:Q77347 wd:Q236161}
    ?artist wdt:P31 ?type .
    ?artist wdt:P19 ?placebirth .
    SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
}
```

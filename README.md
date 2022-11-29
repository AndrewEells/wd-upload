# Wikidata Upload from LDConnect
Currently configured to point to [https://test.wikidata.org](https://test.wikidata.org/)

## Note: the properties below were tweaked to link to similar datatypes on test.wikidata.org, they will be changed when pushed to production wikidata. (See comments in code)

- Quantity ([test.wikidata P69](https://test.wikidata.org/wiki/Property:P69)) -> Number of Pages ([wikidata P1104](https://www.wikidata.org/wiki/Property:P1104))
- Main Subject ([text.wikidata P96524](https://test.wikidata.org/wiki/Property:P96524)) -> Main Subject ([wikidata P921](https://www.wikidata.org/wiki/Property:P921))
	- main subject is a string property on text.wikidata, and an item property on production. still working out a reliable way to correlate keywords to reliable wikidata items (currently considering using a list of keywords, and entering a correlating property for each, but this isn't sustainable long-term)
- Stated In ([test.wikidata P149](https://test.wikidata.org/wiki/Property:P149)) -> Published In ([wikidata P1433](https://www.wikidata.org/wiki/Property:P1433))
	- semantic mediawiki ([test.wikidata Q213541](https://test.wikidata.org/wiki/Q213541)) -> Semantic Web: Interoperability, Usability, Applicability ([wikidata Q15917015](https://www.wikidata.org/wiki/Q15817015))
	- this applies both in the main property and as it is used in the references
- P356: DOI ([test.wikidata P97017](https://test.wikidata.org/wiki/Property:P97017)) -> DOI ([wikidata P356](https://www.wikidata.org/wiki/Property:P356))

### Resulting Entries (on Test.Wikidata):

- SW190368 --- [Neural-symbolic integration and the Semantic Web](https://test.wikidata.org/wiki/Q226972)
- SW190371 --- [Leveraging Knowledge Graphs for Big Data Integration: the XI Pipeline](https://test.wikidata.org/wiki/Q226985)
- SW190372 --- [The Semantic Web identity crisis: In search of the trivialities that never were](https://test.wikidata.org/wiki/Q226988)
- SW190373 --- [Neural language models for the multilingual, transcultural, and multimodal Semantic Web](https://test.wikidata.org/wiki/Q226989)
- SW190374 --- [On the role of knowledge graphs in explainable AI](https://test.wikidata.org/wiki/Q226990)

# Programming in the Life Sciences
## Description
Repository made in the context of a project for the Programming in the Life Sciences practical at the Maastricht Science Programme (Maastricht University). The goal is to retrieve data from the Wikidata SPARQL endpoint, analyze the results in JavaScript, and visualise them on a webpage using d3.js and HTML.
## Project Content
### Biological Question
<ins>What is the global geographic and taxonomic distribution of *Panthera* genus, and how do their native country counts compare across continents?</ins>\
The panthera genus, also known as big cats, is composed of Lions, Tigers, Leopards, Jaguars and Snow leopards. Their genus' name does not refer so much to their size as much as it does to their anatomical characteristics which allows them to roar, which other felids do not possess regardless of their size.\
This question was chosen for a number of reasons. First of all it has the potential for an interesting and interactive website visualisation, it also seems, upon first thought, like a simple enough question to grasp and do data retrieval and coding visualisations for as a beginner.
### SPARQL queries
So far I believe I will be needing three separate SPARQL queries, one finding the geographical distribution of the species, one giving me their numbers in each country, region or continent, depends on where I can find the best numbers, and one giving me the carrying sound bytes of each species.
## Project log
### Week 2
So in order to answer this question, I need two types of data, first the geographical distribution of each of the species and second their numbers in each country, or each general area.\ 
Tried a first SPRQL query to get the county distribution, but it only came up with 27 countries and often only one species per country. Upon looking at the Wikidata entries for the 6 species I realised that some had taxon range maps, showing the geographical spread but didn't have the taxon range listed, which was why it wasn't coming up in my SPRQL query.\
My next step was to try and add the missing statements in each entry, however given that these are highly searched entries they are partially protected from editing, which means that I have to wait until I have over 50 other edits and that my account is 4 days old. I spent the 2nd session making a number of those needed 50 edits on subspecies of the initial species until I could edit the bigger entry, and it worked because when I rerun my initial query I got 50 countries and multiple species in each, still not a complete dataset but closer. I hope that the half protected status of the entries will change so that I am able to get the necessary data for the question.
### Week 3
Further editing of the Wikidata pages, I finally got access to the semi protected Wikidata entries such as lion, by the end of it my query gave me 127 entries, however I believe it included countries multiple times, once with the species name and then with the subspecies which is why I will have to change the query to filter them out or find a way to group the countries and subspecies, to be determined. I also created a first html file, tested an extremely basic layout and inout some baselines.
## License
This project is licensed under the MIT License.

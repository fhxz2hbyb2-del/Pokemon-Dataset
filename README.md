## About this dataset 
<img src="https://lh5.googleusercontent.com/proxy/8Hk_DCSj7YFmPPJxUqBfZgmgpJtGqHwkj7uzRvLn3C_QC62PAd5gmeH-fdQN-lpg1W8ObYaaEuO7Ftwzq_NGnve6C23VqRwAB0f7r6P5EqbNKYcbwv--YdalF3ALJ-h5x0JRrBcZvL0TN-euXDaHbW__bWiv7w0c_o26a9d_8dNkD5uyCCh9g5Hjf-ylWYDqjkXzwmM" width="250" height = "300" align="right">

This dataset was collected programmatically from [PokéAPI](https://pokeapi.co), which provides public REST access to Pokémon game data. The dataset includes all known base Pokémon from Generation I (Kanto) through Generation IX (Paldea), for a total of 1,025 Pokémon.
It contains the following: 

**ID** – The official Pokédex number.\
**Name** – The Pokémon’s English name.\
**Types** – All elemental types associated with the Pokémon (e.g., “Fire”, “Water”).\
**Document** – An English Pokédex entry retrieved from PokéAPI.\
**Filename** – The name of the text file in the data folder where the description is stored.\
**Tokens** - The cleaned text seperated per word.\
**Lemmas** - The tokenized text reduced to their 'roots', their dictionary form.\
**POS (with explanation)** - Fine-grained parts of speech for each token, with human-readable descriptions of the grammatical role. \
**Proper Nouns** - Tokens identified as proper nouns by SpaCy (e.g., names or capitalized terms).<sup> * </sup>\
**Named Entities** – Automatically identified entities (e.g., names, locations, biological terms) extracted using SpaCy’s NER model. <sup>*</sup> 

$^*$ <sup> Some Pokémon descriptions may not have any proper nouns or named entities because they describe fictional creatures and places, so SpaCy finds nothing to annotate. </sup> 

The corpus is made during an exercise carried out for the course Collecting Data in the masters’ program at the University of Groningen. It is intended for use in linguistic analysis and educational purposes. 

Each Pokémon description is also saved as a separate .txt file inside the data/ directory for ease of inspection and later processing. The dataset was created automatically by a Python script that queried the PokéAPI for each Pokémon and exported the results into CSV format. 

Tools used:

* Python
* requests for API access
* pandas for data handling and CSV export
* spaCy for text preprocessing and linguistic annotation

All Pokémon names and descriptions are property of their respective copyright holders. Data was accessed legally via the public PokéAPI under fair use for research and educational purposes.\
<sub>Author: Lise Feringa</sub>

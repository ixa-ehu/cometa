## CoMeta: A Corpus for Metaphor Detection in Spanish

We present CoMeta, a manually annotated **Co**rpus for **Meta**phor Detection in Spanish with the aim of facilitating research on automatic metaphor detection. We believe that CoMeta is the largest publicly available dataset with metaphorical annotations in texts of general domain for the Spanish language.

CoMeta is comprised of miscellaneous texts in Spanish, a subset of 1925 sentences of news domain from the [AnCora dataset](https://github.com/UniversalDependencies/UD_Spanish-AnCora) (Talué et al. 2008); 937 sentences of wiki, blogs, reviews texts from the [GSD corpus](https://github.com/UniversalDependencies/UD_Spanish-GSD); and a total of 771 sentences from manually collected transcriptions of political discourse, from both the [Spanish Government](https://www.lamoncloa.gob.es/consejodeministros/ruedas/Paginas/index.aspx) and parliamentary sessions of the [Basque Government](https://www.ixa.eus/node/13077).


### CoMeta Description 

The annotation of CoMeta has been developed by following the MIPVU guidelines (Steen et al. 2010) used to label
the most popular metaphor corpus for English: the [VUAM corpus](http://www.vismet.org/metcor/documentation/home.html). 

These instructions can be summarized as follows:

1. Read the entire text–discourse to establish a general understanding of the meaning.
3. Determine the lexical units in the text–discourse

3. (a) For each lexical unit in the text, establish its meaning in context, that is, how it applies to an entity, relation, or attribute in the situation evoked by the text (contextual meaning). Take into account what comes before and after the lexical unit.
   (b) For each lexical unit, determine if it has a more basic contemporary meaning in other contexts than the one in the given context. For our purposes, basic      meanings tend to be
      * More concrete; what they evoke is easier to imagine, see, hear, feel, smell, and taste.
      * Related to bodily action.
       * More precise (as opposed to vague).
      * Historically older. Basic meanings are not necessarily the most frequent meanings of the lexical unit.
   (c) If the lexical unit has a more basic current–contemporary meaning in other con- texts than the given context, decide whether the contextual meaning contrasts with the basic meaning but can be understood in comparison with it.
   
4. If yes, mark the lexical unit as metaphorical.

The annotations were performed at token level only for words with semantic content, that is verbs, nouns, adjectives and adverbs. 

CoMeta consists of a total number of 3633 sentences with annotations at token level and binary tagging (B-METAPHOR/O). Only words with semantic content were candidates for the labelling, that includes verbs, nouns, adjectives and adverbs. Due to the subjectivity of the annotations process, the dataset is susceptible of continuous updates, as well as open to improvements.


### Datasets

The dataset is publicly available: [Download Cometa Dataset](https://github.com/ixa-ehu/cometa/blob/main/dataset.zip)

### Metaphor Detection Results

We leverage CoMeta to fine-tune XLM-RoBERTa. We believe that the close performance achieved in comparison to the results obtained with the
larger English VUA dataset are quite promising and encouraging for future researchers interested in using CoMeta or in developing their own
corpora for their languages of interest.

### References

* Sánchez-Bayona, Elisa. (2021). *Detection of Everyday Metaphor in Spanish: Annotation and Evaluation*, Language Analysis and Processing Master's Thesis, University of the Basque Country (UPV/EHU), 2021. [PDF](https://github.com/ixa-ehu/cometa/blob/main/Sanchez-Bayona_MasterThesis.pdf)

* Steen, Gerard & Dorst, Lettie & Herrmann, J. & Kaal, Anna & Krennmayr, Tina & Pasma, Trijntje. (2010). *A method for linguistic metaphor identification: From MIP to MIPVU*. 

* Taulé, M., M.A. Martí, M. Recasens (2008) 'Ancora: Multilevel Annotated Corpora for Catalan and Spanish', Proceedings of 6th International Conference on Language Resources and Evaluation. Marrakesh (Morocco).


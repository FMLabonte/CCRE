# CCRE
# CCEE_for_GRNs
In this repository we provide the CCEE dataset. Matched data, annotaion guidlines, and base data. 
# Notes
Since some updates to naiming conventions were updated during analysis to group labls more effectively and make them more clearly distinct from one another the baseline annotation data still uses those, as does the guidline. We will update the guidline with a revised version with fixed labels. Furthermore for the analysis performed in the paper did ignore the information we captured in () in the annotations with the exception of the mut label. We plan to analyse it in the future, the revised guidlines will therfore exclude these sub labels. 

## A text descriptions of the abels and changes that were made can be found here: 
Annotated for
 ### Instructions for filling the gene/disease interactions table:
#### Gene_Protein
 For the annotation of genes or proteins that were mentioned in the papers either as being related to a specific cancer or connected to another gene, annotators were instructed to note down genes that are connected to one of the above mentioned categories. There were additional labels added: “fam” to denote if the text talked about a gene family, “path” if it was a pathway or “mut” if the gene was described as mutated. Furthermore, the signifiers “(G)” or “(P)” were used to clarify if the text talked about a gene or a protein since the names can be the same.
#### Disease
 The annotation of diseases followed a slightly different strategy. Since the only disease examined here was cancer, the signifiers “(cancer name)(cancer type)” were used to give further details, unless the category was unknown, in which case “(NA)“ was added. The cancer type label options were the following: “carcinoma”, “sarcoma”, “lymphoma”, “leukemia” or “myeloma”.
#### Treatment_Exposure
 Apart from the genes and cancer types, treatments or exposure were annotated as well. If there was a treatment mentioned, it and its connection to the gene were included.
#### Connection_Disease
 There were several labels for the connection to the disease. The identifier “connected” only marked that there was some sort of relationship between the gene and the disease without further description of the specific interaction. “Key gene” was initially used to describe if the gene was clearly stated to be a key gene or if the text overtly portrayed the gene as a key player in the interaction. Nevertheless, this denominator turned out to be too undefined and effectively useless, since it always appeared in conjunction, which is why it was dropped.
#### connection_disease_marker
 The signifier “marker” was supposed to express if something was utilised as a marker gene, however, after the first analysis it was determined that it should be moved to its own category.
#### Disease_Mechanism
 If the gene or protein actively makes the disease worse, firstly the label “driver” was added, later it was changed to “progression”. On the other hand, “suppressor”, renamed to “suppression” was used if the gene or protein directly counteracts the disease, or aspects of it. While these label changes appear confusing at first, for future analyses only the new names will be used.
#### Connection_Treatment
 For the description of the connection to the treatment, similarly to the connection to the disease, annotators were asked to use “connected” if there was no specific interaction described but there was a clear relationship between the gene or protein and treatment.
#### treatment_mechanism_type
 Originally, the word “target” was used if the treatment specifically targets the gene or protein in question, but it was moved to its own category called “mechanism type”. The label was replaced with “connected”. Additionally, the initial categories “activator” and “suppressor” were renamed to “activator” and “inhibitor”, to more accurately represent their function. If the connection was indirect, the label “(ind)” was attached.
#### Disease_Mechanism
 The mechanisms tied to the connection between the genes and diseases, as well as the mechanisms attached to the connection between genes and treatments were annotated as well. Examples of categories are listed above.
#### Associated_Factors
 If there was information on other contexts or more in-depth descriptions that did not fit into any other category, the bracket “associated factors” was included.
#### Cellline
 The cell line in which the connection between the gene and other entities was detailed could be added in the “cellline” category. If there was no exact cell line given, this section was used to give further general information on the cell or specimen.
#### Species
 Annotators included a categorisation of the species that was being studied, as well as the tissue in which the connection was observed. If there was no specific tissue, either the organ was named or “NA”, if no other information on it was available. In this section additional information on whether or not metastases were mentioned was included. Furthermore, if the organ of the metastases was known, it was also named.
#### Confidence
 There were three levels of confidence regarding the given information: “low”, “medium” and “high”. “Low” was used if there was no source or no experimental data and low certainty language was present. The signifier “medium” described if there was a source or experimental data, but still uncertain language. However, “medium” could also be used if there was certain language but no source. Lastly, the label “high” marked that the text had a source or experimental data in addition to high certainty language.
#### Type_of_Evidence
 For the description of the type of evidence, again three labels were used. “Direct” represented information gathered through intervention, most often either in vivo or in vitro. In contrast, the descriptor “indirect” meant that the interaction was observed but without any intervention or immediate interaction, such as inferrals or logical assumptions based on the given evidence. The third label, “citation” denotes no specific type of evidence and that the text instead refers to a different study.
#### Sentence
 The entire document was numbered by sentences and the category “sentence” was used to record which exact sentence the interaction was mentioned. Oftentimes, multiple sentences were included.

Annotated for
 ### Instructions for filling the gene/gene interactions table:
#### Gene_Protein
 Annotators were asked to name the gene or protein for which a connection to a different gene or protein was described. The additional label “(G)” was added if it was stated to be a gene, “(P)” if it was a protein. If the gene or protein had a mutation, the modifier “(mut)” was included. Similarly, the gene or protein connected to the previous gene or protein was labelled with “(G)” or “(P)” and the optional modifier of “(mut)” as well.
#### Connection_Type
 Afterwards, the connection type was identified. Using the marker “activator” meant that a positive regulation between the genes and/or proteins was found. If the opposite was the case and a negative regulation was observed, “inhibitor” was noted. If the gene or inhibitor was co-regulating the gene in combination with another gene or protein, the label “(co)” was added. Additionally, annotators included “(ind)” if the gene was connected in the regulation process in some way but it was not clear whether the gene itself or one of its downstream targets was involved.
#### Connection_Type
 If an activation or inhibition was not mentioned in the text, a few other options were noted. Firstly, “connected” signified that there is a relationship between the gene(s) and/or protein(s), but no specifications were made in the text. Furthermore, if the gene was involved in the regulation process but it was unclear whether itself or one of its downstream targets were involved, “(ind)” was added. Initially, the labels “binding” for a gene or protein that binds to the connected gene or protein, and “target” for a gene or protein that targets the connected gene or protein were introduced, but these were later combined since they were functionally the same and the differentiation proved to be too subtle in practice.
#### Regulation_Level
 To differentiate at what level the regulation took place, several label options were provided. The marker “epigenetic” signified that the regulation took place through methylation and other changes to the DNA and histones that change DNA folding. If instead “transcription” was added, the text described the regulation happening in the process of producing mRNA. For different splicing patterns that change the mRNA, “splicing” was used. If the regulation occurred through longevity and the state of the mRNA, annotators noted “mRNA(L)”. For regulation activities taking place during the process of producing a protein from mRNA, the label “translation(L)” was used. The signifier “protein(L)” denotes if the regulation happened through stability and the state of the protein. If a different method is mentioned, “other” was stated. If localisation was mentioned in the context of regulation, an “(L)” was added as well.
#### Disease
 The next category concerned itself with labelling disease connections. Again, the format “(cancer name)(cancer type)” was used to give sufficient detail, unless there was no category mentioned, in which case “NA” sufficed. The suggested labels were: “carcinoma”, “sarcoma”, “lymphoma”, “leukemia” and “myeloma”.
#### Treatment_Exposure
 If there were mentions of a treatment, it and its connection to the gene were added as well.
#### Associated_Factors
 Contexts and information that was not fitting into any other categories were noted in “associated factors”.
#### Cellline
 The cell line in which the connection between the gene and other entities was detailed could be added in the “cellline” category. If there was no exact cell line given, this section was used to give further general information on the cell or specimen.
#### Species
 Information on the species that was being studied was included, as well as the specific tissue that the connection was observed within. If the text only gave the organ, it was put in this bracket, or “NA” if no further information was available. If metastases were referenced in the study, “metastases” was added.
#### Confidence
 As with the gene/disease interactions, a level of confidence was estimated. The label “low” meant that there was no source or no experimental data, as well as low certainty language. “Medium” signified the presence or a source or experimental data while the language used remained uncertain, or certain language but no source. Thirdly, the label “high” denoted that a source or experimental data was present in addition to high certainty language.
#### Type_of_Evidence
 For the description of the type of evidence, again three labels were used. “Direct” represented information gathered through intervention, most often either in vivo or in vitro. In contrast, the descriptor “indirect” meant that the interaction was observed but without any intervention or immediate interaction, such as inferrals or logical assumptions based on the given evidence. The third label, “citation” denotes no specific type of evidence and that the text instead refers to a different study.
#### Sentence
 Lastly, the sentences of each document were numbered to clarify in which exact sentence the information was taken from. In the bracket “sentence” the sentence number was listed, which could include multiple sentences.



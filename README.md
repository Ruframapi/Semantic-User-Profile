# Semantic-User-Profile
Dataset for semantic modeling strategies evaluation.

## Description

This dataset contains the user profiles of 11 professors in the area of computer science. It was  built from some of the most recent publications found on their Google Scholar web pages. 

Number of publications used to build the profiles: At least  twelve for each professor.
Candidate Set: 5710 different academic documents recovered from Core (https://core.ac.uk/) and Arxiv (https://arxiv.org/) open corpora.

In order to find resources annotations mentions, DBpedia Spotlight service (English and Spanish) with a JAVA heap memory of 16GB was employed.

## Tables

* gs_user: User scholar info and identifiers.
* gs_publications: User's publications info.
* ex_document: DBpedia annotations in user's publications (full text, title and abstract). The final column indicates the language of the document (1 English, 2 Spanish, 3 Others).
* re_core, re_arxiv: Candidate set. Inside of each table the publications identifiers in Arxiv and Core services are found.  The column "repetido" indicates documents with a different id (Arxiv or Core) but which refers to a document already present in the candidate set.
* ex_re_arxiv, ex_re_core: Candidate set DBpedia annotations (full text, title and abstract).
* user_selected_publications: Ground truth. Subset of the candidate set in which the user expresses an explicit interest.

## Folders

Folder Modeling Meta contains titles and abstracts of user's publications. The file name starts with the database identifier. 




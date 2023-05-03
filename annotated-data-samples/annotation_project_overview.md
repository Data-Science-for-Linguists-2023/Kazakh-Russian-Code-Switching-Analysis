# Annotation Project Overview 

If you are interested in code-switching (CS) between two languages and would like to delve into linguistic features of it, here you can find the main stages of my project and step-by-step explanation of annotation process I did.  


## Summary 

This term project aimed to carry out an explanatory analysis of Kazakh-Russian CS based on the conversational dataset and investigate structural and syntactic types of CS through **linguistic annotation**. The questions in focus were whether Kazakh-Russian bilingualism is balanced and whether the language shift is happening toward L2 Russian.


### Literature Review 

First of all, you will start with the literature search on syntactic and morphological annotation types and structure, also look at research related to computational approach to code-switching. The main literature for the linguistic annotation written by Ide & Pustejovsky (2017). This is a sizable work and I recommend briefly skimming the section [Designing Annotation Schemes: From Model to Representation](https://link.springer.com/chapter/10.1007/978-94-024-0881-2_3) to get sense of annotation types and workflow. As for the code-switching research, it will depend on your choice of languages and there is plenty of empirical research that has been done in this field. A good venue to start with is [Special Issue "Interdisciplinary Approaches to Data Collection, Annotation and Computational Processing of Code-Switched Languages around the World"] (https://www.mdpi.com/journal/languages/special_issues/Computational_Codeswitching). Here you can find diverse body of research related to code-switching and annotation. If you are also interested in Kazakh-Russian code-switching, you can look at the study done by [Dyachkov et al.(2020)](https://www.dialog-21.ru/media/5085/dyachkovvvplusetal-101.pdf) who annotated and analyzed CS in four corpora of minority languages of Russia. This work served as the main framework for the current project and I was able to mostly replicate the analysis done by authors except for metrics based on the word-by-word language annotation. 


### Data

Again, your data sourcing would also depend on the languages in focus. For the current project, I used the the [IARPA Babel Program Kazakh language collection](https://catalog.ldc.upenn.edu/LDC2018S13) released by Linguistic Data Consortium at UPen. You can access this dataset via the university's LDC account and to do that you have to ask the course instructors. After authorizing access, you can purchase the pack for $25 which allows you to download the whole data package. However, you can use this project only for the Pitt related coursework and cannot fully share the original data samples. On the other hand, if you are interested in code-switching in other languages, common search engines is a good old way to start. Also, remember consulting with your course instructors as they are more knowledgeable on this matter and can point you in the right direction. 

### Annotation tools 

For annotation, I used the [Labelbox platform](https://docs.labelbox.com/docs/overview). The Labelbox platform offers a standoff annotation (offline) format where annotations are stored separately from the annotated text which can be retrieved via the API key. For the project in focus, the annotation workflow looks like this:

![Annotation workflow](screenshots/annotation-workflow.png)

First, you create a dataset and upload text files for annotation; then, you need to create an ontology known as an [annotation scheme](https://github.com/Data-Science-for-Linguists-2023/Kazakh-Russian-Code-Switching-Analysis/blob/main/annotated-data-samples/annotation_scheme_1st_draft.md); and finally, you generate a project where text samples can be annotated using the ontology. The annotation process looks like [this](https://labelbox.com/product/annotate/text/).

The project overview on the Labelbox platform will look like this:

![The project overview](/screenshots/labeling-progress.png)

**Labeling progress:** This section provides a list of all statuses in a project and a count of data rows for each. It also provides a count of the issues. As can be seen from the picture, 13 annotations were done, and 1 file is waiting to be annotated.

**Workflow tasks:** This lists all the tasks in the project including the Initial labeling task, Rework task, and all review steps. 

Also, in the project overview, the **annotation analytics** can be viewed, and you can see what tags and subtags are more common than others. I found this feature very helpful because you can get a sense of your data even in the early stage of your project.

![Analytics view](/screenshots/annotation-analytics.png)

For each feature, you can see the following:

- Name of the tag;
- Count of data rows that contain the tag;
- %Share indicating the percentage of data rows that contain the tag;
- Horizontal bar chart that depicts the share and also allows you to click through into a filtered view of the data rows tab that contains only the data rows that contain the relevant feature.

Overall, the platform website has plenty of tutorials and guidelines that easy to follow and create your own annotation project. You can learn more about Labelbox features [here](https://docs.labelbox.com/docs/overview). Worth to mention that the Labelbox platform's support team is also very responsive and can help you out if you have any issues. For instance, I had problems with retrieving the text samples in Cyrillic and reached out to the support team via their email. To my big surprise, they replied very quickly and walked me through the proper text retrieval process. 

### Analysis

The Labelbox platform renders output as a JSON file so you need to properly parse the file in order to extract annotated samples. In [this notebook](https://nbviewer.org/github/Data-Science-for-Linguists-2023/Kazakh-Russian-Code-Switching-Analysis/blob/be7a7094bc6ef79c342b349b0674fc5f9cba458b/notebooks/annotationAnalysis.ipynb#Parsing-JSON-files) you can find methods I used to parse the highly nested JSON file. In [this notebook](https://nbviewer.org/github/Data-Science-for-Linguists-2023/Kazakh-Russian-Code-Switching-Analysis/blob/main/notebooks/annotatedDataset.ipynb), first, I worked with a small sample (2 annotated files) to get to know the data and then uploaded and analyzed the bigger sample. Detailed comments and observations on the dataset can be found throughout the notebook. Final analysis and visualization can be found [here](https://nbviewer.org/github/Data-Science-for-Linguists-2023/Kazakh-Russian-Code-Switching-Analysis/blob/be7a7094bc6ef79c342b349b0674fc5f9cba458b/notebooks/annotationAnalysis.ipynb#Analysis-&-Vizualization).
 



	








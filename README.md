**Raw data for the paper** 

Zbigniew Koza (UWr), Robert Lew (UAM), Emanuel Kulczycki (UAM), Piotr Stec (UO)

*How the national academic promotion system is controlled by old boys: An analysis of power distribution in Poland*
Wrocław-Poznań-Opole, 2022.


The repository contains the follwing files:

- **raw_data.csv** - contains the raw data as read by OCR software from CK documents. Contains the following fields:   
  - `first name(s)`  - empty for some cases where the url is unknown (the documents were removed from the CK server after we had first retrieved them)	
  - `family name`    - may contain concatenated first and familiy names if the previous field is empty 
  - `academic field` - in Polish, see the dictionary	
  - `academic discipline` - in Polish, see the dictionary
  - `application number` - internal number used by CK to identify applications
  - `application type` - 'P' for proffesorship, 'H' for habilitation
  - `CK section` - CK was divided into 7 sections, roughly corresponding to 7 large fields of science  
  - `url` - url where the application-related documents can be found
  - `CK decision url` - url where the CK decision (a PDF scan) on the habilitation/professorship committee/referee panel can be found; the primary data source for our study
  - `referee 1`	- name of the 1st referee
  - `referee 2`	- name of the 2nd referee
  - `referee 3`	- name of the 3rd referee
  - `referee 4`	- name of the 4th referee, only for proffesorship applications
  - `referee 5`	- name of the 5th referee, only for proffesorship applications
  - `Chair`	- Chair of te habilitation committee
  - `Secretary`	- Secretary of the habilitation committee
  - `Member`	- 1st member of the habilitation committee
  - `Member`	- 2nd member of the habilitation committee
  - `year` - year when the decision was issued by CK
- **fields_PL-EN_dictionary.csv** - a Polish-English dictionary of scientific field names
- **disciplines_PL-EN_dictionary.csv** - a Polish-English dictionary of scientific discipline names
- **ck_members.csv** - a list of CK members in 2011-2020, with the terms of office, scientific specialisations and affiliations. Here 0 stands for "No", 1 - for "Yes".

**Data format**

All data are in the CSV (comma-separated values) format. 

They can be read as ordinary text or as spreadsheets in LibreOffice, MS Excel, etc.

- Character encoding: UTF-8 (mostly for the Polish language characters)  
- Column separator: comma (,)

**Caveat and disclaimer**

The tables contain information read from documents stored for public acces in the official CK server, https://www.ck.gov.pl/. The data was retrieved through automatic conversion of CK documents from the PDF (raster) format into plain text files using free OCR software. This implies that they can contain spelling errors in names, assignments to disciplines, years, etc. There is thus no firm connection between names in our tables and any real persons: the data do not allow for distinguishing persons with the same first and family names; nor do they contain any information about changes in names (e.g. following a marriage), and both first and family names might have been corrupted by CK staff or our software. With this in mind, our data represent only sequences  of characters (strings), not real persons. Any attemt to apply them to persons requires (presumably manual) verifcation in the original sources. 

We have made every effort to ensure that the data, especially those even indirectly related to personal data, are as close to the actual state as possible, but due to the way they were obtained, we do not guarantee their 100% accuracy. Any departures from the facts are unintentional. 

The data on CK mebership are incomplete in that they do not take into account that they might have slightly evolved in time (stepping down from the office, etc.). Our data show "snapshots" of the memberships in some points of time, for which a reliable source of data could be found. 

During document processing, we took into account only the original decisions on the referee panels / habilitation committees. We did not considered any changes in membersips of these bodies.


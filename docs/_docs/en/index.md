---
title: About ABCD
permalink: /docs/en/
key: docs-quick-start
---


## General introduction to ABCD as a software suite

ABCD is the acronym for a software suite for the automation of libraries and documentation centres. In Spanish this is, in full : ‘**A**utomatisación de **B**ibliotécas y **C**entros de **D**ocumentación’, which keeps the same acronym valid also for French (**A**utomation des **B**ibliothèques et **C**entres de **D**ocumentacion) or Portugese (**A**utomatização das **B**ibliotecas e dos **C**entros de **D**ocumentação). Even in other non-latin languages, with some slight but quite acceptable variations, - e.g. Dutch : ‘**A**utomatisering van **B**ibliotheken en **C**entra voor **D**ocumentatie’ - the acronym can still be maintained.

The name itself already expresses the ambition of the software suite : not only providing automation functions for the ‘classic’ libraries but also other information providers such as documentation centres. Flexibility and versatility are at the forefront of the criteria on which the software is developed. This flexibility e.g. is illustrated by the fact that in principle, but also practically, any bibliographic structure can be managed by the software, or even created by itself. Even non-bibliographic structures can be created, as long as the information is mainly ‘textual’ information, as this is the limitation put by the underlying database technology, which is the (CDS/)ISIS textual database. Good understanding of some basic ISIS-related concepts and techniques, e.g. the Formatting Language, is crucial for full mastering of the ABCD-software. For this reason some sections of this Manual will also deal with the underlying ISIS-technology.

ABCD is called a ‘suite’ of softwares for library and documentation centres automation because it exists of some relatively independent modules, which can fully co-operate but also can exist without each other. In fact some existing advanced softwares, mostly having already shown their potential in demanding environments in BIREME- applications (within the Virtual Health Library context), were adopted and adapted into ABCD - that is why the original names such as iAH, SeCS (both developed by BIREME) and EmpWeb (Empréstimos en Web) developed originally by KALIO ltda. of Uruguay and amply tested in Valparaiso at the University) are maintained. These main parts are shown, with their hierarchical relationships, at the second level in the following picture and subsequently discussed briefly :

![Slide2](https://user-images.githubusercontent.com/20482054/137317883-75797ad3-47d5-43f0-b3b7-7c405f646236.JPG)

### The ABCD Central

The ‘Central’ module of ABCD comprises modules for Database Administration (creation of databases, edit- ing of database-structures, database utilities), Cataloging, Acquisitions, Circulation/Loans and Statistics. A thesaurus management module is also being prepared as part of the cataloging module for a specific the- saurus-structure database with consistency control of the hierarchical levels. As part of this ‘central module’ we would also like to mention import- and export services, printing and database-tools like blocking/unblocking and ‘global changes’ to fields in records. This ‘Central’ part in fact represents the ‘back-office’ part of ABCD, end-users will not be confronted with this but what they will see and be offered is fully defined in this central management part of the software !

Any ISIS-database structure can be defined and managed, with currently records of 1Mb maximum size and 4Gb max, databases (but these restrictions will be made obsolete by the NBP-based next generation of ISIS and ABCD). As compared to ‘normal’ ISIS-technology ,60-character (as compared to 30-character) indexing keys are used, there are much stronger authority control features available (picklists based on tables or authority databases such as thesauri) at the data-entry stage with flexible validation formats) and all interaction is based on WWW-technology of course, allowing e.g. HTML-coded text-strings for full-text indexing, hyperlinks to help-pages etc.

It is perfectly possible to fully automate a smaller library with mostly internal users with all necessary functions, only using this Central part, as e.g. an advanced searching option is built-in, so that all functions are covered with a minimum of technological complexity (i.e. only ISIS and PHP).

### The ABCD OPAC (iAH)

The public search interface (OPAC) is an adapted version of BIREME’s general ‘advanced interface for Health information’ (iAH). It allows meta-searches on not only the local catalogs but also many other information resources.

The iAH interface developed by BIREME is currently being upgraded to iAHx, ensuring it will align perfectly with modern Information Retrieval concepts and techniques (e.g. clustering, relevance ranking based on Lucene indexing).

### The ABCD Site

The search function is offered as part of an ‘end-users’ portal page, presenting the own catalog(s) in a much wider information context by providing access to other information resource.s (e.g. Google, Medline…) and communication (announcements, alerts), also paving the way for ‘Web 2.0’-like functions.

The Site Administrator actually is a specific Content Management System which allows designing the structure and components of the portal page of ABCD.

### The ABCD Serials Control System (SeCS)

This module offers an advanced management tool for serials/journals (classical and/or electronic) of any pub- lication type (referring to periodicity). Serials as such but also issues of a serial and all types of publication patterns can be managed by this module. BIREME uses this technology e.g. for its products ‘Portal of Scientific Journals’ (see :  [http://portal.revistas.bvs.br/main.php?home=true&lang=en)](http://portal.revistas.bvs.br/main.php?home=true&lang=en)) and SCAD (see : http://scad.bvs.br/php/index.php?lang=en) which is the Brazilian union catalog of over 12.000 journals (with millions of issues) of more than 50 libraries.

### The ABCD Advanced Loans module (EmpWeb)

This module offers advanced loans management with some more extra features for larger and more complex organisations. It offers a ‘MyLibrary’ function to end-users through the OPAC and is based on ‘web-services’ technology. It can be used to replace the integrated loans module of ABCD in case of a need to cope with multi-branch/policy and very high transactions volume situations.

The ‘suite’ idea reflects the fact that ABCD has relatively independent parts - as is the case with office automation suites (e.g. Open Office, Microsoft Office) - but with obvious links to co-operate. The Statistics module e.g., as part of the Circulation/Loans module, can work on any ISIS-database, while the iAH-OPAC also can offer advanced web-based retrieval in any (set of) ISIS-databases, not only ABCD-maintained ones. The Serials Control System (SeCS) manages ISIS-databases for serials within or outside the ABCD-context. But together, we believe, these parts constitute a very powerful suite of tools, and as an integrated part we hope ‘the sum is more than just the parts added up’ !ry powerful 'suite' of tools 
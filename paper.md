---
title: 'Enhancing Digital Infrastructures and Data Handling Practices for Single Specimen Barcoding \- the 2024 BGE Barcoding Hackathon'
tags:
  - DNA barcoding
  - Bioinformatics workflows
  - FAIR data publishing
  - Data integration
  - Data curation
  - Biodiversity Genomics Europe (BGE)
authors:
  - name: Rutger Vos (RAV)
    orcid: 0000-0001-9254-7318
    affiliation:
      - 1
      - 2
  - name: Kessy Abarenkov (KA)
    orcid: 0000-0001-5526-4845
    affiliation: 3
  - name: Jireh Agda (JIA)
    orcid: 0009-0004-5235-9610
    affiliation: 4
  - name: Josh Agda (JOA)
    affiliation: 4
  - name: Ruud Altenburg (RA)
    affiliation: 1
  - name: Sarah J. Bourlat (SJB)
    orcid: 0000-0003-0218-0298
    affiliation: 5
  - name: Thomas Brown (TFB)
    orcid: 0000-0001-8293-4816
    affiliation:
      - 6
      - 7
  - name: Eli Chadwick (EC)
    orcid: 0000-0002-0035-6475
    affiliation: 8
  - name: Pierre-Etienne Cholley (PEC)
    affiliation: 1
  - name: Fabian Deister (FD)
    orcid: 0000-0002-3172-3223
    affiliation: 9
  - name: Dick Groenenberg (DG)
    affiliation: 1
  - name: Sharif Islam (SI)
    orcid: 0000-0001-8050-0299
    affiliation: 1
  - name: Nick Juty (NJ)
    orcid: 0000-0002-2036-8350
    affiliation: 8
  - name: Vishnukumar Balavenkataraman Kadhirvelu (VBK)
    orcid: 0000-0001-9845-2547
    affiliation: 10
  - name: Maria Kamouyiaros (MK)
    orcid: 0000-0002-5953-6251
    affiliation: 11
  - name: Douglas Lowe (DL)
    orcid: 0000-0002-1248-3594
    affiliation: 8
  - name: Hana Merchant (HM)
    orcid: 0000-0003-1373-8808
    affiliation: 11
  - name: Joana Pauperio (JP)
    orcid: 0000-0003-2569-0768
    affiliation: 10
  - name: Ben Price (BP)
    orcid: 0000-0001-5497-4087
    affiliation: 11
  - name: Sujeevan Ratnasingham (SR)
    orcid: 0000-0002-3694-0171
    affiliation: 4
  - name: Stian Soiland-Reyes (SSR)
    orcid: 0000-0001-9842-9718
    affiliation: 8
  - name: Giorgia Staffoni (GS)
    orcid: 0009-0003-5916-1757
    affiliation: 12
  - name: Catherine Wei (CW)
    affiliation: 4
  - name: Oliver White (OW)
    orcid: 0000-0001-6444-0310
    affiliation: 11
  - name: Dimitris Koureas (DK)
    orcid: 0000-0002-4842-6487
    affiliation: 1

affiliations:
  - name: Naturalis Biodiversity Center, Leiden, The Netherlands
    index: 1
  - name: Institute of Biology Leiden, Leiden University, Leiden, The Netherlands 
    index: 2 
  - name: Natural History Museum, University of Tartu, Tartu, Estonia
    index: 3 
  - name: Centre for Biodiversity Genomics, Guelph, Canada
    index: 4 
  - name: Leibniz Institute for the Analysis of Biodiversity Change, Museum Koenig, Bonn, Germany
    index: 5 
  - name: Leibniz Institute for Zoo and Wildlife Research, Berlin, Germany 
    index: 6 
  - name: Berlin Center for Genomics in Biodiversity Research, Berlin, Germany
    index: 7 
  - name: The University of Manchester, Manchester, UK 
    index: 8 
  - name: Zoologische Staatssammlung München, Munich, Germany
    index: 9 
  - name: European Molecular Biology Laboratory, European Bioinformatics Institute, Wellcome Genome Campus, Hinxton, UK
    index: 10 
  - name: Natural History Museum, London, UK
    index: 11
  - name: Università degli Studi di Firenze, Florence, Italy
    index: 12
date: 2024
bibliography: paper.bib
authors_short: Vos et al. (2024) BGE Barcoding Hackathon 
group: BGE
event: BGE Barcoding Hackathon
---

## Abstract

The 2024 BGE Barcoding Hackathon, hosted by the Biodiversity Genomics Europe (BGE) project in Leiden, Netherlands, focused on advancing digital infrastructures and data handling practices for single specimen barcoding. This event brought together 24 participants from various consortium member institutes to enhance workflows in DNA barcoding, which complements genome sequencing efforts within BGE. The hackathon was structured around four thematic pillars: Data Generation and Processing, BOLD Release Candidate, Wider Data Integration, and Reference Data Curation. Participants worked on optimizing barcode generation pipelines, developing a new version of the Barcode of Life Data Systems (BOLD) data publishing platform, harmonizing data standards for better integration with databases like ENA and UNITE, and automating curation processes for DNA barcoding records. The outcomes include improved workflows, enhanced data interoperability, and refined curation standards, which collectively support BGE's goals of achieving a step change in molecular biodiversity monitoring and research.

# Background

This proceedings paper outlines the collaborative efforts undertaken during a hackathon hosted by Biodiversity Genomics Europe (BGE), a Horizon Europe-funded project with a consortium of 33 institutional partners, represented by 24 selected participants attending the hackathon. Held from April 23-25, 2024, in Leiden, the Netherlands, and coordinated by Naturalis Biodiversity Center, the event focused on the DNA barcoding [@Hebert2003-1] stream of BGE's project structure. This stream is designed to complement a parallel stream dedicated to genome sequencing.

The DNA barcoding stream of BGE involves several interconnected work packages (WPs) aimed at enhancing the collection, sampling, sequencing, publishing, and curation of barcoding data for undersequenced taxa. The effort begins with sampling in WP4, where project partners gather specimens from the field and existing museum collections, based on a gap list developed at the Zoologische Staatssammlung München (SNSB). The gap list identifies taxa lacking COI-5P barcode sequences by cross-referencing curated taxonomies with the Barcode of Life Data System (BOLD, [@Ratnasingham2007-2]).

In WP6, the sequencing workflow diverges based on the specimen type. Assembled barcode sequences from fresh specimens are generated at UNIFI in Florence, where sequencing is performed using the PacBio Sequel platform. Museum specimens are processed by genome skimming [@Straub2012-3] of the mitogenome at the Natural History Museum (NHM) in London or at Naturalis, in Leiden, which respectively perform DNA extractions and library preparations of samples sent to them. These libraries are then forwarded to SciLifeLab in Uppsala for whole genome sequencing (WGS) on the Illumina platform.

WP8 handles quality verification and BOLD submissions and oversees the transformation of BOLD into a more decentralized, read-only data publishing platform. BOLD is currently on its fifth major version of the data system. This WP also aims to improve data integration with other relevant databases, particularly the European Nucleotide Archive (ENA, [@Harrison2021-11]) and UNITE [@Abarenkov2024-5], focusing on richer metadata exchange and semantic agreement between these repositories.

WP10 focuses on the curation of BOLD data, integrating new DNA barcodes with previously published records into reference libraries. This curation process includes automated checks for the presence and value of various metadata fields and assessment of species correspondences with Barcode Index Numbers (BINs [@Ratnasingham2013-6]). Despite automated processes, manual verification by taxonomic experts is crucial due to potential issues like incomplete lineage sorting, hybridization, cryptic species, and data errors like off-target amplification and misidentifications.

This hackathon was structured around four thematic pillars: Data Generation and Processing, the latest BOLD Release Candidate, Wider Data Integration, and Reference Data Curation. These themes facilitated focused discussions and activities aimed at aligning efforts, coordinating development, and enhancing communication beyond recurrent video calls across the consortium, and allowed concerted effort on identified priorities over an extended duration. The detailed scope of these themes, their activities during the hackathon, and subsequent actions will be elaborated upon in the following sections of this paper.

# Thematic pillars

## Data generation and processing

This theme within the hackathon addressed bioinformatics aspects of barcode generation and the processing of genomic data. The primary focus was on the generation of fresh barcodes at UNIFI and on refining the genome skimming processes at NHM and Naturalis. This theme is integral to BGE's Work Package 6 (WP6), which encompasses the technical and procedural frameworks for DNA barcode generation.

A central component of this theme’s activities was the genome skimming pipeline developed at NHM. This pipeline, which is hosted publicly on GitHub[^1], is implemented using Snakemake—a workflow management system that enables reproducible and scalable genomic analyses. The pipeline incorporates Python programming and various dependencies that are managed through Conda, providing a reproducible and portable environment for data processing. The hackathon resulted in several improvements to the pipeline, including the streamlining of input requirements, the identification and removal of minor issues, simplification of the pipeline deployment through the removal of singularity dependencies, improved readability of code using Snakemake checkpoints, and improvement of the output summary with MultiQC[^2]. 

Efforts were also made to enhance the provenance tracking capabilities of the Snakemake workflows. The team worked on integrating reporting facilities that could output Research Object Crate (RO-Crate [@Soiland-Reyes2022-7]) run profiles, facilitating better documentation and reproducibility of genomic workflows. This development is also available on GitHub[^3]. Lastly, the hackathon resulted in the pipeline's submission to WorkflowHub[^4] [@Silva2020-8], where an RO-Crate detailing the pipeline's configuration and usage is generated.

The application of the genome skimming pipeline at both NHM and Naturalis has demonstrated success, processing reads from various collection specimens to produce mitochondrial genomes and COI-5P barcode sequences. Concurrently, progress was made in standardizing the quality assurance (QA) processes for barcodes prior to their submission to BOLD. This standardization includes verifying the congruence of barcodes with expected species targets, which necessitates a reliable reference library. The hackathon also explored the use of the CRABS tool[^5] [@Jeunen2023-9] for creating such reference databases as an alternative to homegrown curation systems.

Looking forward, the outcomes of this theme have improved preparedness for the application of the skimming pipeline to tens of thousands of specimens over the coming year, aligning with BGE's project targets. This application will be accompanied by continued enhancement and standardization of QA processes, such that the generated barcodes meet the aims of the project and the requirements necessary for scientific and conservation applications.

## BOLD Release Candidate

The development of version 5 of BOLD represents a significant overhaul in its ecosystem of services, a key focus of the hackathon. This new version marks a departure from the previous architecture by separating the data portal from the submission workbench, which were previously integrated in a single, database-backed web application. This separation addresses the accumulation of legacy debt over the last decade, paving the way for a more scalable, decentralized framework.

The redesigned system is read-only and utilizes a NoSQL database (Couchbase) to manage barcode records, now ingested as JSON-L. The structure of these JSON-L records adheres to the Barcode Core Data Model (BCDM) vocabulary[^6], a developing standard that enhances the semantic consistency and expressive richness of barcode metadata. This shift not only modernizes the BOLD infrastructure but also promotes its integration with other resources.

BOLD v.5 features a services-first approach in its web application, constructed using Python and JavaScript. The application acquires its data through the new, richer web service API[^7], facilitating a more dynamic interaction with the underlying data while in the process providing the impetus for performance improvements in the API. The API’s expansion significantly improves the system’s interoperability, for example by enabling DiSSCo[^8] to fetch specimen data held by BOLD.

During the hackathon, progress was made towards achieving a minimum viable product (MVP) for BOLD v.5. Enhancements included the integration of detailed text content, the application of UI/UX guidelines, and the introduction of new features such as reporting tools for barcoding outputs by institutions, autocomplete functions in search fields, and advanced visualizations of specimen collection localities and summary statistics at the country level. These improvements were supported by performance optimizations at both the database and service layers.

Collaboration was a central feature of the hackathon, with participants from the Centre for Biodiversity Genomics (CBG) and Naturalis working closely together. Their joint efforts facilitated the alignment of development practices, such as through the shared adoption of Tilt, a platform for monitoring services in a Kubernetes cluster, enhancing the development environment. As BOLD v.5 moves forward, CBG is leading a sprint to finalize the MVP, aiming to soon launch a version that will significantly enrich the capabilities and user experience of the BOLD system.

## Wider Data Integration

This theme of the hackathon focused on enhancing the interoperability and connectivity between BOLD, DwC, MIxS, ENA, and UNITE. A central element in this effort was the application of the BCDM to enable harmonizing data formats and metadata standards within BGE. In particular, these terms and data formats are crucial for sample data submission to BOLD and ENA. 

We dealt with a variety of terms across different data models, such as processid, museumid, sampleid (BCDM), materialSampleID (DwC), samp\_name, source\_mat\_id (MIxS). All of these terms are related but also have specific context and semantics attached to them, coming from their respective source domains. A structured mapping approach allows not only the conversion and integration of data but also ensures that information can be accurately and efficiently shared between platforms \- with as much machine readability as possible. This way, each domain/source can maintain their terms but still take advantage of data linking and sharing.

We envision a wider adoption of these terms and the use of mapping files to harmonize data formats and automate the mapping process as much as possible. Initially, we expect the process to involve manual mapping curation and validation. However, the goal is to progressively streamline and automate this process, ensuring consistency and efficiency in data sharing and integration across biodiversity information systems.

At the hackathon, UNITE adopted BCDM in the development of a new web service endpoint, which provides data from UNITE formatted according to the BCDM JSON specification. UNITE’s implementation of this endpoint helps promote the integration of its data with other platforms using the same model. Similarly, ENA has evaluated the alignment of BCDM with the current standards adopted for biodiversity genomics projects under the Tree of Life Checklist[^9], to improve interoperability between the databases and facilitate the deposition of more richly annotated data by the consortium.

A significant portion of the hackathon efforts was devoted to developing mappings between BCDM and other widely used vocabularies. Participants worked on creating interoperable mappings for BCDM to DarwinCore [@Wieczorek2012-10], ENA Tree of Life Checklist [@Harrison2021-11], BGE/iBOL-internal terminology, UNITE [@Abarenkov2024-5], and MIxS [@Yilmaz2011-12], facilitating data sharing and integration across diverse biological data systems. These mappings, and a Java implementation that produces document transformations, are documented and accessible for further development and use by the broader community[^10].

During the hackathon, we utilized the Simple Standard for Sharing Ontological Mappings (SSSOM) to create the mappings between different data models. For instance, starting with a manually curated TSV file containing two columns of terms from BCDM and UNITE, we enhanced this file by incorporating essential SSSOM elements to standardize and clarify the mappings. We followed a similar process for the other mapping exercises.

In the updated file, subject\_id represents BCDM terms and object\_id refers to the corresponding UNITE terms, demonstrating the directional mapping from BCDM to UNITE. For example, bcdm:processid maps to unite:source\_url with skos:closeMatch as a predicate\_id. Thus, the mapping context becomes (using the subject-predicate-object triple framework): bcdm:processid maps to unite:source\_url, and we consider this a close match rather than an exact match, based on the Simple Knowledge Organization System (SKOS[^11]) vocabulary. 

Key SSSOM elements such as predicate\_id, mapping\_justification, mapping\_date, and author\_id were added to provide comprehensive metadata for each mapping. In another mapping, bcdm:processid maps to [dwc:materialSampleID](https://dwc.tdwg.org/terms/#dwc:materialSampleID) with skos:exactMatch as the predicate\_id. This indicates a direct equivalence between the terms. This structured approach ensures that each mapping is clear, justified, tracked and maintainable. This approach also allows the mapping file to be machine readable and aligns with the suggestions coming out from different European FAIR mapping initiatives (Metadata and Schema Crosswalk Registry from FAIRCORE4EOSC [@Sanden2024-13].

It is important to note that not all namespace prefixes resolve to a resource that provides further machine-readable metadata or explicitly enumerates the terms from the namespace. For instance, DwC provides IRIs for each term and RDF and XML serializations. Each ENA checklist has a browsable list (example: [ERC000013](https://www.ebi.ac.uk/ena/browser/view/ERC000013)) and an XML download option (example: [ERC000013 XML](https://www.ebi.ac.uk/ena/browser/api/xml/ERC000013)). However, the approach to maintaining terms and vocabularies is not consistent across all data formats and repositories.

In addition to this semantic mapping work, the data integration theme extended to the structural organization of BGE’s genome skimming data submissions. ENA and the genome skimming data uploaders, NHM and Naturalis, agreed upon a multi-level project structure for data submission. This structure assigns different specimen providers their own subproject under which the barcoding data for each specimen is linked with the specific BioSample [@Courtot2022-14] entry assigned to it. 

The proposed setup permits the attachment of richer metadata that goes beyond what can be linked directly to sequence records, addressing previous issues where metadata was lost during synchronization between BOLD and GenBank [@Sayers2024-15]. An important aspect of future work outlined during the hackathon involves setting up authentication and data submission processes to incorporate genome skimming data into ENA to make use of this possibility. 

Furthermore, the hackathon highlighted the need for taxonomic alignment between UNITE and BOLD. With UNITE mapping its taxa, or species hypotheses, to various taxonomies including the Catalogue of Life [@Banki2022-16], the integration of these systems is facilitated by the ChecklistBank [@Doring2022-17], which manages numerous taxonomic checklists, including the BOLD taxonomy. This connection is seen as a pathway for ensuring that the taxonomies used across different databases are harmonized, enhancing the taxonomic reconciliation of data across these platforms.

## Reference Data Curation

The curation theme at the hackathon focused on enhancing the automated curation of BOLD records to determine their suitability for inclusion in reference libraries for metabarcoding within BGE. Such reference libraries are a key deliverable from WP10. Initially, the curation was handled by a set of Perl modules and scripts, which by the end of the hackathon were integrated into a Snakemake pipeline, publicly accessible for further use and development[^12]. This pipeline was also documented and submitted to WorkflowHub during the hackathon[^13].

The pipeline operates by taking a BOLD data package formatted as a BCDM-compliant TSV file as input. This TSV file is ingested into a SQLite relational database where several operations are conducted: normalization of taxonomy data, addition of tables that define and track the status of curation criteria, and computation of indexes to facilitate queries. Object-relational mapping (ORM) Perl helper classes are generated from the database schema to support the curation scripts. These scripts, in turn, produce a TSV file for each curation criterion, which is re-ingested into the database. This structure allows for the computation of aggregated quality scores for each sequence record, providing a ranked metric for assessing record suitability.

Although the pipeline’s framework is operational, refinement of specific curation criteria and verification of results is ongoing. Post-hackathon work includes the development of scripts to assess the quality of matches between species and BINs in the database. The results of these assessments are classified according to the Barcode, Audit & Grade System (BAGS) grading system [@Fontes2021-18]. This grading system aids in determining the reliability of sequence records and their potential inclusion in reference libraries.

Future work involves not only refining these automated processes but also presenting outputs in a manner conducive to manual verification by taxonomic experts. This manual curation serves as a check to adjudicate whether discrepancies between species and BINs are biologically plausible. The ultimate goal of this curation process is to finalize which records are included in the reference libraries, slated for publication as datasets on BOLD. This ensures that only reliable and accurate data is used in biodiversity assessments and related research, both within BGE’s metabarcoding activities and beyond.

# Conclusions

The 2024 BGE Barcoding Hackathon achieved concrete advancements in the digital infrastructure and data handling practices essential for single specimen barcoding. By concentrating efforts on the four thematic pillars—Data Generation and Processing, BOLD Release Candidate, Wider Data Integration, and Reference Data Curation—the event achieved progress in several key areas.

The improvements in barcode generation pipelines and genome skimming processes have streamlined the production and quality assurance of DNA barcodes. The development and enhancement of BOLD version 5 represent a shift towards a more scalable, decentralized, and interoperable data publishing system. The harmonization of data standards across platforms like BOLD, ENA, and UNITE has facilitated better integration and sharing of genomic data, promoting richer metadata exchange and enhancing the overall utility of molecular biodiversity data repositories. Additionally, the automation and refinement of reference data curation processes ensure that only high-quality, reliable data is included in reference libraries, supporting accurate biodiversity assessments and research.

Concretely, the specific next actions following the hackathon for the respective themes are as follows:

* **Data Generation and Processing** \- Incorporate MultiQC output in the genome skimming pipeline for QA purposes. Adopt a common reference library and taxon validation step for genome skimming and amplicon sequencing results. Adopt a common non-sense mutation check (scanning for premature stop codons) for genome skimming and amplicon sequencing.  
* **BOLD release candidate** \- Apply the UI components developed for the reference page on country-specific barcoding results to the other pages in the web application. Finalize the institution-specific results page. Finalize the back-end enhancements for performance and autocomplete functionality.   
* **Wider data integration** \- Implement the proposed project structure for data submission to ENA of genome skimming results. Finalize UNITE’s web service endpoint for BCDM-compliant data delivery. Operationalize the vocabulary-mapping to concrete translation of barcoding metadata between data resources.  
* **Reference data curation** \- Verify the accuracy of the metadata grading pipeline and the BAGS ranks on a subsample of BOLD data. Pre-filter BOLD data through triage into records that are optimal by both standards and those that require manual curation. Partition the latter by taxonomic groups in line with the expertise of the respective curators.

The collaborative efforts during the hackathon have set a solid foundation for future work, with a focus on continuous improvement and standardization of workflows and data integration practices. Overall, the hackathon has significantly contributed to BGE’s objectives, fostering an environment of cooperation and innovation that will drive forward the goals of molecular biodiversity monitoring and research at scale.

# Acknowledgements

We acknowledge the support of the Horizon Europe Framework Programme of the European Union under grant agreement No. 101059492\. The BGE project is funded by Horizon Europe under the Biodiversity, Circular Economy and Environment (REA.B.3); co-funded by the Swiss State Secretariat for Education, Research and Innovation (SERI) under contract number 22.00173; and by the UK Research and Innovation (UKRI) under the Department for Business, Energy and Industrial Strategy’s Horizon Europe Guarantee Scheme.

# Author Contributions

The main manuscript was drafted by RAV. The Data Generation and Processing theme was contributed to by TFB, EC, PEC, DG, MK, HM, BP, GS, and OW. The BOLD Release Candidate theme was contributed to RA, JIA, JOA, SR, CW, and RAV. The Wider Data Integration section was contributed to by KA, SJB, SI, NJ, VBK, DL, JP, and SSR. The Reference Data Curation section was contributed to by TFB, PEC, FD, BP, and SSR. All coauthors have verified and approved the final version of this manuscript.

# References


[^1]:  [https://github.com/o-william-white/skim2mt](https://github.com/o-william-white/skim2mt) 

[^2]:  [https://github.com/MultiQC/MultiQC](https://github.com/MultiQC/MultiQC) 

[^3]:  [https://github.com/UoMResearchIT/ro-crate\_snakemake\_tooling](https://github.com/UoMResearchIT/ro-crate_snakemake_tooling) 

[^4]:  [https://workflowhub.eu/workflows/791](https://workflowhub.eu/workflows/791) 

[^5]:  [https://github.com/gjeunen/reference\_database\_creator](https://github.com/gjeunen/reference_database_creator) 

[^6]:  [https://github.com/DNAdiversity/BCDM](https://github.com/DNAdiversity/BCDM) 

[^7]:  [https://boldsystems.eu/api/docs](https://boldsystems.eu/api/docs) 

[^8]:  [https://www.dissco.eu/](https://www.dissco.eu/) 

[^9]:  [https://www.ebi.ac.uk/ena/browser/view/ERC000053](https://www.ebi.ac.uk/ena/browser/view/ERC000053) 

[^10]:  [https://github.com/bge-barcoding/StayingMapped](https://github.com/bge-barcoding/StayingMapped) 

[^11]:  [https://www.w3.org/2004/02/skos/](https://www.w3.org/2004/02/skos/) 

[^12]:  [https://github.com/FabianDeister/Library\_curation\_BOLD](https://github.com/FabianDeister/Library_curation_BOLD) 

[^13]:  [https://workflowhub.eu/workflows/833](https://workflowhub.eu/workflows/833) 

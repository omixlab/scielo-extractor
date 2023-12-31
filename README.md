# SciELO Extractor

This is a simples CLI application to extract data from [SciELO (Scientific Electronic Library Online)](https://www.scielo.br/).

<p align="center">
  <img src='https://scielo.org/static/images/logo-scielo-portal-no-label.svg' style='width:100px'>
</p>

> SciELO (Scientific Electronic Library Online) is a bibliographic database, digital library, and cooperative electronic publishing model of open access journals. SciELO was created to meet the scientific communication needs of developing countries and provides an efficient way to increase visibility and access to scientific literature. Originally established in Brazil in 1997, today there are 16 countries in the SciELO network and its journal collections: Argentina, Bolivia, Brazil, Chile, Colombia, Costa Rica, Cuba, Ecuador, Mexico, Paraguay, Peru, Portugal, South Africa, Spain, Uruguay, and Venezuela. ([Wikipedia](https://pt.wikipedia.org/wiki/Scientific_Electronic_Library_Online))

## Installing

To install, just use the command:

```
$ pip install scielo-extractor
```

## Usage 

To use the extractor, just provide a query, following SciELO search terms and boolean expressions, an output format (CSV or JSON) and a name for the output file.

```
$ scielo-extractor --query "((ti:leptospira)) AND (au:Kremer)" --output papers.json --format json
```

Using this query, the following file was produced:

```json
[
    {
        "authors": "Jorge,S\u00e9rgio;Kremer,Frederico Schmitt;Oliveira,Natasha Rodrigues de;Navarro,Gabrielle de Oliveira Sanches Valerio;Guimar\u00e3es,Amanda Munari;Sanchez,Christian Domingues;Woloski,Rafael Danelon dos Santos;Ridieri,Karine Forster;Campos,Vin\u00edcius Farias;Pinto,Luciano da Silva;Dellagostin,Odir Ant\u00f4nio",
        "title": "Whole-genome sequencing of Leptospira interrogans from southern Brazil: genetic features of a highly virulent strain",
        "journal": "Mem\u00f3rias do Instituto Oswaldo Cruz",
        "volume": "v113n2",
        "issue": "",
        "doi": "10.1590/0074-02760170130",
        "year": "2018-02",
        "abstract": " BACKGROUND Leptospirosis is the most widespread zoonotic disease. It is caused by infection with pathogenic Leptospira species, of which over 300 serovars have been described. The accurate identification of the causative Leptospira spp. is required to ascertain the pathogenic status of the local isolates.  OBJECTIVES This study aimed to obtain the complete genome sequence of a virulent Leptospira interrogans strain isolated from southern Brazil and to describe its genetic features.  METHODS The whole genome was sequenced by next-generation sequencing (Ion Torrent). The genome was assembled, scaffolded, annotated, and manually reviewed. Mutations were identified based on a variant calling analysis using the genome of L. interrogans strain Fiocruz L1-130 as a reference.  FINDINGS The entire genome had an average GC content of 35%. The variant calling analysis identified 119 single nucleotide polymorphisms (SNPs), from which 30 led to a missense mutation. The structural analyses identified potential evidence of genomic inversions, translocations, and deletions in both the chromosomes.  MAIN CONCLUSIONS The genome properties provide comprehensive information about the local isolates of Leptospira spp., and thereby, could facilitate the identification of new targets for the development of diagnostic kits and vaccines.",
        "start_page": "80",
        "end_page": "86"
    },
    {
        "authors": "Eslab\u00e3o,Marcus Red\u00fc;Kremer,Frederico Schmitt;Ramos,Rommel Thiago Juca;Silva,Artur Luiz da Costa da;Azevedo,Vasco Ariston de Carvalho;Pinto,Luciano da Silva;Silva,\u00c9verton Fagonde da;Dellagostin,Odir Ant\u00f4nio",
        "title": "Genome of Leptospira borgpetersenii strain 4E, a highly virulent isolate obtained from Mus musculus in southern Brazil",
        "journal": "Mem\u00f3rias do Instituto Oswaldo Cruz",
        "volume": "v113n2",
        "issue": "",
        "doi": "10.1590/0074-02760170111",
        "year": "2018-02",
        "abstract": "A previous study by our group reported the isolation and characterisation of Leptospira borgpetersenii serogroup Ballum strain 4E. This strain is of particular interest because it is highly virulent in the hamster model. In this study, we performed whole-genome shotgun genome sequencing of the strain using the SOLiD sequencing platform. By assembling and analysing the new genome, we were able to identify novel features that have been previously overlooked in genome annotations of other strains belonging to the same species.",
        "start_page": "137",
        "end_page": "141"
    },
    {
        "authors": "Moreno,Luisa Z;Miraglia,Fabiana;Kremer,Frederico S;Eslabao,Marcus R;Dellagostin,Odir A;Lilenbaum,Walter;Freitas,Julio C;Vasconcellos,Silvio A;Heinemann,Marcos B;Moreno,Andrea M",
        "title": "Comparative genomics of pathogenic Leptospira interrogans serovar Canicola isolated from swine and human in Brazil",
        "journal": "Mem\u00f3rias do Instituto Oswaldo Cruz",
        "volume": "v113n2",
        "issue": "",
        "doi": "10.1590/0074-02760170119",
        "year": "2018-02",
        "abstract": "Leptospira interrogans serovar Canicola is one of the most important pathogenic serovars for the maintenance of urban leptospirosis. Even though it is considered highly adapted to dogs, serovar Canicola infection has already been described in other animals and even a few human cases. Here, we present the genomic characterisation of two Brazilian L. interrogans serovar Canicola strains isolated from slaughtered sows (L0-3 and L0-4) and their comparison with human strain Fiocruz LV133. It was observed that the porcine serovar Canicola strains present the genetic machinery to cause human infection and, therefore, represent a higher risk to public health. Both human and porcine serovar Canicola isolates also presented sequences with high identity to the Chinese serovar Canicola published plasmids pGui1 and pGui2. The plasmids identification in the Brazilian and Chinese serovar Canicola strains suggest that extra-chromosomal elements are one more feature of this serovar that was previously unnoticed.",
        "start_page": "126",
        "end_page": "129"
    },
    {
        "authors": "Moreno,Luisa Z;Miraglia,Fabiana;Loureiro,Ana P;Kremer,Frederico S;Eslabao,Marcus R;Dellagostin,Odir A;Lilenbaum,Walter;Vasconcellos,Silvio A;Heinemann,Marcos B;Moreno,Andrea M",
        "title": "Genomic characterisation of Leptospira inadai serogroup Lyme isolated from captured rat in Brazil and comparative analysis with human reference strain",
        "journal": "Mem\u00f3rias do Instituto Oswaldo Cruz",
        "volume": "v113n5",
        "issue": "",
        "doi": "10.1590/0074-02760170444",
        "year": "2018",
        "abstract": "Leptospira inadai is classified as a species of the Leptospira intermediate group that has been poorly studied due to its apparent insignificance to human and animal health. Nevertheless, over the last two decades the species has been described in human cases in India and in carrier animals in Ecuador. Here, we present the first identification and genomic characterisation of L. inadai serogroup Lyme isolated from captured rodent in Brazil. Even though the M34/99 strain was not pathogenic for hamsters, it was able to establish renal colonisation. The M34/99 strain presented high similarity with L. inadai serogroup Lyme human reference indicating that animal strain could also infect humans, although it does not represent high risk of severe disease. An extrachromosomal sequence was also identified in M34/99 strain and presented high identity with previously described L. inadai phage LinZ_10, suggesting that phage-like extrachromosomal sequence may be another feature of this understudied species.",
        "start_page": null,
        "end_page": null
    },
    {
        "authors": "Moreno,Luisa Z;Kremer,Frederico S;Miraglia,Fabiana;Loureiro,Ana P;Eslabao,Marcus R;Dellagostin,Odir A;Lilenbaum,Walter;Moreno,Andrea M",
        "title": "Comparative genomic analysis of Brazilian Leptospira kirschneri serogroup Pomona serovar Mozdok",
        "journal": "Mem\u00f3rias do Instituto Oswaldo Cruz",
        "volume": "v111n8",
        "issue": "",
        "doi": "10.1590/0074-02760160174",
        "year": "2016-08",
        "abstract": "Leptospira kirschneri is one of the pathogenic species of the Leptospira genus. Human and animal infection from L. kirschneri gained further attention over the last few decades. Here we present the isolation and characterisation of Brazilian L. kirschneri serogroup Pomona serovar Mozdok strain M36/05 and the comparative genomic analysis with Brazilian human strain 61H. The M36/05 strain caused pulmonary hemorrhagic lesions in the hamster model, showing high virulence. The studied genomes presented high symmetrical identity and the in silico multilocus sequence typing analysis resulted in a new allelic profile (ST101) that so far has only been associated with the Brazilian L. kirschneri serogroup Pomona serovar Mozdok strains. Considering the environmental conditions and high genomic similarity observed between strains, we suggest the existence of a Brazilian L. kirschneri serogroup Pomona serovar Mozdok lineage that could represent a high public health risk; further studies are necessary to confirm the lineage significance and distribution.",
        "start_page": "539",
        "end_page": "541"
    },
    {
        "authors": "Kremer,Frederico S;Eslab\u00e3o,Marcus R;Jorge,S\u00e9rgio;Oliveira,Natasha R;Labonde,Julia;Santos,Monize NP;Monte,Leonardo G;Grassmann,Andr\u00e9 A;Cunha,Carlos EP;Forster,Karine M;Moreno,Lu\u00edsa Z;Moreno,Andrea M;Campos,Vinicius F;McBride,Alan JA;Pinto,Luciano S;Dellagostin,Odir A",
        "title": "Draft genome of the Leptospira interrogans strains, Acegua, RCA, Prea, and Capivara, obtained from wildlife maintenance hosts and infected domestic animals",
        "journal": "Mem\u00f3rias do Instituto Oswaldo Cruz",
        "volume": "v111n4",
        "issue": "",
        "doi": "10.1590/0074-02760160010",
        "year": "2016-04",
        "abstract": "In the present paper, we announce new draft genomes of four Leptospira interrogans strains named Acegua, RCA, Prea, and Capivara. These strains were isolated in the state of Rio Grande do Sul, Brazil, from cattle, dog, Brazilian guinea pig, and capybara, respectively.",
        "start_page": "280",
        "end_page": "283"
    }
]
```

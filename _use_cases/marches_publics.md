---
layout: usecases
title: Marchés Publics
---

## Introduction

Depuis le 1er octobre 2018, les acheteurs publics ont l'obligation légale de passer par une plateforme de dématérialisation des procédures de marchés publics (profil acheteur), pour tout marché dont le besoin estimé est supérieur à 25 000 € HT.
L'accès aux données de l'API Entreprise dans le cas des marchés publics se fait par l'intermédiaire des places de marchés publics.

## Vous avez déjà accès aux données

##### Vous êtes un acheteur public ?

Il est fort probable que vous ayez en réalité déjà accès aux données d'API Entreprise par l'intermédiaire :
- du Document Unique du Marché Européen&#42; (DUME) que peut remplir l'entreprise,
- de votre profil acheteur si celui-ci utilise le service DUME&#42;,
- de votre profil acheteur si l'éditeur nous a demandé un accès direct (cf tableau ci-dessous).

&#42;*Le DUME et le service DUME sont branchés sur API Entreprise.*

Si vous avez un doute, renseignez-vous auprès de votre profil acheteur pour savoir s'il implémente le service DUME ou s'il est connecté directement à API Entreprise.

##### Vous êtes un éditeur de place de marchés publics ?

- Renseignez-vous pour mettre en place le DUME : l'État met gratuitement à disposition le service.
- Si vous souhaitez utiliser l’API dans le cadre d’une application spécifique, il convient de nous préciser le cas d’utilisation, et faire une demande d'accès.


## Liste des éditeurs de places de marchés dotés d'un droit d'accès

{:.tpl-table}
| Éditeur                  |     Profil acheteur associé                 |
|:------------------------:|:-------------------------------------------:|
|    achatpublic.com       |                                             |
|    Atexo                 | Place, pour les administrations centrales   |
|    AWS                   |                                             |
|    provigis              |                                             |
|    klekoon.com           |                                             |


## Données utiles

Vous trouverez ci-dessous les données utiles dans le cadre des marchés publics et classées dans différentes catégories :
- [Informations générales](#infos_generales),
- [Informations financières](#infos_financieres),
- [Attestations sociales et fiscales](#attestations_sociales_fiscales),
- [Certificats professionnels](#certificats_pro),
- [Propriété intellectuelle](#propriete_intellectuelle).


#### Informations générales <a id="infos_generales"></a>

{:.tpl-table}
| Données                                              |        Producteur        |                 Endpoint                  |        Type         |    Ouverture    |
| ----------------------------------------------------- |:------------------------:|:-----------------------------------------:|:-------------------:|:---------------:|
| [Données de référence d'une entreprise](https://doc.entreprise.api.gouv.fr/?json#entreprises){:target="_blank"}                  |    INSEE & Infogreffe    |            `entreprises`            |    données JSON     |    publiques    |
| [Données de référence d'un établissement](https://doc.entreprise.api.gouv.fr/?json#etablissements){:target="_blank"}                |          INSEE           |          `etablissements`           |    données JSON     |    publiques    |
| [Extrait  RCS](https://doc.entreprise.api.gouv.fr/?json#infogreffe-extrait-rcs){:target="_blank"}                                           |        Infogreffe        |         `extraits_rcs_infogreffe`         |    données JSON     |    publiques    |
| [Données déclaratives d'une association](https://doc.entreprise.api.gouv.fr/?json#associations-rna){:target="_blank"}                 | Ministère de l'Intérieur |              `associations`               |    données JSON     |    publiques    |
| [Divers documents d'une association](https://doc.entreprise.api.gouv.fr/?json#documents-association){:target="_blank"}                     | Ministère de l'Intérieur |         `documents_associations`          |     PDF (image)     |    publiques    |

#### Informations financières <a id="infos_financieres"></a>

{:.tpl-table}
| Données                                              |        Producteur        |                 Endpoint                  |        Type         |    Ouverture    |
| ----------------------------------------------------- |:------------------------:|:-----------------------------------------:|:-------------------:|:---------------:|
| [Chiffre d'affaires](https://doc.entreprise.api.gouv.fr/?json#exercices){:target="_blank"}                                     |          DGFIP           |                `exercices`                |    données JSON     | confidentielles |
| [Bilans entreprise](https://doc.entreprise.api.gouv.fr/?json#bilans-entreprises-bdf-banque-de-france){:target="_blank"}                                      |     Banque de France     |         `bilans_entreprises_bdf`          |    données JSON     | confidentielles |
| [Déclarations et dictionnaire de liasses fiscales](https://doc.entreprise.api.gouv.fr/?json#les-d-clarations-des-liasses-fiscales){:target="_blank"}       |          DGFIP           |         `liasses_fiscales_dgfip`          |    données JSON     | confidentielles |

#### Attestations sociales et fiscales <a id="attestations_sociales_fiscales"></a>

{:.tpl-table}
| Données                                              |        Producteur        |                 Endpoint                  |        Type         |    Ouverture    |
| ----------------------------------------------------- |:------------------------:|:-----------------------------------------:|:-------------------:|:---------------:|
| [Attestation fiscale](https://doc.entreprise.api.gouv.fr/?json#attestation-fiscale-dgfip){:target="_blank"}                                    |          DGFIP           |       `attestations_fiscales_dgfip`       |     PDF (texte)     | confidentielles |
| [Attestation de vigilance](https://doc.entreprise.api.gouv.fr/?json#attestation-sociale-acoss){:target="_blank"}                               |          ACOSS           |       `attestations_sociales_acoss`       |     PDF (texte)     | confidentielles |
| [Conformité emploi des travailleurs handicapés AGEFIPH](https://doc.entreprise.api.gouv.fr/?json#attestation-agefiph){:target="_blank"}  |         AGEFIPH          |          `attestations_agefiph`           |    données JSON     | confidentielles |
| [Cotisation de sécurité sociale agricole](https://doc.entreprise.api.gouv.fr/?json#cotisations-msa){:target="_blank"}                |           MSA            |             `cotisations_msa`             |    données JSON     | confidentielles |
| [Attestations cotisation retraite](https://doc.entreprise.api.gouv.fr/?json#cotisations-retraite-probtp){:target="_blank"}                       |          PROBTP          | `attestations_cotisation_retraite_probtp` |    données JSON     |    publiques    |
| [Carte professionnelle travaux publics](https://doc.entreprise.api.gouv.fr/?json#cartes-professionnelles-fntp){:target="_blank"}         |          CNETP           |            `cartes_professionnelles_fntp`            |         PDF         |    publiques    |
| [Cotisations congés payés & chômage intempéries](https://doc.entreprise.api.gouv.fr/?json#certificats-cnetp){:target="_blank"}         |          CNETP           |            `certificats_cnetp`            |         PDF         |    publiques    |

#### Certificats professionnels <a id="certificats_pro"></a>

{:.tpl-table}
| Données                                              |        Producteur        |                 Endpoint                  |        Type         |    Ouverture    |
| ----------------------------------------------------- |:------------------------:|:-----------------------------------------:|:-------------------:|:---------------:|
| [Certification RGE](https://doc.entreprise.api.gouv.fr/?json#certificats-rge-ademe){:target="_blank"}                                      |          ADEME           |          `certificats_rge_ademe`          | données JSON et PDF |    publiques    |
| [Certification de qualification OPQIBI](https://doc.entreprise.api.gouv.fr/?json#certificats-opqibi){:target="_blank"}                  |          OPQIBI          |           `certificats_opqibi`            |    données JSON     |    publiques    |
| [Certification de qualification Qualibat](https://doc.entreprise.api.gouv.fr/?json#certificats-qualibat){:target="_blank"}                  |          OPQIBI          |           `certificats_qualibat`            |    données JSON     |    publiques    |

#### Propriété intellectuelle <a id="propriete_intellectuelle"></a>

{:.tpl-table}
| Données                                              |        Producteur        |                 Endpoint                  |        Type         |    Ouverture    |
| ----------------------------------------------------- |:------------------------:|:-----------------------------------------:|:-------------------:|:---------------:|
| [Brevets, modèles et marques déposées](https://doc.entreprise.api.gouv.fr/?json#extraits-courts-inpi){:target="_blank"}                   |           INPI           |          `extraits_courts_inpi`           |    données JSON     |    publiques    |



**Rappel** : Les places de marchés disposent d'un accès à l'API entreprise, ***il n'est donc pas nécessaire d'effectuer une demande d'accès à API Entreprise.***

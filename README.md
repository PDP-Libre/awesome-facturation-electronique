# Awesome Facturation Electronique

## Spécification AIFE

- [Spécifications externes B2B](https://www.impots.gouv.fr/specifications-externes-b2b)
- [FactureX](https://fnfe-mpe.org/factur-x/)
- [Norme XP Z12-012](https://www.boutique.afnor.org/fr-fr/norme/xp-z12012/formats-et-profils-des-messages-factures-et-statuts-de-cycle-de-vie-constit/fa213746/452462)
- [Norme XP Z12-013](https://www.boutique.afnor.org/fr-fr/norme/xp-z12013/api-pour-interfacer-les-systemes-dinformations-des-entreprises-avec-les-pla/fa213747/452463)
- [Norme XP Z12-014](https://www.boutique.afnor.org/fr-fr/norme/xp-z12014/cas-dusage-b2b-applicables-dans-le-cadre-la-reforme-facture-electronique-en/fa213748/452464)

## PEPPOL

- [Site officiel](https://peppol.org/)
- [Wikipedia](https://fr.wikipedia.org/wiki/PEPPOL)
- [Spécification](https://peppol.org/documentation/technical-documentation/post-award-documentation/)
- [Liste sur le site officiel des implémentations](https://peppol.org/tools-support/links-to-software/)
- [Oxalis](https://github.com/OxalisCommunity/oxalis): Implémentation en java
- [Rejoindre le réseau](https://www.impots.gouv.fr/rejoindre-le-reseau-peppol)

## PA (anciennement PDP)

- [Déclaration](https://www.impots.gouv.fr/sites/default/files/media/1_metier/2_professionnel/EV/2_gestion/290_facturation_electronique/guide-utilisateur---demarches-simplifiees---immatriculation-pdp---2023-06.pdf)
- [Liste officielle](https://www.impots.gouv.fr/liste-des-plateformes-agreees-immatriculees-sous-reserve) 

## Planning

- S1 2026: Publication de la procédure de test des PDP et certification des premiers PDP
- juillet 2026: L’ensemble des entreprises assujetties à la TVA doivent pouvoir recevoir des factures électroniques. Les TPE/PME ne sont pas obligées d’émettre.
- juillet 2027: L’ensemble des entreprises doivent émettre via les PDP.

## Annuaire

- [Chorus](https://facturation.chorus-pro.gouv.fr/annuaire/#/): Chorus permet de rechercher une entreprise et savoir si elle a activé la facturation électronique.

## Factur-x
### Outils standalones

- [FNF-E](https://services.fnfe-mpe.org/account/home): service de validation "officiel".
- [xmllint](https://manpages.debian.org/buster/libxml2-utils/xmllint.1.en.html): Outil générique de vérification, possible de l'utiliser avec le xsd fourni par la FNF-E (`xmllint --schema Factur-X_1.07.3_EN16931.xsd factur-x.xml`)
- [saxonb-xslt](https://manpages.debian.org/buster/libsaxonb-java/saxonb-xslt.1.en.html): Comme xmllint, mais permet de valider avec le XSLT 2.0 (`saxonb-xslt -xsl:FACTUR-X_EN16931.xslt -s:factur-x.xml`)
- [verapdf](https://demo.verapdf.org/): Permet de valider la norme du PDF
- [Ghostscript](https://ghostscript.com/blog/zugferd.html): Permet de générer la facture en ligne de commande.
- [Pince](https://www.princexml.com/): Payant & Non opensource. Fonction de haut niveau et notamment convertir un fichier html en pdf.
- [Mustang Server](https://mustangserver.com/validate/): Permet de valider un document

### Library

- [Python factur-x](https://github.com/akretion/factur-x): Génération, extraction, vérification. Utilisé par le projet Odoo.
- [Libreoffice factur-x](https://github.com/akretion/factur-x-libreoffice-extension): même auteur et functionnalité de la library en python
- [PHP factur-x](https://github.com/atgp/factur-x): Génération, extraction, vérification. Issue de la communauté allemande.
- [JAVA Mustang](https://www.mustangproject.org/) : Lecture, Génération, extraction, vérification, convertion de format. Issue de la communauté allemande.
- 
## UBL (Universal Business Language)
by :The Organization for the Advancement of Structured Information Standards (OASIS) https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=ubl
Universal Business Language Version 2.3 (https://docs.oasis-open.org/ubl/UBL-2.3.html) (https://github.com/oasis-tcs/ubl)

### Outils standalones
- [PHP UBL] (https://github.com/thegreenter/ubl-validator) : OASIS Universal Business Language (UBL) Schema Validator
- [JAVA UBL] (https://github.com/VartikaG02/en16931-ubl2cii) convert UBL to CII
- [JAVA UBL] (https://github.com/phax/en16931-cii2ubl) Converter for unidirectional EN16931 invoices from CII D16B to UBL 2.1, 2.2, 2.3 or 2.4.

### Library
- [JAVA UBL] (https://github.com/phax/ph-ubl):Set of Java libraries for reading and writing OASIS UBL 2.0, 2.1, 2.2, 2.3 and 2.4 documents.


## CII (Cross Industry Invoice) 
standard ouvert développé par le Centre des Nations Unies pour la facilitation du commerce et les transactions électroniques (UN/CEFACT)
### Library
- [JAVA CII] (https://github.com/phax/ph-cii) Java Wrapper for the UN/CEFACT Cross Industry Invoice.This library focuses currently on D16A.1 and D16B for use with the EN resulting from directive 2014/55/EU. Additionally it supports D22B for support for the Zugferd 2.3+ versions.

## Divers

- [Weasyprint](https://weasyprint.org/): Conversion HTML en PDF. [Article pour rajouter les données annexes](https://binary-butterfly.de/artikel/factur-x-zugferd-e-invoices-with-python/)
- [e-invoice-eu](https://github.com/gflohr/e-invoice-eu/tree/main)  Free and open source tool chain for generating EN16931 conforming e-invoices (Factur-X/ZUGFeRD, UBL, CII, XRechnung) from popular spreadsheet formats or JSON with free and open source software.


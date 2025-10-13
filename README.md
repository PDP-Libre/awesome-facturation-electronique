# Awesome Facturation Electronique

## Factur-x
### Outils standalones

- [FNF-E](https://services.fnfe-mpe.org/account/home): service de validation "officiel".
- [xmllint](https://manpages.debian.org/buster/libxml2-utils/xmllint.1.en.html): Outil générique de vérification, possible de l'utiliser avec le xsd fourni par la FNF-E (`xmllint --schema Factur-X_1.07.3_EN16931.xsd factur-x.xml`)
- [saxonb-xslt](https://manpages.debian.org/buster/libsaxonb-java/saxonb-xslt.1.en.html): Comme xmllint, mais permet de valider avec le XSLT 2.0 (`saxonb-xslt -xsl:FACTUR-X_EN16931.xslt -s:factur-x.xml`)
- [verapdf](https://demo.verapdf.org/): Permet de valider la norme du PDF
- [Ghostscript](https://ghostscript.com/blog/zugferd.html): Permet de générer la facture en ligne de commande.
- [Pince](https://www.princexml.com/): Payant & Non opensource. Fonction de haut niveau et notamment convertir un fichier html en pdf.

### Library

- [Python factur-x](https://github.com/akretion/factur-x): Génération, extraction, vérification. Utilisé par le projet Odoo.
- [Libreoffice](https://github.com/akretion/factur-x-libreoffice-extension): même auteur et functionnalité de la library en python
- [PHP factur-x](https://github.com/atgp/factur-x): Génération, extraction, vérification. Issue de la communauté allemande.


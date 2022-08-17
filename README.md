# Bible Publications Details

**A detailed registry of Bible originals, translations, editions, and publications**

This is part of the *Bible Organisational System* (BibleOrgSys or BOS) software package
that has been renamed and separated out as a separate library.
Formerly this was called *Bible Organisational Systems*.

Also includes short Bible version codes, e.g., KJB for King James Bible
or NIV for New International Version.
However there’s also different editions so KJB-1611 is quite different from KJB-1769.

## History

Most Bible study software displays multiple different Bible versions and so typically they create their own short reference codes.
However, this is an attempt to provide a registry of codes that publishers can add to (and correct)
and which will be used as a part of the [Bible Reference system](https://github.com/Freely-Given-org/BibleReferences)
and hence the syntax is restrained by compatibility with that.

These version codes can also include other resources like commentaries that also
use B/C/V (book/chapter/verse) structuring. Note however that commentaries and
such-like will generally be assigned longer abbreviations, i.e., Bibles and partial Bibles like New Testaments will be given priority on the shorter codes.

This data was originally hosted [here](https://Freely-Given.org/BibleReference/BibleVersions/) (now archived) and part of [this](https://github.com/Freely-Given-org/BibleOrgSys/blob/main/BibleOrgSys/DataFiles/BibleOrganisationalSystems.xml).

## Aims

- To provide a registry of short (2-8 character) abbreviations for Bible versions or commentaries
- To include both original language Bible texts and translations
- Version code must not contain whitespace (so it’s a single token)
- May contain uppercase and lowercase letters (including any Unicode letters), but the UPPERCASEd version must be unique, i.e., can have MyRV but can’t have both MyRV and MYRV representing different publications
- To avoid clashes when a publisher is looking for new abbreviation (remembering that Bibles are published in many languages), some versions will need to make adjustments -- first in, first served, e.g., if SRV is "Seminary Revised Version" then "Swahili Revised Version" might need to be SwRV
- To be able to have a 4-digit publication year appended as necessary, e.g., KJB-1611
- To be able to have an edition string appended as necessary KJB!MBS_1997_Printing or KJB-1769!MBS_1997_Printing

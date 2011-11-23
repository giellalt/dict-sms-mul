This directory contains material relevant to the Skolt gtdictionary. The aim of this "common" dictionary database is to create a rich structure in one single lexicon file which later allows exporting for different purposes: e.g. bilingual learner dictionaries, Oahpa!, descriptive dictionaries, etc. Thus "sms2X" basically means both …2Xlanguages and …2Xproducts.

Documentation at http://victorio.uit.no/cgi-bin/wiki/index.php/Smsdict

Incoming raw files go into inc/

Apostrophe ´ is Modifier Letter Apostrophe

English default is "American"

=====
meta
=====
Here is the list of the attribute values for the attribute 'meta'
on the e-element in the xml files:

01 - this is a list of sme entries with multiple translations collected by Kimberly Mäkäräinen (http://www.uta.fi/~km56049/same/skolt/koltansaame.html).

02 - 99-word list from the current smsoahpa; this word list with multiple translations, taken from the 100-Swadesh-list, was originally collected by Michael Rießler.

03 - word list from teaching materials under deveolpment by the Project "Skolt Saami Culture across Borders" (building on an already existing Finnish version, which is extended with Russian [Eino Koponen] and Norwegian [Michael Rießler] translations); each lesson of this materials gets its own attribute

04 - entries added manually by Michael Rießler; these are mostly from field- or other notes and will serve to test the most appropriate structure for the "common" dictionary database

=====
TODO
=====

TODO's 
* write better documentation
* think about better grouping, e.g.
** <lg>
** <etymology group>
** <oahpa group> (simpler <mg> for oahpa export) 
** <mg> (complete information, for dictionary export)
** …
* fill in xxx's
* check <t> vs. <tg> vs. <mg>
* check <tr> <te> (what exactly does it mean?)
* check inflected personal pronouns (e.g. <l pos="PRO" person="2" number="sg">tun</l>) (how should they be listed?)

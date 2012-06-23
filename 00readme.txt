This directory contains material relevant to the Skolt gtdictionary. The aim of this "common" dictionary database is to create a rich structure in one single lexicon file which later allows exporting for different purposes: e.g. bilingual learner dictionaries, Oahpa!, descriptive dictionaries, etc. Thus "sms2X" basically means both …2Xlanguages and …2Xproducts.

Documentation at http://victorio.uit.no/cgi-bin/wiki/index.php/Smsdict

Incoming raw files go into inc/

=====
Preliminary conventions
=====
ʹ = 02B9.MODIFIER LETTER PRIME (This is a syllable break)
!! e.g. 'to be heard' kollʹjed 
ˈ = 02C8 MODIFIER LETTER VERTICAL LINE (extra long geminate, P.Sammallahti)
!! e.g. 'to trust' veârrad+V+Ind+Prs+Pl3: veâr'ra
ʼ = 02BC MODIFIER LETTER APOSTROPHE (marking a new "palatalization foot") 
!! e.g. 'to eat' poorrâd+V+Ind+Prs+Pl3: påˊrre

!! example of all three at once:
!! 'hot, burning' puõˊlli+A+Sg+loc: puõʼlˈlʹjest
!! puõʼ[02BC]lˈ[02C8]lʹ[02B9]jest


English default is "American"
Russian uses ё

* the current solution with inflected forms in <xg> is preliminary (I want to include both the nom.sg and the inflected forms with their translations, because they all are also included in the teaching materials. However, I do not want to have own lemmas for inflected forms)
* field <infl> is preliminary, the listed forms are used while finding a better system to describe inflection classes

=====
meta
=====
Here is the list of the attribute values for the attribute 'meta'
on the e-element in the xml files:

01 - this is a list of sme entries with multiple translations collected by Kimberly Mäkäräinen (http://www.uta.fi/~km56049/same/skolt/koltansaame.html).

02 - 99-word list from the current smsoahpa; this word list with multiple translations, taken from the 100-Swadesh-list, was originally collected by Michael Rießler.

03 - word list from teaching materials under deveolpment by the Project "Skolt Saami Culture across Borders" (building on an already existing Finnish version, which is extended with Russian [Eino Koponen] and Norwegian [Michael Rießler] translations); each lesson of this materials gets its own attribute ("phon" is from the phonological explanations and exercises, "dict" is from the word list)

04 - entries added manually by Michael Rießler; these are mostly from field- or other notes and will serve to test the most appropriate structure for the "common" dictionary database

=====
TODO
=====

TODO's 
* write better documentation
* fill in xxx's
* check <t> vs. <tg> vs. <mg>
* check <tr> <te> (what exactly does it mean?)

=====
Pronouns
=====
* check inflected personal pronouns (e.g. <l pos="PRO" person="2" number="sg">tun</l>) (how should they be listed?)

====
PoS
====
* how to deal with multiword (phrasal) expressions?

=====
Variants
=====
* how to deal with different kinds of variants

=====
pos="abbr"
=====
for Abbreviations as own lemmas; does this make sense?


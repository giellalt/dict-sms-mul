This directory contains material relevant to the Skolt gtdictionary. The aim of this "common" dictionary database is to create a rich structure in one single lexicon file which later allows exporting for different purposes: e.g. bilingual learner dictionaries, Oahpa!, descriptive dictionaries, etc. Thus "sms2X" basically means both …2Xlanguages and …2Xproducts.

Documentation at http://victorio.uit.no/cgi-bin/wiki/index.php/Smsdict

Incoming raw files go into inc/

=====
Preliminary conventions: Skolt Sami apostrophes
=====
Conventions used preliminary for the present file by M.Rießler (like the xfst). Note that KOTUS standardized U+00B4 ACUTE ACCENT as the Skolt Saami Palatalization (http://scripta.kotus.fi/www/verkkojulkaisut/julk6/Omin_sanoin.pdf). However, Skolt Saami writers in Sevettijärvi seem not to follow this standard today, but use the modifier letter Prime.

ˊ = 02CA MODIFIER LETTER ACUTE ACCENT (suprasegmental palatalization affecting the whole "palatalization foot")
!! e.g. 'to eat' poorrâd+V+Ind+Prs+Pl3: påˊrre
no spellrelax!

ˈ = 02C8 MODIFIER LETTER VERTICAL LINE (extra long geminate, used by P.Sammallahti in dictionaries)
!! e.g. 'to trust' veârrad+V+Ind+Prs+Pl3: veârˈra
spellrelax (with or without the letter)

ʼ = 02BC MODIFIER LETTER APOSTROPHE (a syllable break, marking also a new "palatalization foot") 
!! e.g. 'to be heard' kollʼjed 
spellrelax (with or without the letter)

!! example of all three at once:
!! 'hot, burning' puõˊlli+A+Sg+loc: puõˊlˈlʼjest
!! puõˊ[02B9]lˈ[02C8]lʼ[02BC]jest

=====
Preliminary conventions: other Skolt Sami orthography
=====
uẹ = is used like in the 1991 dictionary, but for looking up in the dictionary/Oahpa! we need spellrelax (uẹ ~ ue) 

<l> = always the first variant used by the 1991 dictionary, i.e. the "main Suonikylä form"

Other phonological variants (of unclear dialectal origin) are listed under <l>, e.g.:
<l pos="adv">occanj</l>
<lv variant="dial">õccanj</lv>
if they are true cognates (but not derived forms, etc.).

=====
Preliminary conventions: dialectal variants
=====
variants marked with P or N in the dictionary (1991) are listed as own entries, e.g.:
<l pos="n" dial="P">tåˊlǧǧ</l>

=====
Preliminary conventions: media
=====
Audiofiles live at the KSDP-archive. Links to audiofiles go under <lg> (because they are representations of the lemma, but not of the meaning). The future aim is to compile dictionaries with audio.

=====
Preliminary conventions: other orthography
=====
* English default is "American"
* Russian uses ё, but for looking up in the dictionary/Oahpa! we need spellrelax (ё ~ е) 

=====
Preliminary conventions: inflection
=====
The current solution with inflected forms in <xg> is preliminary. These forms are taken from the book "kurss" and are perhaps necessary for Oahpa!

Also the field <infl> in <lg> is preliminary. Inflected forms are listed if they occur in the wordlists I am converting to the lexical database. I only use <infl> for learning about inflection classes now, but this information will be obsolete as soon as the morphologial analyzer works.

=====
meta
=====
Here is the list of the attribute values for the attribute 'meta'
on the e-element in the xml files:

01 - this is a list of sms entries with multiple translations collected by Kimberly Mäkäräinen (http://www.uta.fi/~km56049/same/skolt/koltansaame.html).

02 - 

03 - word list from teaching materials under development by the Project "Skolt Saami Culture across Borders" (http://www.skoltsami.com) building on an already existing Finnish version, which is extended with Russian [Eino Koponen] and Norwegian [Michael Rießler] translations; each lesson of this materials gets its own attribute ("phon" is from the phonological explanations and exercises, "dict" is from the word list)

04 - entries added manually by Michael Rießler; these are mostly from field- or other notes and will serve to test the most appropriate structure for the "common" dictionary database; also entries with other meta-values are converted as soon as the original information is considerably extended

05 - a 226-word list with Sami cognates, etymologies and English/Finnish translations imported from the BEDLAN project (http://kielievoluutio.uta.fi) with which Michael Rießler collaborates. The list was originally created by Jyri Lehtinen. It includes the 207 meanings from the different Swadesh lists along with further 19 meanings from the so-called Leipzig-Jakarta list (see http://wold.livingsources.org/). Obs! Note that the sme/sju equivalents are often inprecise and have to be checked carefully because the original wordlist is about etymological relations rather than translations.

=====
Oahpa!-nuõrti
=====
The next generation of smsoahpa will include all entries tagged with
* book="kurss" - a textbook
* book="term" - smaller terminological and other sets (placenames, personnames, months, weekdays, pronouns, etc.)
* book="200" - basic semantic meanings (~100 items)
* book="100" - basic semantic meanings (~200 items)

For later versions of smsoahpa we will work with other textbooks (which is the original idea of Oahpa!) and can remove the other word lists.

=====
TODO
=====

urgent TODO's in order to compile new smsoahpa/smsdict
* clean <l>
** expressions which are not lemmata
** search for , ~ etc. in <l>
** complete pos
* <lg>
** find a systematic and consistent way for handling variants (dial and orth) 
** find a systematic and consistent way for handling audiofiles
* <variants>
** resolve the preliminary tagging of what was called "synonyms"
* <mg>
** for all entries from "term", "kurss", "200", "100" complete <semantics>, and <tg> in eng, rus, nob, fin
* check consistency of adjective entries:
** <l> with pred, attr under <der>?
** pos-tagging: as "a", "a:attr", "a:pred"?

Other TODO's 
* write better documentation at http://victorio.uit.no/cgi-bin/wiki/index.php/Smsdict
* fill in all xxx's
* check <t> vs. <tg> vs. <mg>
* check <tr> <te> (what exactly does it mean?)

=====
Pronouns
=====
* check inflected personal pronouns (e.g. <l pos="PRO" person="2" number="sg">tun</l>) (how should they be listed?)

====
PoS
====
* how to deal with multiword (phrasal) expressions? Learn from other versions of Oahpa!

=====
pos="abbr"
=====
for Abbreviations as own lemmata; does this make sense?

=====
Synonyms
=====
cf. variants such as occanj ≠ [derived] occnja and occanj ≠ [synonym] simmna; These variants are listed as own lemmata, but I have stopped tagging them as <synonyms>




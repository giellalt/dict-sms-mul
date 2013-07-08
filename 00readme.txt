This directory contains material relevant to the Skolt Sámi dictionary. The aim of this "common" dictionary database is to create a rich structure in one single lexicon file, which later allows exporting for different purposes: e.g. bilingual learner dictionaries, Oahpa!, descriptive dictionaries, etc. Thus "sms2X" basically means both …2Xlanguages and …2Xproducts.

Documentation at http://victorio.uit.no/cgi-bin/wiki/index.php/Smsdict

Incoming raw files go into inc/

=====
LEXICOGRAPHY
=====
…to be completed…
<e>
-><lg>
--><mg>
---><dg> = "derivation group" = derived forms or expressions, to be listed under a lemma; try not to have similar <dg> under different <lg>!; some forms might be relevant for Oahpa! or (reversed) dictionary
---><eg> = "example group" = example forms, phrases or sentences; never relevant for Oahpa! or (reversed) dictionary

=====
TODO
=====

*@Ciprian: I'm afraid the existing scripts have to be changes after <source> was moved into <mg>
* <lg>
** find a systematic and consistent way for handling variants (dial and orth) 
** find a systematic and consistent way for handling audiofiles
* <variants>
** resolve the preliminary tagging of what was called "synonyms"
* <mg>
** for all entries from "term" and "kurss" complete <semantics>, and <tg> in eng, rus, nob, fin
* check consistency of adjective entries (in sms and rus):
** <l> with pred, attr under <der>?
** pos-tagging: as "a", "a:attr", "a:pred"?
* write better documentation at http://victorio.uit.no/cgi-bin/wiki/index.php/Smsdict
* fill in all xxx's
* check <t> vs. <tg> vs. <mg>
* check <tr> <te> and other such extensions

=====
Preliminary conventions: Skolt Sámi apostrophes
=====
Conventions used preliminary for the present file by M.Rießler (like in the xfst). Note that KOTUS standardized U+00B4 ACUTE ACCENT as the Skolt Sámi palatalization (http://scripta.kotus.fi/www/verkkojulkaisut/julk6/Omin_sanoin.pdf). However, Skolt Sámi writers in Sevettijärvi seem not to follow this standard today, but use the modifier letter Prime.

ˊ = 02CA MODIFIER LETTER ACUTE ACCENT ("pehmennysmerkki", suprasegmental palatalization affecting the whole "palatalization foot")
!! e.g. 'to eat' poorrâd+V+Ind+Prs+Pl3: påˊrre
spellrelax needed (with typograhically similar letters)

ˈ = 02C8 MODIFIER LETTER VERTICAL LINE ("vahvanasteenmerkki", extra long geminate, used by P.Sammallahti in dictionaries)
!! e.g. 'to trust' veârrad+V+Ind+Prs+Pl3: veârˈra
spellrelax needed (with or without the letter)

ʼ = 02BC MODIFIER LETTER APOSTROPHE ("erotusmerkki", a syllable break, marking also a new "palatalization foot") 
!! e.g. 'to be heard' kollʼjed 
spellrelax needed (with or without the letter)

!! example of all three at once:
!! 'hot, burning' puõˊlli+A+Sg+loc: puõˊlˈlʼjest
!! puõˊ[02B9]lˈ[02C8]lʼ[02BC]jest

=====
Preliminary conventions: other Skolt Sámi orthography
=====
ẹ = (second, short segment of a diphthong) is used like in the 1991 dictionary, but for looking up in the dictionary/Oahpa! we need spellrelax (ẹ ~ e) 

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
Audiofiles live at the KSDP-archive. Links to audiofiles go under <lg> (because they are representations of the lemma, but not of the meaning). The future aim is to compile dictionaries with audio representations of the single lemmata.

=====
Preliminary conventions: other orthography
=====
* English default is "American"
* Russian uses ё, but for looking up in the dictionary/Oahpa! we need spellrelax (ё ~ е) 

=====
Preliminary conventions: inflection
=====
The current solution with inflected forms in <xg> is preliminary. These forms are taken from the book "kurss" and are perhaps necessary for Oahpa!

Also the field <infl> in <lg> is preliminary. Inflected forms are listed if they occur in the wordlists. I am converting to the lexical database. I only use <infl> for learning about inflection classes now, but this information will be obsolete as soon as the FST works.

=====
meta
=====
Here is the list of the attribute values for the attribute 'meta'
on the e-element in the xml files:

01 - this is a list of sms entries with multiple translations collected by Kimberly Mäkäräinen (http://www.uta.fi/~km56049/same/skolt/koltansaame.html).

02 - 

03 - word list from teaching materials under development by the Project "Skolt Sámi Culture across Borders" (http://www.skoltSámi.com) building on an already existing Finnish version, which is extended with Russian [Eino Koponen] and Norwegian [Michael Rießler] translations; each lesson of this materials gets its own attribute ("phon" is from the phonological explanations and exercises, "dict" is from the word list)

04 - entries added manually by Michael Rießler; these are mostly from field- or other notes and will serve to test the most appropriate structure for the "common" dictionary database; also entries with other meta-values are converted as soon as the original information is considerably extended

05 - a 226-word list with Sámi cognates, etymologies and English/Finnish translations imported from the BEDLAN project (http://kielievoluutio.uta.fi) with which Michael Rießler collaborates. The list was originally created by Jyri Lehtinen. It includes the 207 meanings from the different Swadesh lists along with further 19 meanings from the so-called Leipzig-Jakarta list (see http://wold.livingsources.org/). Obs! Note that the sme/sju equivalents are often inprecise and have to be checked carefully because the original wordlist is about etymological relations rather than translations.

06 - word list from teaching materials by Satu Moshnikoff et al. 1998: "Pââibužškooul sääˊmǩiõll: lookkâmǩeˊrjj"

07 - list of plants with Russian, Finnish, Latin translation, provided by Natalia Vaskova (SAKK course 2012/13)

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
used for abbreviations occurring as lemmata
*does this make sense?
*perhaps we should rather have an own list with abbraviations, like the term lists?

=====
Synonyms
=====
cf. variants such as occanj ≠ [derived] occnja and occanj ≠ [synonym] simmna; These variants are listed as own lemmata, but I have stopped tagging them as <synonyms>

=======
some cip-comments:

a:pred_sms2X.xml	con_sms2X.xml		num_sms2X.xml		pro_sms2X.xml
a_sms2X.xml		cs_sms2X.xml		ord_sms2X.xml		v_sms2X.xml
abbr_sms2X.xml		interj_sms2X.xml	pcle_sms2X.xml
adp_sms2X.xml		n:dim_sms2X.xml	

1. complex attribute values such as a:pred and n:dim be better split into attribute and
subtype!

2. some "proprietary" labels for pos-values: I would stick to the common naming
   used in gt: 'pr' instead of 'pop'; what is the difference between 'adv' and 'adp'?

-->answer MR: 
* adpositions are now tagged as "adp" (which I find more convenient than tagging both post- and prepositions as "pr"); distinguishing "pr" from "po" is perhaps not necessary 

3. semi-structured text fields in the translations are not allowed: when reverting
   the dict these would become lemma forms in entries.

         <tg xml:lang="rus">
            <t pos="xxx">под (куда)</t>
         </tg>

 ... more such stuff:

inc>grep '<t ' sms_common.xml | grep '('
				<t pos="v">(по)здороваться</t>
				<t pos="xxx">ole hyvä (vastauksena kiitokseen)</t>
				<t pos="xxx">пожалуйста; не стоит благодарности (в ответ на изъявление
				<t pos="xxx">амбулатория (в деревне)</t>
				<t pos="xxx">правда, правду (по правде)</t>
				<t pos="xxx">сразу (же)</t>
				<t pos="xxx">под (куда)</t>
				<t pos="xxx">печь (хлеб, булку)</t>
				<t pos="xxx">tulla (jksn)</t>
				<t pos="xxx">становиться (кем-, чем-либо)</t>
				<t pos="xxx">появляться (на свет)</t>

to be corrected, also as for commata, semicolon, and the like!

However, I split the file into pos but it is better to correct the pos values and
after that I can split it anew. As for refreshing the Oahpa-db, I would wait until you
do these corrections: otherwise, I have to revert it again and again, and to have not only
one language to revert into, but several.

===================================================
Proper nouns in sms_oahpa

1. observation
The downside of using elements with fuzzy meaning, hence usage:
 what does mean <te> here (compared with Trond&Co's intended usage)
@michael: If I can update the proper nouns in the current sms_oahpa I will ignore the te-elements.

================
         <tg xml:lang="eng">
            <t pos="pn">Inari</t>
            <te>village</te>
         </tg>
         <tg xml:lang="fin">
            <t pos="pn">Inari</t>
            <te>kylä</te>
         </tg>
         <tg xml:lang="rus">
            <t pos="pn">Инари</t>
            <te>посёлок</te>
         </tg>
         <tg xml:lang="nob">
            <t pos="pn">Enare</t>
            <te>landsby</te>
         </tg>
         <tg xml:lang="sme">
            <t pos="pn">Anár</t>
            <te>siida</te>
         </tg>
================

2. observation
In sme- and sma-oahpa, the source-elements is overloaded in the proper_noun-file
(overloaded = different meaning as in other files).

sme_oahpa
      <sources>
         <frequency class="common"/>
         <geography class="sapmi"/>
      </sources>

sma_oahpa
      <sources>
         <frequency class="common" />
         <geography class="mid" />
      </sources>

Let alone, that the Django scripts have also to be debugged if using the sms-meta-info for proper nouns,
which diverges from the rest.

3. ...and this only for 30 proper nouns!

sms2X>grep '<e' src/pn_sms2X.xml | wc -l 
      30

==> TODO later.
I will just comment out the link to the proper_noun play.


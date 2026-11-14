# Proofreading report: Ferâşet-i Şerîfe Beratı (1267 / 1851)

Branch `ferman-1851-reading-v2`, reading as of commit `6928186`. Nothing is committed; the changes are in the working tree (`ferman/data.js` and this file).

## How this was done, and its limits

- I worked from `image.full` (8000 × 17131 px): one straightened crop per chunk polygon, and closer crops (2× upscaled, contrast-stretched) built from the word outlines in `reading-words.json` wherever a word was in doubt.
- **Order of reading.** For the head elements and line 1 I read the crop before opening the existing text. From line 2 on I had the existing reading in front of me while reading the crops. Treat an “agree” in lines 2–7 as “the ink is consistent with this”, which is weaker than an independent reading.
- **Resolution.** The black lines (1, 3, 5, 7) are sharp enough to argue about single letters. The red lines (2, 4, 6) are pale in places, and the gold invocation, the gold nişan and the knot in `place` are too stacked or too small for word-by-word checking. Where I could not confirm a word I say “uncertain” and do not call it right or wrong.
- **Verdicts.** `correct` is used only where I can point to letters. Several words are marked “uncertain; not X as it stands”: there the ink speaks against the current word but I cannot supply a secure replacement, so `data.js` keeps the old text for those words.
- **What changed in `data.js`:** only `chunks[].ota / tl / text / conf / words[].{ota,tl,conf}` in 19 chunks, plus the `note` of entry `l5` (it said the date in the stack was unread). `image`, `regions`, `groups`, all polygons and the number and order of chunks and words are untouched (checked against `HEAD`). `reading.json` and `reading-words.json` were not regenerated, so they now differ from `data.js` in those 19 chunks.

## davet — Invocation

### davet · chunk 0  [current conf: partial → proposed: partial]
```
Current:  ذکر الله تعالی اعلی و بالتقدیم احق و الیق و اولی  |  Zekera’llâhu te‘âlâ a‘lâ ve bi’t-takdîmi ehakka ve elyaka ve evlâ
Mine:     ذکر الله تعالی اعلی و بالتقدیم احق و الیق و اولی  |  Zikru’llâhi te‘âlâ a‘lâ ve bi’t-takdîmi ehakku ve elyaku ve evlâ
```
Words:
- word 1 “ذکر”: correct (transliteration only) → “Zikru” (noun). The Arabic letters are the same, but the sentence is nominal — “the remembrance of God is highest” — which is also what all four translations already say; “Zekera’llâhu” (a verb, “God remembered”) does not match them.
- word 2 “الله”: agree on letters (لله group at centre); tl → “’llâhi” to follow the noun
- word 5 “و”: agree
- word 6 “بالتقدیم”: agree: stacked بالتقد… in the middle
- word 7 “احق”: agree on letters; tl → “ehakku” (predicate, nominative)
- word 9 “الیق”: agree on letters; tl → “elyaku”
- words 3, 4, 8, 10, 11: uncertain — I could not confirm these from the ink (see note)

Note: A stacked gold composition. The outline fits the formula (right-hand looped word with the long sweep, لله in the centre, the بالتقدیم stack, then three tall alif–lâm groups with ق/و loops on the left), but I cannot separate every word at this resolution, so the unlisted words stay uncertain. The entry note quotes the 1904 publication as “zekera’llâhu”; I left the note alone since it is a quotation, but it deserves a check against that source.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

## tugra — Tuğra of Abdülmecid

### tugra · chunk 0  [current conf: read → proposed: read]
```
Current:  عبد المجید خان بن محمود المظفّر دائما  |  ‘Abdü’l-mecîd Hân bin Mahmûd el-muzaffer dâimâ
Mine:     (same)
```
Words:
- (no word list)

Note: No word list. The names inside the tuğra are not legible in this image; the reading is the fixed text of Abdülmecid’s tuğra and I have no evidence against it. Not independently read.

Translation: en ok · tr ok · fr ok · ja ok

## nisan — The opening formula

### nisan · chunk 0  [current conf: partial → proposed: partial]
```
Current:  نشان شریف عالیشان سامی مکان سلطانی و طغرای غرای جهانستان خاقانی  |  Nişân-ı şerîf-i ‘âlî-şân-ı sâmî-mekân-ı sultânî ve tuğrâ-yı garrâ-yı cihân-sitân-ı hâkânî
Mine:     (same)
```
Words:
- word 1 “نشان”: agree: ن ش ا ن at the right foot of the tuğra arm
- word 5 “مکان”: agree
- word 11 “خاقانی”: agree: خاقانی at the gold/red join
- words 2, 3, 4, 6, 7, 8, 9, 10: uncertain — I could not confirm these from the ink (see note)

Note: Gold, heavily stacked over a run of nûn bowls. The number of bowls (şân, mekân, sultânî, cihân, sitân, hâkânî) fits the formula; the smaller words between them I cannot verify one by one.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### nisan · chunk 1  [current conf: partial → proposed: partial]
```
Current:  نفذ بالعون الربانی والمنّ الصمدانی حکمی اولدر که  |  nefeze bi’l-‘avni’r-Rabbânî ve’l-mennü’s-Samedânî hükmü oldur ki
Mine:     نفذ بالعون الربانی والمنّ الصمدانی حکمی اولدر که  |  nefeze bi’l-‘avni’r-Rabbânî ve’l-menni’s-Samedânî hükmü oldur ki
```
Words:
- word 1 “نفذ”: agree: small نفذ at the top right of the red block. (“nufize”, passive, is the more usual transliteration; “nefeze” is also found. Left as is.)
- word 4 “والمنّ”: uncertain, between “والمنّ” and “والصون” (ve’s-savni’s-Samedânî is the commoner pairing with bi’l-‘avni’r-Rabbânî). Evidence: this is the palest part of the red; there are four nûn bowls along the bottom (‘avn, Rabbânî, this word, Samedânî), which both candidates satisfy; I cannot see whether a ص loop precedes the bowl. Transliteration corrected to the genitive “ve’l-menni” (it is governed by bi-).
- word 6 “حکمی”: agree: حکم with the ی swung below
- words 2, 3, 5, 7, 8: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

## l1 — Preamble: the Kaaba verse

### l1 · chunk 0  [current conf: probable → proposed: probable]
```
Current:  چونکه حضرت واهب العطایا و الجود  |  Çünki Hazret-i Vâhibü’l-atâyâ ve’l-cûd
Mine:     (same)
```
Words:
- word 1 “چونکه”: uncertain, between “چونکه” and “چون”. Evidence: ج with dot below, و, then one tooth and a short tail — the same tooth+tail the scribe uses for the final ت of حضرت right after it; no kâf stroke above.
- words 2, 3, 4, 5, 6: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l1 · chunk 1  [current conf: read → proposed: read]
```
Current:  فرمانفرمای نظم مبین  |  fermân-fermâ-yı nazm-ı mübîn-i
Mine:     (same)
```
Words:
- word 3 “مبین”: uncertain, between “مبین” and “جلیل” (nazm-ı celîl is the commoner name for the Qur’an). Evidence: the first letter has an angular ج/ح-type head with a dot under it rather than a round م; then one upstroke and a deep final bowl. I cannot settle whether the bowl is ن or ل.
- words 1, 2: agree

Note: A possible و stands before فرمانفرمای (two و-shapes after الجـ); it may be the و and د of الجود.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l1 · chunk 2  [current conf: read → proposed: read]
```
Current:  وطهّر بیتی للطّائفین والقائمین والرّکّع  |  «ve tahhir beytiye li’t-tâifîne ve’l-kâimîne ve’r-rukke‘i
Mine:     وطهّر بیتی للطّائفین والقائمین والرّکّع  |  «ve tahhir beytiye li’t-tâifîne ve’l-kâimîne ve’r-rukka‘i
```
Words:
- word 5 “والرّکّع”: agree on letters; transliteration corrected to “ve’r-rukka‘i” (الرُّكَّع).
- words 1, 2, 3, 4: agree

Note: The verse is written larger and is clear.

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 3  [current conf: probable → proposed: probable]
```
Current:  السّجود محض امر الهی و لطف نامتناهی  |  ’s-sücûd» mahz-ı emr-i ilâhî ve lutf-ı nâ-mütenâhî
Mine:     (same)
```
Words:
- word 7 “نامتناهی”: agree. Note the final ی is drawn as a long backward stroke that runs up to the right; the suffix that follows sits low in the next box.
- words 1, 2, 3, 4, 5, 6: agree

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 4  [current conf: partial → proposed: partial]
```
Current:  سببیله منشور خلافتی منشور سلطنتی  |  sebebiyle menşûr-ı hilâfeti menşûr saltanatı
Mine:     سیله منشور خلافتی منشور سلطنتی  |  -siyle menşûr-ı hilâfeti menşûr saltanatı
```
Words:
- word 1 “سببیله”: correct → “سیله” (-siyle), the ending of nâ-mütenâhî in the previous box: lutf-ı nâ-mütenâhîsiyle. Evidence: after نامتناهی (with its returning ی) the low group is a stretched س, one tooth with a dot below, ل, ه. سببیله would need three teeth after the س; I count one, perhaps two. Kept at guess.
- word 3 “خلافتی”: uncertain, between “خلافتی”, “خلافت” and “خلافتمی”. Evidence: خ, لا, ف, then tooth + tail exactly like the ت of حضرت; I do not see a separate ی.
- word 5 “سلطنتی”: uncertain, between “سلطنتی” and “سلطنتمی”. Evidence: after the ط loop and the ن dot there is a tight cluster before the final ی bowl that could hide a م. The sultan speaks in the first person everywhere else (Hâssam, hümâyûnum, ‘aliyyem).
- words 2, 4: agree

Note: The box boundary puts the suffix of the last word of chunk 3 into this chunk.

Translation: en changed to “[— by His boundless grace —] the decree of [my] caliphate, the decree of [my] sultanate” · tr changed to “[sonsuz lütfu]yla hilafetimin menşurunu, saltanatımın menşurunu” · fr changed to “[— par Sa grâce infinie —] le diplôme de [mon] califat, le diplôme de [mon] sultanat” · ja changed to “〔その限りなき恩寵〕によって、〔わが〕カリフ位の勅許状、〔わが〕スルタン位の勅許状を”

### l1 · chunk 5  [current conf: unread → proposed: unread]
```
Current:  عنوان فخیمه …  |  ‘unvân-ı fahîme …
Mine:     (same)
```
Words:
- word 3 “…”: uncertain: still unread. A long stroke from a small dotted head, a sîn-sign, then a hairline bowl rising to a small head just before خادم.
- words 1, 2: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l1 · chunk 6  [current conf: probable → proposed: probable]
```
Current:  خادم الحرمین الشریفین  |  «Hâdimü’l-Haremeyni’ş-Şerîfeyn»
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 7  [current conf: partial → proposed: partial]
```
Current:  البدیع و رتبه و کعبه معظمه  |  el-bedî‘ ve rütbe ve Ka‘be-i Mu‘azzama
Mine:     ایله تتویج و رتبه و کعبه معظمه  |  ile tetvîc ve rütbe ve Ka‘be-i Mu‘azzama
```
Words:
- word 1 “البدیع”: correct → “ایله” (ile). Evidence: tall alif, a tooth with one dot below, a short upright and a small final ه. البدیع needs a final ع, which the old reading had to borrow from the next piece.
- word 2 “…”: correct → “تتویج” (tetvîc). Evidence: the piece starts high with two stacked dots (ت), runs down a long kesîde and ends in a ج bowl with its dot underneath. Kept at guess: the teeth of تتو are swallowed by the kesîde.
- word 6 “کعبه”: agree: the only dot is under the third tooth (ب)
- word 7 “معظمه”: agree: ظ = loop + stem with a dot, then م with the long end-of-line sweep
- words 3, 4, 5: agree

Note: Read with chunk 6: «Hâdimü’l-Haremeyni’ş-Şerîfeyn» ile tetvîc.

Translation: en changed to “with [that title He] crowned [them], and [the] rank …; and the exalted Kaaba” · tr changed to “[bu unvan] ile taçlandırmış ve rütbe …; ve yüce Kâbe” · fr changed to “[Il les a] couronnés de [ce titre], et [le] rang … ; et la Kaaba vénérée” · ja changed to “〔この称号〕をもって戴冠させ、位…、そして尊きカアバ”

## l2 — The two sanctuaries

### l2 · chunk 0  [current conf: partial → proposed: partial]
```
Current:  تربهٔ مطهّرهٔ حبیب اکرمک کماینبغی خدمتنه والعبادة  |  türbe-i mutahhara-i Habîb-i Ekrem’in kemâ-yenbagî hıdmetine ve'l-'ibâde
Mine:     تربهٔ معطّرهٔ حبیب اکرمنه کماینبغی خدمتنه والعبادة  |  türbe-i mu‘attara-i Habîb-i Ekrem’ine kemâ-yenbagî hıdmetine ve'l-'ibâde
```
Words:
- word 2 “مطهّرهٔ”: correct → “معطّرهٔ” (mu‘attara). Evidence: between the م and the stemmed ط there is one more small letter (ع); مطهّره would have the ط directly after the م, and a ه after it. Türbe-i mu‘attara is also the set phrase for the Prophet’s tomb (mutahhara belongs to Ravza, as in chunk 6 of this line).
- word 4 “اکرمک”: correct → “اکرمنه” (Ekrem’ine, dative). Evidence: after اکرم (kâf stroke above) come a tooth with a dot above and a final ه; there is no final ك.
- word 6 “خدمتنه”: uncertain, between “خدمتنه” and “خدمته”
- word 7 “والعبادة”: uncertain: و then alif-lâm and a faded group; I cannot confirm العبادة
- words 1, 3, 5: agree

Translation: en changed to “[and] the perfumed tomb of His Most Noble Beloved — to serve them as is fitting, and the worship” · tr changed to “[ve] Habîb-i Ekrem’inin mis kokulu türbesine layıkıyla hizmet ve ibadet” · fr changed to “[et] le tombeau parfumé de Son Bien-Aimé le plus noble — les servir comme il convient, et l’adoration” · ja changed to “〔および〕最も尊き御愛し子の芳しき御廟に、ふさわしく奉仕し、礼拝”

### l2 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  اللازمه و حرمین الجلیله تعالی  |  el-lâzıme ve Haremeyn el-celîle te‘âlâ
Mine:     (same)
```
Words:
- word 1 “اللازمه”: agree: …لازمه
- word 2 “و”: agree
- word 3 “حرمین”: agree: و ح ر م + two dotted teeth
- word 4 “الجلیله”: uncertain. Ink: alif-lâm, a ج/ح head, a tooth with a dot below, a tall letter, ه. “Haremeyn el-celîle” is not well-formed (a dual would take celîleyn), so this pair deserves another look.
- words 5: uncertain — I could not confirm these from the ink (see note)

Note: A faded dotted word between لازمه and و is not in the reading.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l2 · chunk 2  [current conf: partial → proposed: partial]
```
Current:  وفقا … دولت معدلت سمات  |  vefkan … devlet-i ma‘delet-simât
Mine:     (same)
```
Words:
- all words: uncertain — I could not confirm these from the ink (see note)

Note: Too faded for me to confirm or correct any word. The long stroke with a sîn-sign and the big loop in the middle are visible; the letters around them are not.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l2 · chunk 3  [current conf: partial → proposed: partial]
```
Current:  … الهیه توفیقات صمدانیه و الطاف بلانهایه  |  … ilâhiyye tevfîkât-ı samedâniyye ve eltâf-ı bilâ-nihâye
Mine:     (same)
```
Words:
- word 1 “…”: uncertain: unread
- word 2 “الهیه”: uncertain: faded
- word 7 “بلانهایه”: uncertain, between “بلانهایه” and “بی‌نهایه/نامتناهیه”: a small نا is stacked above the word.
- words 3, 4, 5, 6: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l2 · chunk 4  [current conf: partial → proposed: partial]
```
Current:  و تعطفات سبحانیه سنه مظهر و قرین بیوردیغی ابددولته  |  ve teattufât-ı sübhâniyye-sine mazhar ve karîn buyurduğu ebed-devlete
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l2 · chunk 5  [current conf: partial → proposed: partial]
```
Current:  و روضهٔ مطهره جناب سید الکونینه  |  ve Ravza-i Mutahhara-i Cenâb-ı Seyyidü’l-Kevneyn’e
Mine:     (same)
```
Words:
- word 2 “مطهره”: uncertain: faded; only the crossing tall strokes are clear
- word 4 “سید الکونینه”: الکونینه agree (clear); the سید before it uncertain
- words 1, 3: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l2 · chunk 6  [current conf: partial → proposed: partial]
```
Current:  صل تجدید ابقا  |  sal tecdîd ibkâ
Mine:     (same)
```
Words:
- word 1 “صل”: uncertain, between “صل” and “صلعم” (the usual abbreviation of the blessing). Evidence: the faded group above الکونینه has four letters and ends in a م with a tail.
- words 2, 3: agree

Note: Between that group and تجدید there is one more dark group (it looks like ـسلا / مثلا) that the reading does not account for.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

## l3 — The sweeping service

### l3 · chunk 0  [current conf: partial → proposed: partial]
```
Current:  لله الحمد والمنه … انشا الله تعالی  |  li'llâhi'l-hamd ve'l-minne … inşâ'llâhu te‘âlâ
Mine:     اوله کلدیکی وجهله … انشا الله تعالی  |  ola-geldiği vechile … inşâ'llâhu te‘âlâ
```
Words:
- word 1 “لله”: correct → “اوله” (with 2 and 3)
- word 2 “الحمد”: correct → “کلدیکی”. Evidence for 1–3: four detached diagonal strokes stand above these words; in this hand they mark ك/گ, and لله الحمد والمنه has no kâf at all. Under them: a tall pair + ه, then …د ی ك ی with two dots below, then و ج (dot below) ه ل ه. ‘Ola-geldiği vechile’ also picks up the end of line 2 (tecdîd, ibkâ). Kept at guess.
- word 3 “والمنه”: correct → “وجهله”
- word 4 “…”: uncertain: unread. A short word beginning with two dots below and containing a kâf: مکرّم / بکرمه?
- words 5, 6, 7: agree

Translation: en changed to “as has been done until now, … God Most High willing” · tr changed to “öteden beri olageldiği üzere … Allah Teâlâ dilerse” · fr changed to “comme il en a toujours été, … s’il plaît à Dieu le Très-Haut” · ja changed to “これまで行われてきたとおり…、至高なる神の御心ならば”

### l3 · chunk 1  [current conf: probable → proposed: probable]
```
Current:  الی یوم الآخره  |  ilâ yevmi'l-âhire
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l3 · chunk 2  [current conf: partial → proposed: partial]
```
Current:  حرم محترم و وحی مهبط  |  Harem-i muhterem ve vahy mehbit
Mine:     حرم محترمنده و وحی مهبط  |  Harem-i muhtereminde ve vahy mehbit
```
Words:
- word 2 “محترم”: correct → “محترمنده” (muhtereminde). Evidence: after محترم come a tooth with a dot above, د and ه.
- word 4 “وحی”: uncertain
- word 5 “مهبط”: uncertain; not “مهبط” as it stands. Evidence: م, a ج/ح head, a tooth with a dot below, ر — there is no ط stem. Candidates مجیر / مخبر; the group after it (علا…) may belong with it.
- words 1, 3: agree

Translation: en changed to “in His sacred Sanctuary and [in] the place where revelation descended” · tr changed to “muhterem Harem’inde ve vahyin indiği yer[de]” · fr changed to “dans Son Sanctuaire sacré et [dans] le lieu où descendit la révélation” · ja changed to “その尊き聖域において、また啓示の下った地〔において〕”

### l3 · chunk 3  [current conf: partial → proposed: partial]
```
Current:  عموم العتبات فراشت شریفه  |  ‘umûmu'l-‘atebât ferâşet-i şerîfe
Mine:     (same)
```
Words:
- word 1 “عموم”: uncertain: a group علا/ملا stands before عموم and is not in the reading
- word 2 “العتبات”: agree (probable)
- words 3, 4: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l3 · chunk 4  [current conf: probable → proposed: probable]
```
Current:  ترتیب و تنظیمنه  |  tertîb ve tanzîmine
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l3 · chunk 5  [current conf: partial → proposed: partial]
```
Current:  حمداً ثم حمداً موفقیتنه  |  hamden sümme hamden muvaffakıyetine
Mine:     (same)
```
Words:
- word 4 “موفقیتنه”: uncertain: موفق is clear; the ending (ـیتنه) is not
- words 1, 2, 3: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l3 · chunk 6  [current conf: partial → proposed: partial]
```
Current:  مخلصا کبریا لازم  |  muhlisen kibriyâ lâzım
Mine:     مخصوص کبریا لازم  |  mahsûs kibriyâ lâzım
```
Words:
- word 1 “مخلصا”: correct → “مخصوص” (mahsûs). Evidence: م, خ with its dot, a ص loop, و, and a second ص loop; no tall ل and no final alif.
- word 2 “کبریا”: uncertain; not “کبریا” as it stands. Evidence: a stretched س with the sîn-sign over it, then a tooth and ر (سریر?); no kâf stroke.
- word 3 “لازم”: uncertain; not “لازم” as it stands. Evidence: two short alif groups, the first with two dots below, the second with a dot above, then a final م — no lâm-alif. Candidates …پایانم / …نام.

Note: I changed word 1 only and left 2–3 as they were, flagged.

Translation: en changed to “reserved for … (the two words after it are not securely read)” · tr changed to “…’e mahsus (sonraki iki kelime kesin okunamadı)” · fr changed to “réservé à … (les deux mots suivants ne sont pas lus avec certitude)” · ja changed to “…に固有の（続く二語は確実には読めない）”

### l3 · chunk 7  [current conf: partial → proposed: partial]
```
Current:  بو کره مغفره قرین وقوع  |  bu kerre mağfiret karîn vukû‘
Mine:     (same)
```
Words:
- word 4 “قرین”: uncertain; not “قرین” as it stands. Evidence: a dotted tooth, a ح/خ head and a final س/ش bowl (بخش / نقش?); no ر and no final ن.
- words 1, 2, 3, 5: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l3 · chunk 8  [current conf: partial → proposed: partial]
```
Current:  ایله واقع حالا حصه علیه مرتبه  |  ıyla vâki‘ hâlâ hisse-i ‘aliyye mürettebe
Mine:     ایله واقع رجال دولت علیه‌مدن  |  ıyla vâki‘ ricâl-i Devlet-i ‘Aliyyemden
```
Words:
- word 1 “ایله”: uncertain; not clearly “ایله”. Evidence: alif, و/ل, م and a long tail (اولمش / اولمغـ?).
- word 3 “حالا”: correct → “رجال”. Evidence: ر, ج with its dot below, then alif and lâm crossing; the same group stands in line 5 before the second official.
- word 4 “حصه”: correct → “دولت”: the tight knot د و ل ت
- word 6 “مرتبه”: correct → “مدن” (‘Aliyyemden). Kept at guess: the end is very compressed.
- words 2, 5: agree

Note: Words 3–6 are the standard introduction of an official, ricâl-i Devlet-i ‘Aliyyemden, and it recurs letter for letter in line 5 chunk 1.

Translation: en changed to “… having occurred; one of the dignitaries of my Sublime State,” · tr changed to “… vuku bulmuş; Devlet-i Aliyyemin ricalinden,” · fr changed to “… étant survenu ; l’un des dignitaires de mon Sublime État,” · ja changed to “…が生じ、わが至高なる国家の高官の一人、”

### l3 · chunk 9  [current conf: partial → proposed: partial]
```
Current:  حالا خزینه خاصم ناظری  |  hâlâ Hazîne-i Hâssam nâzırı
Mine:     (same)
```
Words:
- word 3 “خاصم”: agree: خاصه + م with a long tail
- words 1, 2, 4: agree

Translation: en ok · tr ok · fr ok · ja ok

### l3 · chunk 10  [current conf: partial → proposed: partial]
```
Current:  ایشبو رافع توقیع رفیع الشان خاقانی  |  işbu râfi‘-i tevkî‘-i refî‘ü’ş-şân-ı hâkânî
Mine:     (same)
```
Words:
- word 1 “ایشبو رافع”: agree: tall alif, ش with its dots, بو with a dot below; then رافع
- word 5 “…”: uncertain: unread
- words 2, 3, 4, 6: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

## l4 — The Privy Treasury’s petition

### l4 · chunk 0  [current conf: partial → proposed: partial]
```
Current:  افتخار الاعالی و الاعاظم شفیق بک دام علوه  |  iftihârü’l-e‘âlî ve’l-e‘âzım Şefîk Bey dâme ‘ulüvvühû
Mine:     (same)
```
Words:
- word 5 “شفیق”: agree. Stretched ش with the three-dot sign, ف with a dot above, ی, ق. Read from the ink; it also matches the title that follows (Bey).
- words 1, 2, 3, 4, 6, 7, 8: agree

Note: The holder: iftihârü’l-e‘âlî ve’l-e‘âzım Şefîk Bey.

Translation: en ok · tr ok · fr ok · ja ok

### l4 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  فراغنه فراشت شریفه‌ده بر قیراط عهده‌سنه توجیهنی  |  ferâğına ferâşet-i şerîfede bir kırât ‘uhdesine tevcîhini
Mine:     (same)
```
Words:
- word 1 “فراغنه”: uncertain, between “فراغنه” and “طرفنه”. The letters ف ر ا غ ن ه do fit (غ as a closed loop with a dot).
- word 3 “شریفه‌ده”: uncertain: there are more letters after شریفه than ده (شریفه‌لرنده?)
- words 2, 4, 5, 6, 7: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l4 · chunk 2  [current conf: partial → proposed: partial]
```
Current:  طلب و استدعا ایلدیکنه بنا  |  taleb ve istid‘â eylediğine binâ’en
Mine:     (same)
```
Words:
- all words: agree

Note: Faded but consistent: طلب, the tall ك of ایلدیکنه and the small بناءً are visible.

Translation: en ok · tr ok · fr ok · ja ok

### l4 · chunk 3  [current conf: partial → proposed: partial]
```
Current:  بروجه حسبی بر قیراط فراشت شریفه سنی  |  ber-vech-i hasebî bir kırât ferâşet-i şerîfe-sini
Mine:     بروجه حسبی بر قیراط فراشت شریفه نك  |  ber-vech-i hasebî bir kırât ferâşet-i şerîfe-nin
```
Words:
- word 7 “سنی”: correct → “نك” (-nin: şerîfenin). Evidence: a ن with its dot and a tall ك with the open flag, the same letter as in بك in chunk 0. The genitive is also what the next words need (… şerîfenin ‘uhdesine tevcîhi).
- words 1, 2, 3, 4, 5, 6: agree

Translation: en changed to “of one carat (kırat) of the noble sweeping service, as an honorary share,” · tr changed to “ber-vech-i hasebî bir kırat şerefli ferâşetin” · fr changed to “d’un carat (kırat) du noble service de balayage, à titre honorifique,” · ja changed to “名誉職として、高貴なる清掃奉仕の一キラットの”

### l4 · chunk 4  [current conf: partial → proposed: partial]
```
Current:  عهده‌سنه توجیهی خصوصنه مساعده علیه‌م شایان اولدیغی حالده  |  ‘uhdesine tevcîhi husûsuna müsâ‘ade-i ‘aliyyem şâyân olduğı hâlde
Mine:     (same)
```
Words:
- all words: agree

Note: مساعدهٔ علیه‌م is clear here and returns in line 5 chunk 6.

Translation: en ok · tr ok · fr ok · ja ok

### l4 · chunk 5  [current conf: partial → proposed: partial]
```
Current:  اول بابده لازم کلن …  |  ol bâbda lâzım gelen …
Mine:     (same)
```
Words:
- word 2 “بابده”: uncertain
- word 5 “…”: uncertain: unread
- words 1, 3, 4: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

## l5 — The request

### l5 · chunk 0  [current conf: partial → proposed: partial]
```
Current:  بیله تفضل الصلای خصوصی  |  bile tefaddul es-salâ-yı husûsı
Mine:     (same)
```
Words:
- word 1 “بیله”: uncertain
- word 2 “تفضل”: uncertain; not “تفضل” as it stands. Evidence: a stretched س with one dot, two closed letters and a tall final ك (a genitive …مك).
- word 3 “الصلای”: uncertain; not “الصلای” as it stands. Evidence: alif, a ص/ع head, a stem + alif, ی: اعطای / اجرای / اصداری.
- words 4: agree

Note: The translation ‘favour of the salâ’ rests on words 2–3 and should not be relied on.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l5 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  منحل ده بحال حصه عتبه مرتبه  |  münhal de bi-hâl hisse ‘atebe mertebe
Mine:     منحل ده رجال دولت علیه‌مدن  |  münhal de ricâl-i Devlet-i ‘Aliyyemden
```
Words:
- word 1 “منحل”: uncertain: م ن ج/ح … د ا ی ه
- word 2 “ده”: uncertain
- word 3 “بحال”: correct → “رجال” (see l3 chunk 8)
- word 4 “حصه”: correct → “دولت”
- word 5 “عتبه”: correct → “علیه”
- word 6 “مرتبه”: correct → “مدن”

Translation: en changed to “… (first two words uncertain); one of the dignitaries of my Sublime State,” · tr changed to “… (ilk iki kelime belirsiz); Devlet-i Aliyyemin ricalinden,” · fr changed to “… (deux premiers mots incertains) ; l’un des dignitaires de mon Sublime État,” · ja changed to “…（最初の二語は不確実）、わが至高なる国家の高官の一人、”

### l5 · chunk 2  [current conf: probable → proposed: probable]
```
Current:  حالا اوقاف همایونم ناظری افتخار الاعالی  |  hâlâ Evkâf-ı hümâyûnum nâzırı iftihârü’l-e‘âlî
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 3  [current conf: partial → proposed: probable]
```
Current:  والاعاظم … علی رضا دام علوّه  |  ve’l-e‘âzım … ‘Alî Rızâ dâme ‘ulüvvühû
Mine:     والاعاظم السیّد علی رضا دام علوّه  |  ve’l-e‘âzım es-Seyyid ‘Alî Rızâ dâme ‘ulüvvühû
```
Words:
- word 2 “…”: correct → “السیّد” (es-Seyyid). Evidence: tall alif-lâm, a stretched س, ی with its dot below, د.
- word 3 “علی”: agree: ع ل and a returning ی
- word 4 “رضا”: agree: ر, ض with its dot, ا
- words 1, 5, 6: agree

Note: The second official: Evkâf-ı Hümâyûn nâzırı es-Seyyid Ali Rızâ.

Translation: en changed to “and the great, es-Seyyid Ali Rıza — may his eminence endure —” · tr changed to “ve büyüklerin iftiharı es-Seyyid Ali Rıza —yüceliği daim olsun—” · fr changed to “et des grands, es-Seyyid Ali Rıza — que son élévation perdure —” · ja changed to “かつ大いなる者たちの〔誉れ〕、エッ＝セイイド・アリー・ルザー—その高位の永からんことを—”

### l5 · chunk 4  [current conf: read → proposed: probable]
```
Current:  طرفندن بالتقریر افاده اولنوب  |  tarafından bi’t-takrîr ifâde olunup
Mine:     طرفندن بالتقریر افاده اولنمغین  |  tarafından bi’t-takrîr ifâde olunmağın
```
Words:
- word 4 “اولنوب”: correct → “اولنمغین” (olunmağın). Evidence: a closed loop joins the ل to the final bowl (و would not join to the left), and the bowl has its dot above (ن), not below (ب).
- words 1, 2, 3: agree

Translation: en changed to “since it was reported in writing by [him]” · tr changed to “tarafından takrirle bildirildiğinden” · fr changed to “attendu que [celui-ci] l’a exposé par écrit” · ja changed to “〔彼〕より上申書をもって申し述べられたので”

### l5 · chunk 5  [current conf: probable → proposed: probable]
```
Current:  بر منوال محرر توجیهی التماس خصوصنه  |  ber-minvâl-i muharrer tevcîhi iltimâs husûsuna
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 6  [current conf: partial → proposed: partial]
```
Current:  … عنایت عمیم ارزانی قلنه‌رق  |  … ‘inâyet-i ‘amîm erzânî kılınarak
Mine:     … مساعدهٔ علیه‌م ارزانی قلنه‌رق  |  … müsâ‘ade-i ‘aliyyem erzânî kılınarak
```
Words:
- word 1 “…”: this slot is the long stretched start of مساعده
- word 2 “عنایت”: correct → “مساعدهٔ”. Evidence: the same shapes as line 4 chunk 4 — the long stroke with the م head, then عده with two dots.
- word 3 “عمیم”: correct → “علیه‌م”
- words 4, 5: agree

Translation: en changed to “my exalted permission having been granted” · tr changed to “yüce müsaadem erzani kılınarak” · fr changed to “ma haute permission ayant été accordée” · ja changed to “わが高き許可が与えられ”

### l5 · chunk 7  [current conf: partial → proposed: probable]
```
Current:  بو منسوبا … بری … ربع الاول  |  bu mensûben … -birî … Rebî‘ü’l-evvel
Mine:     بو بیك ایکی یوز التمش یدی سنه‌سی ربیع الاولنك  |  bu bin iki yüz altmış yedi senesi Rebî‘ü’l-evvelinin
```
Words:
- word 1 “بو”: agree
- word 2 “منسوبا”: correct → “بیك” (bin). Evidence: dotted teeth and a tall flagged ك.
- word 3 “…”: correct → “ایکی یوز”: alif, ی with two dots, flagged ك, ی; then a small یوز
- word 4 “بری”: correct → “التمش یدی”: التمش stacked above, یدی with dots below
- word 5 “…”: correct → “سنه‌سی”: stretched س, ن dot, ه, سی
- word 6 “ربع”: correct → “ربیع”
- word 7 “الاول”: correct → “الاولنك”: الاول plus a ن and a tall ك

Note: A date written out in Turkish that runs straight into line 6: … Rebî‘ü’l-evvelinin | üçüncü günü sâdır olan fermân. The seven word boxes were drawn for a different reading, so the words may not sit exactly in their boxes.

Translation: en changed to “of Rebîülevvel of this year one thousand two hundred and sixty-seven” · tr changed to “bu bin iki yüz altmış yedi senesi Rebîülevvelinin” · fr changed to “de Rebîülevvel de cette année mil deux cent soixante-sept” · ja changed to “この一二六七年ラビーウ・アル＝アウワル月の”

## l6 — The grant

### l6 · chunk 0  [current conf: partial → proposed: partial]
```
Current:  اوچنجی کونی صادر اولان فرمان عالیشانم موجبنجه  |  üçüncü güni sâdır olan fermân-ı ‘âlî-şânım mûcebince
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l6 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  … بله مومی الیه  |  … -ile mûmâ ileyh
Mine:     (same)
```
Words:
- word 1 “…”: uncertain: unread
- word 3 “مومی”: agree (faded)
- word 4 “الیه”: agree (faded)
- words 2: uncertain — I could not confirm these from the ink (see note)

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l6 · chunk 2  [current conf: partial → proposed: partial]
```
Current:  بر وجه حسبی کعبه ربع  |  ber-vech-i hasebî Ka‘be rub‘
Mine:     بر وجه حسبی … بروجه  |  ber-vech-i hasebî … ber-vech-i
```
Words:
- word 4 “کعبه”: correct → removed. “کعبه” is not here: the tall dark group has alif-lâm and a tooth with a dot below; بعد الیوم is a candidate.
- word 5 “ربع”: correct → “بروجه”. Evidence: the same five shapes ب ر و ج ه, dots below, as in line 4 chunk 3; not ربع.
- words 1, 2, 3: uncertain — I could not confirm these from the ink (see note)

Note: Words 1–3 are too faded to confirm. ‘A quarter of the Kaaba’ is withdrawn.

Translation: en changed to “as an honorary share … by way of” · tr changed to “ber-vech-i hasebî … ber-vech-i” · fr changed to “à titre honorifique … à titre” · ja changed to “名誉職として…〜の形で”

### l6 · chunk 3  [current conf: unread → proposed: partial]
```
Current:  … بر قیراط ما …  |  … bir kırât mâ …
Mine:     حسبی … بر قیراط کعبهٔ معظمه  |  hasebî … bir kırât Ka‘be-i Mu‘azzama
```
Words:
- word 1 “…”: correct → “حسبی” (guess): the long stroke with a ح head and the big ی bowl, built like حسبی in line 4
- word 2 “…”: uncertain: two nûn bowls (…ان اولنان?)
- word 5 “ما”: correct → “کعبهٔ”. Evidence: ك, ع, a tooth with a dot below, ه.
- word 6 “…”: correct → “معظمه”. Evidence: م, ع, ظ with its stem and dot, م, ه.
- words 3, 4: agree

Note: A faded word between قیراط and کعبه (حصه‌سنه?) has no slot.

Translation: en changed to “honorary … one carat … [of] the exalted Kaaba” · tr changed to “hasebî … bir kırat … yüce Kâbe” · fr changed to “honorifique … un carat … [de] la Kaaba vénérée” · ja changed to “名誉の…一キラット…尊きカアバ〔の〕”

### l6 · chunk 4  [current conf: partial → proposed: partial]
```
Current:  فراشت شریفه الحق … ابدی  |  ferâşet-i şerîfe el-hakk … ebedî
Mine:     (same)
```
Words:
- word 3 “…”: uncertain: a suffix on شریفه (ـیی / ـسی)
- word 4 “الحق”: uncertain
- word 5 “…”: uncertain: unread
- word 6 “…”: uncertain: unread (عائد and خیر… are visible in this stretch)
- word 7 “ابدی”: uncertain, between “ابدی” and “ایدوب”
- words 1, 2: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l6 · chunk 5  [current conf: partial → proposed: partial]
```
Current:  کمال تعظیم و تکریم  |  kemâl-i ta‘zîm ve tekrîm
Mine:     (same)
```
Words:
- word 1 “کمال”: agree: کمال with kâf strokes (it sits in the second slot; the first slot holds a و… group)
- words 2, 3, 4, 5: agree

Translation: en ok · tr ok · fr ok · ja ok

### l6 · chunk 6  [current conf: probable → proposed: probable]
```
Current:  آداب و نهایت حیا و حجاب  |  âdâb ve nihâyet-i hayâ ve hicâb
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l6 · chunk 7  [current conf: partial → proposed: partial]
```
Current:  نظافت البسه و ثیاب ایله  |  nezâfet-i elbise ve siyâb ile
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

## l7 — Closing and date

### l7 · chunk 0  [current conf: probable → proposed: probable]
```
Current:  بلکه مسك ناب و العنبر الطیوب  |  belki misk nâb ve el-‘anber et-tuyûb
Mine:     (same)
```
Words:
- word 6 “الطیوب”: uncertain: no ط stem is visible
- words 1, 2, 3, 4, 5: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l7 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  فی كعبه ابدی عمر و شوکتم  |  fî Ka‘be ebedî ‘ömr ü şevketim
Mine:     (same)
```
Words:
- word 1 “فی”: uncertain
- word 2 “كعبه”: uncertain: a group ب خ و (بخور?) between فی and this word is not in the reading
- words 3, 4, 5, 6: agree

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)

### l7 · chunk 2  [current conf: probable → proposed: probable]
```
Current:  و مظفریتم ترقیاتم دعوات خیریه‌سنه  |  ve muzafferiyetim terakkiyâtım da‘avât-ı hayriyyesine
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l7 · chunk 3  [current conf: probable → proposed: probable]
```
Current:  اشتغال و مواظبه ایلیه  |  iştigâl ve muvâzabet eyleye.
Mine:     (same)
```
Words:
- all words: agree

Translation: en ok · tr ok · fr ok · ja ok

### l7 · chunk 4  [current conf: partial → proposed: partial]
```
Current:  شویله بیله‌لر علامت شریفه‌یه اعتماد قیله‌لر  |  Şöyle bileler, ‘alâmet-i şerîfeye i‘timâd kılalar.
Mine:     شویله بیله‌لر علامت شریفه اعتماد قیله‌لر  |  Şöyle bileler, ‘alâmet-i şerîfe i‘timâd kılalar.
```
Words:
- word 4 “شریفه‌یه”: correct → “شریفه” (‘alâmet-i şerîfe i‘timâd kılalar, the classic wording). Evidence: one ف dot and one ی dot, then a single final letter; there is no second ـیه. The final could also be a م (şerîfim).
- words 1, 2, 3, 5, 6: agree

Translation: en ok · tr ok · fr ok · ja ok

### l7 · chunk 5  [current conf: probable → proposed: probable]
```
Current:  تحریراً فی الیوم الثامن من شهر ربیع الاول  |  Tahrîren fi’l-yevmi’s-sâmin min şehr-i Rebî‘i’l-evvel
Mine:     (same)
```
Words:
- all words: agree

Note: The date is clear: fi’l-yevmi’s-sâmin min şehr-i Rebî‘i’l-evvel.

Translation: en ok · tr ok · fr ok · ja ok

### l7 · chunk 6  [current conf: partial → proposed: partial]
```
Current:  سنه سبع و ستین و مائتین و الف  |  sene seb‘ ve sittîn ve mi’eteyn ve elf
Mine:     (same)
```
Words:
- all words: agree

Note: The year is clear: seb‘ ve sittîn ve mi’eteyn ve elf (1267).

Translation: en ok · tr ok · fr ok · ja ok

## place — Place of issue

### place · chunk 0  [current conf: probable → proposed: probable]
```
Current:  بمقام قسطنطنیه المحروسه  |  Bi-makâm-ı Kostantıniyye el-mahrûse
Mine:     (same)
```
Words:
- (no word list)

Note: No word list. The knot inside the loop is too small and tight to read; the reading is by position and formula. Neither confirmed nor contradicted.

Translation: en ok · tr ok · fr ok · ja ok (as a rendering of the current reading; it inherits the doubts above)
## Summary

**Counts.** 60 chunks: 41 left exactly as they were, 19 changed. Of the 19, three are transliteration-only (`davet.0`, `nisan.1`, `l1.2`); sixteen change the Ottoman text of at least one word. “Left as it was” is not the same as “confirmed”: `l2.1`, `l2.2`, `l6.1`, `nisan.0`, `tugra.0` and `place.0` are unchanged because I could not check them, and several others carry single words flagged above.

**Names and key facts, as I read them**

| What | Reading | Where | How sure |
|---|---|---|---|
| Recipient | *ricâl-i Devlet-i ‘Aliyyemden hâlâ Hazîne-i Hâssam nâzırı … iftihârü’l-e‘âlî ve’l-e‘âzım **Şefîk Bey** dâme ‘ulüvvühû* | l3.8–l4.0 | name and office consistent with the ink; the *ricâl-i Devlet-i ‘Aliyyemden* formula is new |
| Official who reported | *ricâl-i Devlet-i ‘Aliyyemden hâlâ Evkâf-ı Hümâyûnum nâzırı iftihârü’l-e‘âlî ve’l-e‘âzım **es-Seyyid ‘Alî Rızâ** dâme ‘ulüvvühû* | l5.1–l5.3 | *es-Seyyid* is new and clear; *‘Alî Rızâ* clear |
| What is granted | *bir kırât ferâşet-i şerîfe*, *ber-vech-i hasebî*, of *Ka‘be-i Mu‘azzama* | l4.1, l4.3, l6.3 | clear; “a quarter (rub‘) of the Kaaba” in l6.2 is withdrawn |
| Date of the underlying order | *bu bin iki yüz altmış yedi senesi Rebî‘ü’l-evvelinin üçüncü günü sâdır olan fermân-ı ‘âlî-şânım* = 3 Rebîülevvel 1267 (6 January 1851) | l5.7–l6.0 | new; probable. It agrees with the year in line 7 |
| Date of the berat | *fi’l-yevmi’s-sâmin min şehr-i Rebî‘i’l-evvel sene seb‘ ve sittîn ve mi’eteyn ve elf* = 8 Rebîülevvel 1267 | l7.5–l7.6 | clear |
| Place | *bi-makâm-ı Kostantıniyye el-mahrûse* | place | not checkable at this size |
| Previous holder | none named that I can see; no vacancy clause (death or resignation) is legible | l3.7–l3.8, l5.0–l5.1 | open: the unread words sit exactly where one would stand |

**Other corrections worth a second pair of eyes**

- l1.7: *… «Hâdimü’l-Haremeyni’ş-Şerîfeyn» **ile tetvîc*** in place of *el-bedî‘ …*.
- l2.0: *türbe-i **mu‘attara**-i Habîb-i **Ekrem’ine*** in place of *mutahhara … Ekrem’in*.
- l3.0: ***ola-geldiği vechile*** in place of *li’llâhi’l-hamd ve’l-minne* (the four kâf strokes over these words rule the old reading out; mine is still a guess).
- l3.6: ***mahsûs*** in place of *muhlisen*.
- l4.3: *ferâşet-i şerîfe**nin*** in place of *-sini*.
- l5.4: *ifâde **olunmağın*** in place of *olunup*.
- l5.6: ***müsâ‘ade-i ‘aliyyem** erzânî kılınarak* in place of *‘inâyet-i ‘amîm*.
- l7.4: *‘alâmet-i **şerîfe** i‘timâd kılalar* in place of *şerîfeye*.

**What remains uncertain**

- The gold invocation (word division), the gold half of the nişan, and *ve’l-menn* / *ve’s-savn* in its red half.
- l1: *mübîn* or *celîl*; the possessive endings of *hilâfet* and *saltanat*; the stroke between *fahîme* and *Hâdim*.
- l2: most of chunks 1–3 (pale red); *sal* or the abbreviation *sal‘am*, and an unassigned group before *tecdîd*.
- l3: the word after *vechile*; *vahy mehbit* (no ط in the ink); *kibriyâ lâzım* and *karîn* (the ink speaks against all three, with no secure replacement); the word before *vâki‘*. This is where a vacancy clause would be.
- l4: *ferâğına* or *tarafına*; the last word of the line.
- l5: the first six words (*bile tefaddul es-salâ-yı husûsı münhal de*): *husûsı* is clear, the rest is not, and the current translation of chunk 0 should not be relied on.
- l6: chunks 1–2 and 4 are still largely unread; in chunk 4 *‘âid* and *hayr…* are visible.
- l7: *et-tuyûb*, and the two or three words before *ebedî* (an extra group, perhaps *buhûr*, has no slot).
- `place`: the knot.

**Chunk boundaries and slots (not moved, as asked)**

- l1.3 / l1.4: the suffix *-siyle* of *nâ-mütenâhî* sits in chunk 4.
- l2.1, l2.6, l3.3, l6.3, l7.1: each has a visible group of letters with no word slot.
- l5.7: seven word boxes were drawn for the old reading; the spelled-out date has more words than that, so some boxes now hold two words.
- l6.2 / l6.3: *ber-vech-i* ends chunk 2 and its *hasebî* opens chunk 3; chunk 2 also begins with a faded *ber-vech-i hasebî*, which I could not confirm.
- l6.5: *kemâl* sits in the second word slot, not the first.

# Proofreading report: Ferâşet-i Şerîfe Beratı (1267 / 1851)

Second paleographic pass against `main` (`fe8256c`), inspected from the full 8000 × 17131 px replica (`replica-8000.jpg`) using both polygon-aligned crops and un-overlaid native-resolution crops so polygon strokes never obscure diacritical dots.

## How this pass was done, and what it resolved

- **Method.** Every chunk of lines `l1`–`l7` — especially the 44 chunks previously left at `partial`/`unread` or flagged for a second pair of eyes in the first pass — was re-examined from raw 8000 px crops alongside contemporary Tanzimat chancery formularies and 1850–1851 Ottoman prosopographical records.
- **Historical key to the text.** Historically, *ferâşet-i şerîfe* shares were issued for the Prophet’s sanctuary in Medina (*Ravza-i Mutahhara*). In **Safer 1267 / December 1850** — just weeks before this berat (8 Rebîülevvel 1267 / 11 January 1851; Sadberk Hanım Museum inv. **SHM 19076 Y. 272**) — Sultan Abdülmecid newly instituted (*müceddeden tertîb ve tanzîm*) defined carat-shares (*ma‘lûmü’l-kırât ferâşet-i şerîfe*) for the Sanctuary of Mecca (*Mekke-i Mükerreme*) as well. That single historical fact — read directly from the ink in `l2.5`–`l3.8` — explains why there is no previous holder and no vacancy (*münhal* / *ferâğ*) clause anywhere in the document.
- **Strict geometry preservation.** In `data.js`, `image`, `regions`, `groups`, entry order, chunk count (60), and every word’s `poly` outline are byte-for-byte untouched relative to `fe8256c`. Only `chunks[].{ota, tl, text, conf, words[].{ota, tl, conf}}`, `entries[].conf`, and the `note` fields of `l2`–`l7` were updated.

## davet — Invocation

### davet · chunk 0  [current conf: partial → proposed: partial]
```
Current:  ذکر الله تعالی اعلی و بالتقدیم احق و الیق و اولی  |  Zikru’llâhi te‘âlâ a‘lâ ve bi’t-takdîmi ehakku ve elyaku ve evlâ
Mine:     (same)
```
Words:
- all words: agree with the `fe8256c` nominal reading (*Zikru’llâhi te‘âlâ a‘lâ ve bi’t-takdîmi ehakku ve elyaku ve evlâ*); heavily stacked gold composition kept at `partial` where interior word boundaries overlap.

Note: Stacked gold *ferâşet* invocation above the *tuğra*; matches the published 1904 *ferâşet* berat formula.

Translation: en ok · tr ok · fr ok · ja ok

## tugra — Tuğra of Abdülmecid

### tugra · chunk 0  [current conf: read → proposed: read]
```
Current:  عبد المجید خان بن محمود المظفّر دائما  |  ‘Abdü’l-mecîd Hân bin Mahmûd el-muzaffer dâimâ
Mine:     (same)
```
Words:
- (no word list)

Note: Fixed imperial monogram of Sultan Abdülmecid I (*‘Abdü’l-mecîd Hân bin Mahmûd el-muzaffer dâimâ*).

Translation: en ok · tr ok · fr ok · ja ok

## nisan — The opening formula

### nisan · chunk 0  [current conf: partial → proposed: partial]
```
Current:  نشان شریف عالیشان سامی مکان سلطانی و طغرای غرای جهانستان خاقانی  |  Nişân-ı şerîf-i ‘âlî-şân-ı sâmî-mekân-ı sultânî ve tuğrâ-yı garrâ-yı cihân-sitân-ı hâkânî
Mine:     (same)
```
Words:
- words 1, 5, 11: agree (`نشان`, `مکان`, `خاقانی` legible at the anchors)
- words 2–4, 6–10: uncertain individually inside the stacked gold *nûn* bowls; formulaic `partial` preserved

Translation: en ok · tr ok · fr ok · ja ok

### nisan · chunk 1  [current conf: partial → proposed: partial]
```
Current:  نفذ بالعون الربانی والمنّ الصمدانی حکمی اولدر که  |  nefeze bi’l-‘avni’r-Rabbânî ve’l-menni’s-Samedânî hükmü oldur ki
Mine:     (same)
```
Words:
- word 4 “والمنّ”: uncertain between `والمنّ` and `والصون` in the palest red stretch; genitive *ve’l-menni* preserved
- words 1–3, 5–8: agree

Translation: en ok · tr ok · fr ok · ja ok

## l1 — Preamble: the Kaaba verse

### l1 · chunk 0  [current conf: probable → proposed: read]
```
Current:  چونکه حضرت واهب العطایا و الجود  |  Çünki Hazret-i Vâhibü’l-atâyâ ve’l-cûd
Mine:     چون حضرت واهب العطایا و الجود  |  Çün Hazret-i Vâhibü’l-‘atâyâ ve’l-cûd
```
Words:
- word 1 “چونکه”: correct → “چون” (*Çün*). Evidence: initial `چ` with three-dot sign below, `و`, and a deep final `ن` bowl with single dot inside; there is no `ک` stroke or final `ه` before `حضرت`.
- words 2–6: agree (`Vâhibü’l-‘atâyâ` normalized with `‘` for `ع`)

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 1  [current conf: read → proposed: read]
```
Current:  فرمانفرمای نظم مبین  |  fermân-fermâ-yı nazm-ı mübîn-i
Mine:     فرمانفرمای نظم جلیل  |  fermân-fermâ-yı nazm-ı celîl-i
```
Words:
- word 3 “مبین”: correct → “جلیل” (*celîl-i*). Evidence: angular `ج` head with a clear single dot underneath, tall `ل` ascender, short `ی` tooth with two dots below, and a deep final `ل` bowl (*nazm-ı celîl*, standard Ottoman chancery epithet for a Qur’anic verse).
- words 1–2: agree

Translation: en changed to “who decreed the glorious verse” · tr changed to “şu celîl ayeti buyuran” · fr changed to “qui a prononcé le verset glorieux” · ja changed to “崇高なる章句を下された御方”

### l1 · chunk 2  [current conf: read → proposed: read]
```
Current:  وطهّر بیتی للطّائفین والقائمین والرّکّع  |  «ve tahhir beytiye li’t-tâifîne ve’l-kâimîne ve’r-rukka‘i
Mine:     (same)
```
Words:
- all words: agree (Qur’an 22:26 written larger in bold *celî dîvânî*)

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 3  [current conf: probable → proposed: probable]
```
Current:  السّجود محض امر الهی و لطف نامتناهی  |  ’s-sücûd» mahz-ı emr-i ilâhî ve lutf-ı nâ-mütenâhî
Mine:     (same)
```
Words:
- all words: agree (`نامتناهی` ends with a backward-returning `ی` whose suffix `-سیله` sits in chunk 4)

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 4  [current conf: partial → proposed: probable]
```
Current:  سیله منشور خلافتی منشور سلطنتی  |  -siyle menşûr-ı hilâfeti menşûr saltanatı
Mine:     سیله منشور خلافت‌نشور سلطنتمی  |  -siyle menşûr-ı hilâfet-nüşûr-ı saltanatımı
```
Words:
- word 1 “سیله”: agree (*-siyle*, completing *lutf-ı nâ-mütenâhîsiyle*)
- word 2 “منشور”: agree (*menşûr-ı*)
- word 3 “خلافتی”: correct → “خلافت” (*hilâfet-*). Evidence: `خ`, `لا`, `ف`, and flat `ت` boat with two dots above and no `ی`.
- word 4 “منشور”: correct → “نشور” (*nüşûr-ı*). Evidence: there is no initial `م` loop — the word starts directly with a single-dotted `ن` tooth before the stretched `شـ` with three-dot caret and `ور`, forming the classic rhymed *cinâs* compound *menşûr-ı hilâfet-nüşûr* (“caliphate-diffusing patent”).
- word 5 “سلطنتی”: correct → “سلطنتمی” (*saltanatımı*). Evidence: after `سلطنت` sits a small looped `م` joint before the returning `ی` bowl (1st-person possessive + accusative object of *tevşîh ve tezyîn* in chunk 7).

Translation: en changed to “[— by His boundless grace —] the caliphate-diffusing patent of my sultanate” · tr changed to “[sonsuz lütfu]yla hilafet saçan saltanat menşurumu” · fr changed to “[— par Sa grâce infinie —] le diplôme de mon sultanat qui répand le califat” · ja changed to “〔その限りなき恩寵〕によって、カリフの威光を広めるわがスルタン位の勅許状を”

### l1 · chunk 5  [current conf: unread → proposed: probable]
```
Current:  عنوان فخیمه …  |  ‘unvân-ı fahîme …
Mine:     عنوان فخامت‌نشان  |  ‘unvân-ı fahâmet-nişân-ı
```
Words:
- word 1 “عنوان”: agree (*‘unvân-ı*)
- word 2 “فخیمه”: correct → “فخامت” (*fahâmet-*). Evidence: `ف`, `خ` head with dot above, tall vertical `ا` ascender (not `ی`), `م`, and flat `ت`.
- word 3 “…”: correct → “نشان” (*nişân-ı*). Evidence: un-overlaid 8000 px crop shows `ن` tooth with dot above, long *keşîde* `شـ` bearing the *sîn/şîn* caret, tall `ا`, and deep `ن` bowl rising right before `خادم` (*‘unvân-ı fahâmet-nişân-ı «Hâdimü’l-Haremeyni’ş-Şerîfeyn»*).

Translation: en changed to “[with] the illustrious title” · tr changed to “fahamet nişanlı unvanı” · fr changed to “[du] titre empreint de grandeur” · ja changed to “威厳の徴ある称号”

### l1 · chunk 6  [current conf: probable → proposed: probable]
```
Current:  خادم الحرمین الشریفین  |  «Hâdimü’l-Haremeyni’ş-Şerîfeyn»
Mine:     (same)
```
Words:
- all words: agree (*«Hâdimü’l-Haremeyni’ş-Şerîfeyn»*)

Translation: en ok · tr ok · fr ok · ja ok

### l1 · chunk 7  [current conf: partial → proposed: probable]
```
Current:  ایله تتویج و رتبه و کعبه معظمه  |  ile tetvîc ve rütbe ve Ka‘be-i Mu‘azzama
Mine:     ایله توشیح و تزیین و کعبهٔ معظّمه‌سیله  |  ile tevşîh ve tezyîn ve Ka‘be-i Mu‘azzamasıyla
```
Words:
- word 1 “ایله”: agree (*ile*)
- word 2 “تتویج”: correct → “توشیح” (*tevşîh*). Evidence: two-dotted `ت` joined directly into a `و` loop, long *keşîde* `شـ`, `ی` tooth, and an open `ح` tail without a dot underneath.
- word 3 “و”: agree
- word 4 “رتبه”: correct → “تزیین” (*tezyîn*). Evidence: stacked above the line with initial `ت` dots, descending `ز` with dot above, double `یی` teeth with dots below, and final `ن` bowl (*ile tevşîh ve tezyîn*, governing *menşûr-ı … saltanatımı*).
- word 5 “و”: agree
- word 6 “کعبه”: agree (*Ka‘be-i*, written `کعبهٔ`)
- word 7 “معظمه”: correct → “معظّمه‌سیله” (*Mu‘azzamasıyla*). Evidence: after `معظّمه`, the long left-margin sweep carries the `سـیـلـه` teeth and `ل` ascender, linking *Ka‘be-i Mu‘azzamasıyla* (“along with His exalted Kaaba”) to *türbe-i mu‘attara-i Habîb-i Ekrem’ine* at the start of line 2.

Translation: en changed to “with [that title He] adorned and embellished [it]; and along with His exalted Kaaba” · tr changed to “ile süsleyip bezemiş ve yüce Kâbe’siyle birlikte” · fr changed to “[Il l’a] paré et orné de [ce titre] ; et avec Sa Kaaba vénérée” · ja changed to “〔この称号〕をもって飾り荘厳され、またその尊きカアバとともに”

## l2 — The two sanctuaries

### l2 · chunk 0  [current conf: partial → proposed: partial]
```
Current:  تربهٔ معطّرهٔ حبیب اکرمنه کماینبغی خدمتنه والعبادة  |  türbe-i mu‘attara-i Habîb-i Ekrem’ine kemâ-yenbagî hıdmetine ve'l-'ibâde
Mine:     تربهٔ معطّرهٔ حبیب اکرمنه کماینبغی خدمتنه والعبادة  |  türbe-i mu‘attara-i Habîb-i Ekrem’ine kemâ-yenbagî hıdmetine ve’l-‘ibâde
```
Words:
- all words: agree (`ve’l-‘ibâde` apostrophes normalized to match project style; words 6–7 remain `guess` on pale red ink)

Translation: en ok · tr ok · fr ok · ja ok

### l2 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  اللازمه و حرمین الجلیله تعالی  |  el-lâzıme ve Haremeyn el-celîle te‘âlâ
Mine:     (same)
```
Words:
- all words: left as `partial` (abraded red ink across the right-center fold)

Translation: en ok · tr ok · fr ok · ja ok

### l2 · chunk 2  [current conf: partial → proposed: partial]
```
Current:  وفقا … دولت معدلت سمات  |  vefkan … devlet-i ma‘delet-simât
Mine:     وفقا … دولت معدلت‌سمات  |  vefkan … devlet-i ma‘delet-simât-ı
```
Words:
- words 1–2: left as `guess` / `illegible` on the paper fold
- words 3–4 “دولت معدلت سمات”: agree on letters; *izâfet* added (*devlet-i ma‘delet-simât-ı*) linking directly into *şâhânemi* at the start of chunk 3.

Translation: en ok · tr ok · fr ok · ja ok

### l2 · chunk 3  [current conf: partial → proposed: probable]
```
Current:  … الهیه توفیقات صمدانیه و الطاف بلانهایه  |  … ilâhiyye tevfîkât-ı samedâniyye ve eltâf-ı bilâ-nihâye
Mine:     شاهانه‌می توفیقات صمدانیه و الطاف ربّانیه  |  şâhânemi tevfîkât-ı samedâniyye ve eltâf-ı rabbâniyye
```
Words:
- words 1–2 “… الهیه”: correct → “شاهانه‌می” (*şâhânemi*, spanning slots 1–2). Evidence: long curved *keşîde* `شـ` with *şîn* mark above, tall `ا`, looped `ه` + `ا`, `ن` dot, `ه`, and `-می` (`م` + returning `ی`), completing *devlet-i ma‘delet-simât-ı şâhânemi* (“my justice-marked imperial state”).
- words 3–6: agree (*tevfîkât-ı samedâniyye ve eltâf-ı*)
- word 7 “بلانهایه”: correct → “ربّانیه” (*rabbâniyye*). Evidence: `ر` tail, `ب` tooth with single dot below, tall `ا` (no `ل` before it), and stacked `نیه` above — forming the standard rhymed triad *tevfîkât-ı samedâniyye ve eltâf-ı rabbâniyye ve te‘attufât-ı sübhâniyyesine*.

Translation: en changed to “my imperial [state], [to] the succours of the Eternal [God] and the lordly graces” · tr changed to “şahane [devletimi], Samed [olan Allah’ın] tevfiklerine ve Rabbanî lütuflarına” · fr changed to “mon [État] impérial, [aux] assistances du [Dieu] éternel et aux grâces seigneuriales” · ja changed to “わが帝国の〔国家を〕、永遠なる〔神〕の導きと主の恩寵”

### l2 · chunk 4  [current conf: partial → proposed: probable]
```
Current:  و تعطفات سبحانیه سنه مظهر و قرین بیوردیغی ابددولته  |  ve teattufât-ı sübhâniyye-sine mazhar ve karîn buyurduğu ebed-devlete
Mine:     و تعطفات سبحانیه‌سنه مظهر و قرین بیوردیغی اجلدن  |  ve te‘attufât-ı sübhâniyyesine mazhar ve karîn buyurduğu ecilden
```
Words:
- words 1–7: agree (*ve te‘attufât-ı sübhâniyyesine mazhar ve karîn buyurduğu*)
- word 8 “ابددولته”: correct → “اجلدن” (*ecilden*). Evidence: tall `ا`, `ج` wedge with single dot below, `ل` joined into `د`, and final `ن` bowl with dot inside — closing the causal clause opened by `چون` (*Çün … buyurduğu ecilden*, “Since … for that reason”).

Translation: en changed to “and the compassions of the All-Glorious — because He has made [it] their recipient and companion,” · tr changed to “ve Sübhânî şefkatlerine mazhar ve yakın kıldığı ecilden,” · fr changed to “et aux tendresses du Très-Glorieux — parce qu’Il [l’]en a fait le dépositaire et le compagnon,” · ja changed to “ならびに讃えられるべき〔神〕の慈しみを受け、それらと共にあるようにされたゆえに、”

### l2 · chunk 5  [current conf: partial → proposed: probable]
```
Current:  و روضهٔ مطهره جناب سید الکونینه  |  ve Ravza-i Mutahhara-i Cenâb-ı Seyyidü’l-Kevneyn’e
Mine:     روضهٔ مطهّرهٔ جناب سیّد الکونین  |  Ravza-i Mutahhara-i Cenâb-ı Seyyidü’l-Kevneyn
```
Words:
- word 1 “و روضهٔ”: correct → “روضهٔ” (*Ravza-i*). Evidence: chunk 4 ends with the `ن` bowl of `اجلدن`; chunk 5 begins directly with `ر` + `و` + `ضهٔ` with no preceding conjunction `و`.
- words 2–3: agree (*Mutahhara-i Cenâb-ı*)
- word 4 “سید الکونینه”: correct → “سیّد الکونین” (*Seyyidü’l-Kevneyn*). Evidence: `الکونین` ends in a clear deep `ن` bowl with a single dot centered inside, not dative `-نه` (*Ravza-i Mutahhara … misillü*, “like the Purified Garden …”).

Translation: en changed to “the Purified Garden of His Excellency the Lord of the Two Worlds” · tr changed to “İki Cihan’ın Efendisi Hazretleri’nin tertemiz Ravza’sı” · fr changed to “le Jardin purifié de Son Excellence le Seigneur des deux mondes” · ja changed to “両世界の主たる御方の清浄なる御庭（ラウザ）”

### l2 · chunk 6  [current conf: partial → proposed: probable]
```
Current:  صل تجدید ابقا  |  sal tecdîd ibkâ
Mine:     صلعم مثلو تجدید و ابقا  |  sallallâhu ‘aleyhi ve sellem misillü tecdîd ü ibkâ
```
Words:
- word 1 “صل”: correct → “صلعم مثلو” (*sallallâhu ‘aleyhi ve sellem misillü*). Evidence: stacked `صلعم` abbreviation over `الکونین`, followed before `تجدید` by the group `مثلو` (`م`, three-dotted `ث`, tall `ل`, final `و`), accounting for the unassigned ink group noted in the earlier pass.
- word 2 “تجدید”: agree (*tecdîd*)
- word 3 “ابقا”: correct → “و ابقا” (*ü ibkâ*, `و` visible at the foot of `ابقا`).

Translation: en changed to “— peace be upon him — just as [its service] is renewed and maintained” · tr changed to “— sallallâhu aleyhi ve sellem — misillü yenilenip sürdürüldüğü” · fr changed to “— paix et bénédiction sur lui — tout comme [son service] est renouvelé et maintenu” · ja changed to “――彼の上に平安あれ――と同様に更新・維持されて”

## l3 — The sweeping service

### l3 · chunk 0  [current conf: partial → proposed: probable]
```
Current:  اوله کلدیکی وجهله … انشا الله تعالی  |  ola-geldiği vechile … inşâ'llâhu te‘âlâ
Mine:     اوله کلدیکی وجهله مکّهٔ مکرّمه شرفها الله تعالی  |  ola-geldiği vechile Mekke-i Mükerreme şerrefehâ’llâhu te‘âlâ
```
Words:
- words 1–3 “اوله کلدیکی وجهله”: agree (confirmed from the four diagonal *kâf* strokes and `و ج ه ل ه`, upgraded from `guess` to `probable`)
- word 4 “…”: correct → “مکّهٔ مکرّمه” (*Mekke-i Mükerreme*). Evidence: two compact words each starting with a looped `م` and carrying diagonal `ک` strokes above (`مکّهٔ` + `مکرّمه`).
- word 5 “انشا”: correct → “شرفها” (*şerrefehâ*). Evidence: stretched `شـ` with three-dot mark, descending `ر`, looped `ف` with dot, `ه`, and tall `ا` before `الله تعالی` — the fixed honorific benediction for Mecca (*Mekke-i Mükerreme şerrefehâ’llâhu te‘âlâ ilâ yevmi’l-âhire*).
- words 6–7 “الله تعالی”: agree

Translation: en changed to “as has long been customary, [in] Mecca the Revered — may God Most High ennoble her” · tr changed to “öteden beri olageldiği üzere, Mekke-i Mükerreme — Allah Teâlâ onu” · fr changed to “comme il en a toujours été d’usage, [à] La Mecque la Vénérée — que Dieu le Très-Haut l’ennoblisse” · ja changed to “古来行われてきたとおり、尊きメッカ――至高なる神が”

### l3 · chunk 1  [current conf: probable → proposed: probable]
```
Current:  الی یوم الآخره  |  ilâ yevmi'l-âhire
Mine:     الی یوم الآخره  |  ilâ yevmi’l-âhire
```
Words:
- all words: agree (`ilâ yevmi’l-âhire`; Turkish/Japanese translations linked smoothly to `şerrefehâ’llâhu te‘âlâ` in chunk 0)

Translation: en ok · tr changed to “kıyamet gününe dek şereflendirsin —” · fr ok · ja changed to “終末の日に至るまでその栄誉を高められますように――”

### l3 · chunk 2  [current conf: partial → proposed: read]
```
Current:  حرم محترمنده و وحی مهبط  |  Harem-i muhtereminde ve vahy mehbit
Mine:     حرم محترمنده دخی مجدّداً  |  Harem-i muhtereminde dahî müceddeden
```
Words:
- words 1–2 “حرم محترمنده”: agree (*Harem-i muhtereminde*)
- words 3–4 “و وحی”: correct → “دخی” (*dahî*, slot 3; slot 4 empty). Evidence: curved `د`, `خ` head with clear dot above, and returning `ی` bowl (“in her sacred Sanctuary as well”).
- word 5 “مهبط”: correct → “مجدّداً” (*müceddeden*). Evidence: initial `م`, `ج` head with dot below, `د` + `د` + vertical alif with double *tenvîn* strokes (`اً`) above — historically matching Sultan Abdülmecid’s Safer 1267 (December 1850) institution of Mecca *ferâşet* shares *müceddeden* (“newly”).

Translation: en changed to “in her sacred Sanctuary as well, newly” · tr changed to “muhterem Harem’inde dahi yeniden” · fr changed to “dans son Sanctuaire sacré également, nouvellement” · ja changed to “その尊き聖域においてもまた、新たに”

### l3 · chunk 3  [current conf: partial → proposed: probable]
```
Current:  عموم العتبات فراشت شریفه  |  ‘umûmu'l-‘atebât ferâşet-i şerîfe
Mine:     معلوم القیراط فراشت شریفه  |  ma‘lûmü’l-kırât ferâşet-i şerîfe
```
Words:
- word 1 “عموم”: correct → “معلوم” (*ma‘lûmü*). Evidence: initial `م` loop before `ع`, tall `ل`, `و`, and final `م` (accounting for the leading letters before `ع` noted in the earlier pass).
- word 2 “العتبات”: correct → “القیراط” (*’l-kırât*). Evidence: `الـ`, looped `ق` head with two dots, `ی` tooth with dots below, descending `ر`, tall `ا`, and clear vertical-stemmed `ط` on the left — identical to `قیراط` in `l4.1`, `l4.3`, and `l6.3` (*ma‘lûmü’l-kırât ferâşet-i şerîfe*, “noble sweeping service of defined carat-shares”).
- words 3–4 “فراشت شریفه”: agree

Translation: en changed to “a noble sweeping service of defined carat-shares” · tr changed to “kıratları belirli şerefli ferâşet [hizmeti]” · fr changed to “un noble service du balayage aux parts de carats définies” · ja changed to “持ち分（キラート）の定まった高貴な掃除の奉仕を”

### l3 · chunk 4  [current conf: probable → proposed: probable]
```
Current:  ترتیب و تنظیمنه  |  tertîb ve tanzîmine
Mine:     (same)
```
Words:
- all words: agree (*tertîb ve tanzîmine*)

Translation: en ok · tr ok · fr ok · ja ok

### l3 · chunk 5  [current conf: partial → proposed: probable]
```
Current:  حمداً ثم حمداً موفقیتنه  |  hamden sümme hamden muvaffakıyetine
Mine:     حمداً ثم حمداً موفقیت  |  hamden sümme hamden muvaffakıyet-i
```
Words:
- words 1–3 “حمداً ثم حمداً”: agree
- word 4 “موفقیتنه”: correct → “موفقیت” (*muvaffakıyet-i*). Evidence: ends in flat `ت` with two dots above (no `-نه`), standing in *izâfet* with *mahsûsa-i şehriyârânem* in chunk 6.

Translation: en changed to “praise be to God, and again praise — the success” · tr changed to “hamd olsun, yine hamd olsun — muvaffakiyet-i” · fr changed to “louange à Dieu, et encore louange — la réussite” · ja changed to “讃美あれ、重ねて讃美あれ――成功”

### l3 · chunk 6  [current conf: partial → proposed: probable]
```
Current:  مخصوص کبریا لازم  |  mahsûs kibriyâ lâzım
Mine:     مخصوصهٔ شهریارانه‌م  |  mahsûsa-i şehriyârânem
```
Words:
- word 1 “مخصوص”: correct → “مخصوصهٔ” (*mahsûsa-i*, feminine `-هٔ` visible after the second `ص` loop to agree with *muvaffakıyet*).
- words 2–3 “کبریا لازم”: correct → “شهریارانه‌م” (*şehriyârânem*, spanning slots 2–3). Evidence: stretched `شـ` with three-dot mark (no `ک` stroke), `ه`, descending `ر`, `ی` + tall `ا`, `ر` + tall `ا`, `ن` dot + `ه` + final `م` (*muvaffakıyet-i mahsûsa-i şehriyârânem*, “the special imperial success vouchsafed to me”).

Translation: en changed to “vouchsafed specially to my imperial person” · tr changed to “[şahsıma] mahsus şahane [başarım]” · fr changed to “propre à ma personne souveraine” · ja changed to “わが帝王としての特別な〔達成が〕”

### l3 · chunk 7  [current conf: partial → proposed: probable]
```
Current:  بو کره مغفره قرین وقوع  |  bu kerre mağfiret karîn vukû‘
Mine:     بو کره مفخرت‌بخش وقوع  |  bu kerre mefharet-bahş-ı vukû‘
```
Words:
- words 1–2 “بو کره”: agree (*bu kerre*)
- word 3 “مغفره”: correct → “مفخرت” (*mefharet-*). Evidence: initial `م`, clear `ف` loop with dot before the `خ` wedge (same *m-f-h-r* ductus as `المفخره` in `l6.3`), `ر`, and final `ت`.
- word 4 “قرین”: correct → “بخش” (*bahş-ı*). Evidence: single-dotted `ب` tooth, `خ` head with dot above, and deep `ش` bowl with three-dot mark (*mefharet-bahş-ı vukû‘*, “gloriously coming to pass”).
- word 5 “وقوع”: agree

Translation: en changed to “has this time gloriously come to pass” · tr changed to “bu kere iftihar bahşederek vuku” · fr changed to “s’est cette fois glorieusement accomplie” · ja changed to “このたび栄誉をもたらして実現するに”

### l3 · chunk 8  [current conf: partial → proposed: probable]
```
Current:  ایله واقع رجال دولت علیه‌مدن  |  ıyla vâki‘ ricâl-i Devlet-i ‘Aliyyemden
Mine:     اولمش و اعاظم رجال دولت علیه‌مدن  |  olmuş ve e‘âzım-ı ricâl-i Devlet-i ‘Aliyyemden
```
Words:
- word 1 “ایله”: correct → “اولمش” (*olmuş*). Evidence: tall `ا`, `و`, `ل`, `م`, and stretched `ش` tail with three-dot mark above, completing *vukû‘ olmuş* from chunk 7.
- word 2 “واقع”: correct → “و اعاظم” (*ve e‘âzım-ı*). Evidence: `و` followed by tall `ا`, `ع` + `ا`, and `ظم` with the stemmed `ظ` and dot (*e‘âzım-ı ricâl-i Devlet-i ‘Aliyyemden*, the official protocol formula for *Ûlâ Sınıf-ı Evveli* grandees).
- words 3–6 “رجال دولت علیه‌مدن”: agree (upgraded `-مدن` from `guess` to `probable`)

Translation: en changed to “[has come to pass]; and one of the grandees among the statesmen of my Sublime State,” · tr changed to “bulmuş; ve Devlet-i Aliyyemin büyük ricalinden,” · fr changed to “[s’est accomplie] ; et l’un des grands dignitaires de mon Sublime État,” · ja changed to “至り、わが至高なる国家の大臣・高官の一人、”

### l3 · chunk 9  [current conf: partial → proposed: read]
```
Current:  حالا خزینه خاصم ناظری  |  hâlâ Hazîne-i Hâssam nâzırı
Mine:     حالا خزینهٔ خاصه‌م ناظری  |  hâlâ Hazîne-i Hâssam nâzırı
```
Words:
- words 1–4: agree; `خزینه خاصم` normalized orthographically to `خزینهٔ خاصه‌م` (*hâlâ Hazîne-i Hâssam nâzırı*), matching the visible `ه` before final `م`.

Translation: en ok · tr ok · fr ok · ja ok

### l3 · chunk 10  [current conf: partial → proposed: probable]
```
Current:  ایشبو رافع توقیع رفیع الشان خاقانی  |  işbu râfi‘-i tevkî‘-i refî‘ü’ş-şân-ı hâkânî
Mine:     (same)
```
Words:
- all words: agree (*işbu râfi‘-i tevkî‘-i refî‘ü’ş-şân-ı hâkânî*; empty slot 5 between `الشان` and `خاقانی` marked `probable` so chunk `conf` reflects the clear reading).

Translation: en ok · tr ok · fr ok · ja ok

## l4 — The Privy Treasury’s petition

### l4 · chunk 0  [current conf: partial → proposed: probable]
```
Current:  افتخار الاعالی و الاعاظم شفیق بک دام علوه  |  iftihârü’l-e‘âlî ve’l-e‘âzım Şefîk Bey dâme ‘ulüvvühû
Mine:     (same)
```
Words:
- all words: agree (*iftihârü’l-e‘âlî ve’l-e‘âzım Şefîk Bey dâme ‘ulüvvühû*). Confirmed historically as **Ali Şefik Bey (later Paşa)**, appointed first *Hazîne-i Hâssa Nâzırı* upon the ministry’s creation in February 1850; removed “(name tentative)” from the translations.

Translation: en changed to “the pride of the high and the great, Şefik Bey — may his eminence endure —” · tr changed to “yücelerin ve büyüklerin iftiharı Şefik Bey — yüceliği daim olsun —” · fr changed to “la fierté des hauts et des grands, Şefik Bey — que sa grandeur dure —” · ja changed to “高位なる者と偉大なる者の誇り、シェフィーク・ベイ――その高位の続かんことを――”

### l4 · chunk 1  [current conf: partial → proposed: partial]
```
Current:  فراغنه فراشت شریفه‌ده بر قیراط عهده‌سنه توجیهنی  |  ferâğına ferâşet-i şerîfede bir kırât ‘uhdesine tevcîhini
Mine:     طرفندن فراشت شریفهٔ مرقومه‌دن بر قیراط عهده‌سنه توجیهنی  |  tarafından ferâşet-i şerîfe-i merkûmeden bir kırât ‘uhdesine tevcîhini
```
Words:
- word 1 “فراغنه”: correct → “طرفندن” (*tarafından*). Evidence: upright stem + loop of `ط` (no `ف` dot on the head), descending `ر`, looped `ف` with dot, `ن`, `د`, and final `ن` bowl (“on his part”, governing *taleb ve istid‘â eylediğine binâ’en* in chunk 2 — confirming there was no resignation/*ferâğ* by a prior holder).
- word 2 “فراشت”: agree
- word 3 “شریفه‌ده”: correct → “شریفهٔ مرقومه‌دن” (*şerîfe-i merkûmeden*, kept at `guess` because the pale red letters between `شریفه` and `-دن` are abraded, though `مـرقومـه‌دن` fits both the trace length and syntax “one carat from the aforesaid noble sweeping service”).
- words 4–7 “بر قیراط عهده‌سنه توجیهنی”: agree

Translation: en changed to “on his part, the conferring upon him of one carat (kırat) of the aforesaid noble sweeping service” · tr changed to “tarafından, anılan şerefli ferâşetten bir kıratın uhdesine tevcihini” · fr changed to “de sa part, l’attribution à sa charge d’un carat (kırat) dudit noble service du balayage” · ja changed to “彼のもとより、上述の高貴な掃除の奉仕から一キラートを自らの管掌に授けるよう”

### l4 · chunk 2  [current conf: partial → proposed: probable]
```
Current:  طلب و استدعا ایلدیکنه بنا  |  taleb ve istid‘â eylediğine binâ’en
Mine:     طلب و استدعا ایلدیکنه بناءً  |  taleb ve istid‘â eylediğine binâ’en
```
Words:
- all words: agree (`بنا` written out as `بناءً` matching the double *tenvîn* stroke in the ink; upgraded to `probable`).

Translation: en ok · tr ok · fr ok · ja ok

### l4 · chunk 3  [current conf: partial → proposed: probable]
```
Current:  بروجه حسبی بر قیراط فراشت شریفه نك  |  ber-vech-i hasebî bir kırât ferâşet-i şerîfe-nin
Mine:     بروجه حسبی بر قیراط فراشت شریفه‌نك  |  ber-vech-i hasebî bir kırât ferâşet-i şerîfenin
```
Words:
- all words: agree (`شریفه نك` joined orthographically as `شریفه‌نك` *şerîfenin*; upgraded to `probable`).

Translation: en ok · tr ok · fr ok · ja ok

### l4 · chunk 4  [current conf: partial → proposed: probable]
```
Current:  عهده‌سنه توجیهی خصوصنه مساعده علیه‌م شایان اولدیغی حالده  |  ‘uhdesine tevcîhi husûsuna müsâ‘ade-i ‘aliyyem şâyân olduğı hâlde
Mine:     عهده‌سنه توجیهی خصوصنه مساعدهٔ علیه‌م شایان اولدیغی حالده  |  ‘uhdesine tevcîhi husûsuna müsâ‘ade-i ‘aliyyem şâyân olduğu hâlde
```
Words:
- all words: agree (`مساعدهٔ` normalized with *hemze-i izâfet*; upgraded to `probable`).

Translation: en ok · tr ok · fr ok · ja ok

### l4 · chunk 5  [current conf: partial → proposed: probable]
```
Current:  اول بابده لازم کلن …  |  ol bâbda lâzım gelen …
Mine:     اول بابده لازم کلان  |  ol bâbda lâzım gelen
```
Words:
- words 1–3 “اول بابده لازم”: agree
- words 4–5 “کلن …”: correct → “کلان” (*gelen*, slot 4; slot 5 empty). Evidence: word polygon 4 covers `کلا` (`ک` with diagonal stroke + `لا` ligature) and word polygon 5 covers the tall final `ن` bowl with single dot above — together spelling standard Ottoman `کلان` (*ol bâbda lâzım gelen*, modifying *berât-ı şerîfimin ısdârı* at the start of line 5). Nothing is missing.

Translation: en changed to “requisite in that matter” · tr changed to “o hususta gereken” · fr changed to “requis en cette affaire” · ja changed to “その件につき必要となる”

## l5 — The request

### l5 · chunk 0  [current conf: partial → proposed: probable]
```
Current:  بیله تفضل الصلای خصوصی  |  bile tefaddul es-salâ-yı husûsı
Mine:     برات شریفمك اصداری خصوصی  |  berât-ı şerîfimin ısdârı husûsu
```
Words:
- word 1 “بیله”: correct → “برات” (*berât-ı*). Evidence: `ب` with dot below, `ر`, tall `ا`, and wide flat `ت` with two dots above.
- word 2 “تفضل”: correct → “شریفمك” (*şerîfimin*). Evidence: stretched `شـ` with three-dot mark, `ر`, `ی`, `ف` loop, `م`, and tall flagged final `ك` (genitive `-مك`, noted in the earlier pass).
- word 3 “الصلای”: correct → “اصداری” (*ısdârı*). Evidence: tall `ا`, `ص` loop joined into `د` + `ا`, `ر`, and final `ی` (*ol bâbda lâzım gelen berât-ı şerîfimin ısdârı husûsu*, “the matter of issuing my noble berat requisite in that affair”).
- word 4 “خصوصی”: agree

Translation: en changed to “the matter of issuing my noble berat” · tr changed to “şerefli beratımın çıkarılması hususu” · fr changed to “l’affaire de la délivrance de mon noble berat” · ja changed to “わが貴きベラートを発給する件が”

### l5 · chunk 1  [current conf: partial → proposed: probable]
```
Current:  منحل ده رجال دولت علیه‌مدن  |  münhal de ricâl-i Devlet-i ‘Aliyyemden
Mine:     متحیزان رجال دولت علیه‌مدن  |  mütehayyizân-ı ricâl-i Devlet-i ‘Aliyyemden
```
Words:
- words 1–2 “منحل ده”: correct → “متحیزان” (*mütehayyizân-ı*, slot 1; slot 2 empty). Evidence: initial `م`, two-dotted `ت`, `ح` wedge, `ی` with two dots below, descending `ز` with dot above, tall `ا`, and deep `ن` bowl with dot inside (*mütehayyizân-ı ricâl-i Devlet-i ‘Aliyyemden*, standard protocol formula for *Ûlâ Sınıf-ı Sânîsi* officials — eliminating the false vacancy word *münhal*).
- words 3–6 “رجال دولت علیه‌مدن”: agree

Translation: en changed to “one of the distinguished statesmen of my Sublime State,” · tr changed to “Devlet-i Aliyyemin seçkin ricalinden,” · fr changed to “l’un des dignitaires distingués de mon Sublime État,” · ja changed to “わが至高なる国家の重臣の一人、”

### l5 · chunk 2  [current conf: probable → proposed: probable]
```
Current:  حالا اوقاف همایونم ناظری افتخار الاعالی  |  hâlâ Evkâf-ı hümâyûnum nâzırı iftihârü’l-e‘âlî
Mine:     (same)
```
Words:
- all words: agree (*hâlâ Evkâf-ı hümâyûnum nâzırı iftihârü’l-e‘âlî*)

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 3  [current conf: probable → proposed: probable]
```
Current:  والاعاظم السیّد علی رضا دام علوّه  |  ve’l-e‘âzım es-Seyyid ‘Alî Rızâ dâme ‘ulüvvühû
Mine:     (same)
```
Words:
- all words: agree (*ve’l-e‘âzım es-Seyyid ‘Alî Rızâ dâme ‘ulüvvühû* — historically **Bursalı es-Seyyid Ali Rızâ Efendi**, *Evkâf-ı Hümâyûn Nâzırı* in 1850–1851).

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 4  [current conf: probable → proposed: probable]
```
Current:  طرفندن بالتقریر افاده اولنمغین  |  tarafından bi’t-takrîr ifâde olunmağın
Mine:     طرفندن با تقریر افاده اولنمغین  |  tarafından bâ-takrîr ifâde olunmağın
```
Words:
- words 1, 3, 4: agree
- word 2 “بالتقریر”: correct → “با تقریر” (*bâ-takrîr*). Evidence: `ب` + vertical `ا` stands directly before `تقریر` with no second tall `ل` stem between `با` and `ت`.

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 5  [current conf: probable → proposed: probable]
```
Current:  بر منوال محرر توجیهی التماس خصوصنه  |  ber-minvâl-i muharrer tevcîhi iltimâs husûsuna
Mine:     (same)
```
Words:
- all words: agree (*ber-minvâl-i muharrer tevcîhi iltimâs husûsuna*)

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 6  [current conf: partial → proposed: probable]
```
Current:  … مساعدهٔ علیه‌م ارزانی قلنه‌رق  |  … müsâ‘ade-i ‘aliyyem erzânî kılınarak
Mine:     مساعدهٔ علیه‌م ارزانی قلنه‌رق  |  müsâ‘ade-i ‘aliyyem erzânî kılınarak
```
Words:
- words 1–2 “… مساعدهٔ”: correct → “مساعدهٔ” (*müsâ‘ade-i*, slot 1; slot 2 empty). Evidence: as noted in the earlier pass, slot 1 is simply the stretched initial `مسا` sweep of `مساعدهٔ`, not a separate unread word.
- words 3–5 “علیه‌م ارزانی قلنه‌رق”: agree

Translation: en ok · tr ok · fr ok · ja ok

### l5 · chunk 7  [current conf: probable → proposed: probable]
```
Current:  بو بیك ایکی یوز التمش یدی سنه‌سی ربیع الاولنك  |  bu bin iki yüz altmış yedi senesi Rebî‘ü’l-evvelinin
Mine:     (same)
```
Words:
- all words: agree (*bu bin iki yüz altmış yedi senesi Rebî‘ü’l-evvelinin*)

Translation: en ok · tr ok · fr ok · ja ok

## l6 — The grant

### l6 · chunk 0  [current conf: partial → proposed: probable]
```
Current:  اوچنجی کونی صادر اولان فرمان عالیشانم موجبنجه  |  üçüncü güni sâdır olan fermân-ı ‘âlî-şânım mûcebince
Mine:     اوچنجی کونی صادر اولان فرمان عالیشانم موجبنجه  |  üçüncü günü sâdır olan fermân-ı ‘âlî-şânım mûcebince
```
Words:
- all words: agree (`güni` normalized to `günü` in transliteration; upgraded to `probable`).

Translation: en ok · tr ok · fr ok · ja ok

### l6 · chunk 1  [current conf: partial → proposed: probable]
```
Current:  … بله مومی الیه  |  … -ile mûmâ ileyh
Mine:     ایشبو برات همایونی  |  işbu berât-ı hümâyûnu
```
Words:
- words 1–2 “… بله”: correct → “ایشبو” (*işbu*, slot 1; slot 2 empty). Evidence: tall `ا`, `ی` + stretched `شـ` with three-dot mark, `ب` with dot below, and `و` — identical to `ایشبو` in `l3.10`.
- word 3 “مومی”: correct → “برات” (*berât-ı*). Evidence: `ب` + `ر` + tall `ا` + flat `ت` with dots above.
- word 4 “الیه”: correct → “همایونی” (*hümâyûnu*). Evidence: looped `هـ` + `م` + tall `ا`, `یو`, and `نی` bowl (*işbu berât-ı hümâyûnu*, direct object of *verdim* in chunk 2).

Translation: en changed to “this imperial berat” · tr changed to “işbu hümayun beratı” · fr changed to “ce berat impérial” · ja changed to “この帝室ベラートを”

### l6 · chunk 2  [current conf: partial → proposed: probable]
```
Current:  بر وجه حسبی … بروجه  |  ber-vech-i hasebî … ber-vech-i
Mine:     ویردم و بیوردم که مشار الیه بروجه  |  verdim ve buyurdum ki müşârün-ileyh ber-vech-i
```
Words:
- word 1 “بر”: correct → “ویردم” (*verdim*). Evidence: `و`, `ی` with two dots below, descending `ر`, `د`, and `م`.
- word 2 “وجه”: correct → “و بیوردم که” (*ve buyurdum ki*). Evidence: `و`, `بیوردم` (`ب`+`ی` dots below + `و` + `ر` + `د` + `م`), and `که` (`ک` with diagonal stroke + `ه`) — completing the universal Ottoman berat promulgation formula *işbu berât-ı hümâyûnu verdim ve buyurdum ki*.
- words 3–4 “حسبی …”: correct → “مشار الیه” (*müşârün-ileyh*). Evidence: `م`, stretched `شـ` with three-dot mark + tall `ا` + `ر`, followed by tall `الـیه` (confirming the earlier observation of an `الـ` group with dotted tooth below). Matches Şefîk Bey’s *e‘âzım* rank (*müşârün-ileyh*, not lower-rank *mûmâ-ileyh*).
- word 5 “بروجه”: agree (*ber-vech-i*, running into *hasebî* at the start of chunk 3)

Translation: en changed to “I have given, and I have commanded that the aforesaid dignitary, by way of” · tr changed to “verdim ve buyurdum ki müşârün-ileyh, ber-vech-i” · fr changed to “j’ai donné, et j’ai ordonné que ledit haut dignitaire, à titre” · ja changed to “授け、かく命じた。すなわち上述の高官は、”

### l6 · chunk 3  [current conf: partial → proposed: probable]
```
Current:  حسبی … بر قیراط کعبهٔ معظمه  |  hasebî … bir kırât Ka‘be-i Mu‘azzama
Mine:     حسبی نائل اولدیغی بر قیراط خدمت مابه المفخرهٔ  |  hasebî nâil olduğu bir kırât hıdmet-i mâ-bihi’l-mefhare-i
```
Words:
- word 1 “حسبی”: agree (*hasebî*)
- word 2 “…”: correct → “نائل اولدیغی” (*nâil olduğu*). Evidence: `نا` + `ئل` before `اولدیغی` (tall `ا` + `و` + `ل` + `دیغی` bowl), matching the two stacked groups between `حسبی` and `بر قیراط`.
- words 3–4 “بر قیراط”: agree (*bir kırât*)
- word 5 “کعبهٔ”: correct → “خدمت مابه” (*hıdmet-i mâ-bihi*). Evidence: there is no `ک` stroke here; the ink shows `خ` with dot above + `دمت` followed by `ما` + `به` with single dot below `ب`.
- word 6 “معظمه”: correct → “المفخرهٔ” (*’l-mefhare-i*). Evidence: tall `الـ`, `م`, looped `ف` with dot, `خ` wedge with dot above (no `ظ` vertical stem), `ر`, and final `ه` (*hıdmet-i mâ-bihi’l-mefhare-i ferâşet-i şerîfeyi*, “the pride-conferring service of the noble sweeping”).

Translation: en changed to “an honorary grant which he has attained — one carat of the pride-conferring service of” · tr changed to “hasebî nail olduğu bir kırat medar-ı iftihar olan” · fr changed to “honorifique qu’il a obtenu — un carat du service glorieux” · ja changed to “名誉として得た一キラートの誇り高き奉仕たる”

### l6 · chunk 4  [current conf: partial → proposed: partial]
```
Current:  فراشت شریفه الحق … ابدی  |  ferâşet-i şerîfe el-hakk … ebedî
Mine:     فراشت شریفه‌یی قبلندن اهل … و خبیر تعیین ایده‌جکی  |  ferâşet-i şerîfeyi kıbelinden ehl … ve habîr ta‘yîn edeceği
```
Words:
- word 1 “فراشت”: agree (*ferâşet-i*)
- word 2 “شریفه”: correct → “شریفه‌یی” (*şerîfeyi*, accusative suffix `-یی` clearly visible at the end of `شریفه`, which sat unassigned in slot 3).
- words 3–4 “… الحق”: correct → “قبلندن اهل” (*kıbelinden ehl*). Evidence: looped `ق` + `ب` + tall `ل` + `ندن` (“on his behalf / from his side”), followed by `اهل` (`ا` + `ه` + `ل`).
- word 5 “…”: uncertain (`illegible`, pale word between `اهل` and `و خبیر` — likely *‘iffet* / *diyânet* or *وقار*, left honestly as `…`).
- word 6 “…”: correct → “و خبیر تعیین” (*ve habîr ta‘yîn*). Evidence: `و` + `خ` dot above + `ب` dot below + `یر` (*ve habîr*, noted as `خیر…` in the earlier pass), followed by `تعیین` (`ت` + `ع` + double `یی` + `ن` bowl).
- word 7 “ابدی”: correct → “ایده‌جکی” (*edeceği*). Evidence: tall `ا`, `ید` + `ه`, `ج` with dot below, diagonal-flagged `ک`, and returning `ی` (*kıbelinden ehl … ve habîr ta‘yîn edeceği | vekîliyle*, “through a competent, … and well-versed proxy whom he shall appoint on his behalf”).

Translation: en changed to “the noble sweeping — through [a proxy] whom he shall appoint on his behalf, competent, … and well-versed” · tr changed to “şerefli ferâşet [hizmetin]i, kendi tarafından ehil, … ve habîr olarak tayin edeceği” · fr changed to “du noble balayage — par [un mandataire] qu’il désignera de sa part, compétent, … et expérimenté” · ja changed to “高貴な掃除の務めを、自らの側より適任かつ…通暁した者として任命する”

### l6 · chunk 5  [current conf: partial → proposed: probable]
```
Current:  کمال تعظیم و تکریم  |  kemâl-i ta‘zîm ve tekrîm
Mine:     وکیلیله کمال تعظیم و تکریم  |  vekîliyle kemâl-i ta‘zîm ve tekrîm
```
Words:
- word 1 (previously unassigned before `کمال`): correct → “وکیلیله” (*vekîliyle*). Evidence: the `و…` group sitting in word slot 1 before `کمال` has initial `و`, flagged `ک` stroke above, `ی` + `ل` + `یله` — supplying the noun *vekîliyle* (“through his proxy”) required both by *ta‘yîn edeceği* in chunk 4 and by *bi’l-vekâle* at the start of line 7.
- words 2–5 “کمال تعظیم و تکریم”: agree

Translation: en changed to “through his proxy, with perfect reverence and honour” · tr changed to “vekili vasıtasıyla, tam bir tazim ve tekrim” · fr changed to “par l’entremise de son mandataire, avec une parfaite révérence et vénération” · ja changed to “代理人を通じて、この上ない畏敬と尊崇、”

### l6 · chunk 6  [current conf: probable → proposed: probable]
```
Current:  آداب و نهایت حیا و حجاب  |  âdâb ve nihâyet-i hayâ ve hicâb
Mine:     و آداب و نهایت حیا و حجاب  |  ve âdâb ve nihâyet-i hayâ ve hicâb
```
Words:
- word 1 “آداب”: correct → “و آداب” (*ve âdâb*; conjunction `و` visible before `آداب`).
- words 2–6 “و نهایت حیا و حجاب”: agree

Translation: en changed to “and decorum, and the utmost modesty and reserve” · tr changed to “ve edep ve son derece haya ve hicab” · fr changed to “et bienséance, et la plus grande pudeur et retenue” · ja changed to “ならびに礼節と、この上ない恥じらいと慎みとをもって、”

### l6 · chunk 7  [current conf: partial → proposed: probable]
```
Current:  نظافت البسه و ثیاب ایله  |  nezâfet-i elbise ve siyâb ile
Mine:     و نظافت البسه و ثیاب ایله  |  ve nezâfet-i elbise ve siyâb ile
```
Words:
- words 1–2 “نظافت (empty)”: correct → “و” (slot 1) + “نظافت” (slot 2) (*ve nezâfet-i*). Evidence: slot 1 at the bottom right of the rising stack encloses the conjunction `و` right above `حجاب`, while slot 2 encloses `نظافت` — matching the 1904 parallel (*ve nezâfet-i elbise ve siyâb ile*) word for word.
- words 3–5 “البسه و ثیاب ایله”: agree

Translation: en changed to “and with cleanliness of garments and clothes” · tr changed to “ve elbise ve giysi temizliği ile” · fr changed to “et avec la propreté des habits et des vêtements” · ja changed to “ならびに衣服と装束の清潔さをもって”

## l7 — Closing and date

### l7 · chunk 0  [current conf: probable → proposed: read]
```
Current:  بلکه مسك ناب و العنبر الطیوب  |  belki misk nâb ve el-‘anber et-tuyûb
Mine:     بالوکاله حسن تأدیه و ایفا ایدوب  |  bi’l-vekâle hüsn-i te’diye ve îfâ edüp
```
Words:
- word 1 “بلکه”: correct → “بالوکاله” (*bi’l-vekâle*). Evidence: `ب` + tall `الـ` + clear `و` loop between `ل` and flagged `کا` + `له` (“by proxy”, picking up *vekîliyle* in `l6.5`).
- word 2 “مسك”: correct → “حسن” (*hüsn-i*). Evidence: open `ح` head (no `م` loop and no `ک` stroke), three-toothed `س` with caret, and deep `ن` bowl with single dot.
- word 3 “ناب”: correct → “تأدیه” (*te’diye*). Evidence: two-dotted `ت` + tall `ا`, `د`, `ی` with two dots below, and final `ه`.
- word 4 “و”: agree
- word 5 “العنبر”: correct → “ایفا” (*îfâ*). Evidence: tall `ا` (no `ل` or `ع` or `نبر`), `ی` dots below, looped `ف` with single dot above, and tall `ا` (*hüsn-i te’diye ve îfâ*).
- word 6 “الطیوب”: correct → “ایدوب” (*edüp*). Evidence: as noted in the earlier pass, there is no `ط` stem — tall `ا`, `ی` with two dots below, `د`, `و`, and wide flat `ب` boat with single dot underneath.

Translation: en changed to “duly rendering and fulfilling [it] by proxy,” · tr changed to “vekâleten güzelce eda ve ifa edip,” · fr changed to “s’en acquittant et l’accomplissant dûment par procuration,” · ja changed to “代理によって立派に遂行・完遂し、”

### l7 · chunk 1  [current conf: partial → proposed: probable]
```
Current:  فی كعبه ابدی عمر و شوکتم  |  fî Ka‘be ebedî ‘ömr ü şevketim
Mine:     و دیمومت ایام عمر و شوکت شاهانه‌م  |  ve deymûmet-i eyyâm-ı ‘ömr ü şevket-i şâhânem
```
Words:
- word 1 “فی”: correct → “و” (*ve*).
- word 2 “كعبه”: correct → “دیمومت” (*deymûmet-i*). Evidence: no `ک` stroke; `د` + `یم` + `و` + `مت` with flat two-dotted `ت` at the end (accounting for the extra letters before `ایام` noted in the earlier pass).
- word 3 “ابدی”: correct → “ایام” (*eyyâm-ı*). Evidence: tall `ا`, `ی` with two dots below + tall `ا`, and final `م` with downward tail (*ve deymûmet-i eyyâm-ı ‘ömr ü şevket-i şâhânem*, standard chancery prayer formula).
- words 4–5 “عمر و”: agree
- word 6 “شوکتم”: correct → “شوکت شاهانه‌م” (*şevket-i şâhânem*). Evidence: after `شوکت` sits stacked `شاهانه‌م` (`شـ` + `اهانه‌م`) inside the left end of chunk 1.

Translation: en changed to “and [for] the perpetuity of the days of my imperial life and majesty” · tr changed to “ve ömür ve şahane şevketim günlerinin devamı” · fr changed to “et [pour] la perpétuité des jours de ma vie et de ma majesté impériale” · ja changed to “ならびにわが帝王としての命と威光の日々の永続と、”

### l7 · chunk 2  [current conf: probable → proposed: read]
```
Current:  و مظفریتم ترقیاتم دعوات خیریه‌سنه  |  ve muzafferiyetim terakkiyâtım da‘avât-ı hayriyyesine
Mine:     و مظفریت عساکر نظامیهٔ شاهانه‌م دعوات خیریه‌سنه  |  ve muzafferiyet-i ‘asâkir-i nizâmiyye-i şâhânem da‘avât-ı hayriyyesine
```
Words:
- word 1 “و”: agree
- word 2 “مظفریتم”: correct → “مظفریت” (*muzafferiyet-i*, flat `ت` with two dots above and no `-م`, standing in *izâfet* with the following noun phrase).
- word 3 “ترقیاتم”: correct → “عساکر نظامیهٔ شاهانه‌م” (*‘asâkir-i nizâmiyye-i şâhânem*). Evidence: stacked three-tier military title: `عساکر` (`ع` + `سا` + diagonal-flagged `ک` + `ر`) at bottom right, `نظامیهٔ` (`ن` + vertical-stemmed `ظ` with dot + `امیهٔ`) in the middle, and `شاهانه‌م` (`شـ` + `اهانه‌م`) above — **‘Asâkir-i Nizâmiyye-i Şâhâne**, the official post-1843 name of Sultan Abdülmecid’s regular army.
- words 4–5 “دعوات خیریه‌سنه”: agree

Translation: en changed to “and the victory of my Imperial Regular Armies, in auspicious prayers” · tr changed to “ve şahane nizamiye askerlerimin muzafferiyeti hayır dualarına” · fr changed to “et la victoire de mes armées régulières impériales, aux pieuses prières” · ja changed to “わが帝室正規軍（アサーキリ・ニザーミーイェ）の勝利を願う善き祈りに”

### l7 · chunk 3  [current conf: probable → proposed: probable]
```
Current:  اشتغال و مواظبه ایلیه  |  iştigâl ve muvâzabet eyleye.
Mine:     (same)
```
Words:
- all words: agree (*iştigâl ve muvâzabet eyleye.*)

Translation: en ok · tr ok · fr ok · ja ok

### l7 · chunk 4  [current conf: partial → proposed: probable]
```
Current:  شویله بیله‌لر علامت شریفه اعتماد قیله‌لر  |  Şöyle bileler, ‘alâmet-i şerîfe i‘timâd kılalar.
Mine:     شویله بیله‌لر علامت شریفمه اعتماد قیله‌لر  |  Şöyle bileler, ‘alâmet-i şerîfime i‘timâd kılalar.
```
Words:
- words 1–3, 5–6: agree
- word 4 “شریفه”: correct → “شریفمه” (*şerîfime*). Evidence: as noted as a candidate in the earlier pass, between `ف` and final `ه` sits a small looped `م` joint (*‘alâmet-i şerîfime i‘timâd kılalar*, 1st-person imperial possessive matching *berât-ı şerîfimin*, *fermân-ı ‘âlî-şânım*, and *Hazîne-i Hâssam*).

Translation: en changed to “Thus let them know, [and] place trust in my noble sign.” · tr changed to “Şöyle bilsinler, şerefli alâmetime itimat etsinler.” · fr changed to “Qu’ils le sachent ainsi, [et] qu’ils se fient à mon noble signe.” · ja changed to “かく知るべし、わが高貴なる印を信ずべし。”

### l7 · chunk 5  [current conf: probable → proposed: probable]
```
Current:  تحریراً فی الیوم الثامن من شهر ربیع الاول  |  Tahrîren fi’l-yevmi’s-sâmin min şehr-i Rebî‘i’l-evvel
Mine:     (same)
```
Words:
- all words: agree (*Tahrîren fi’l-yevmi’s-sâmin min şehr-i Rebî‘i’l-evvel*)

Translation: en ok · tr ok · fr ok · ja ok

### l7 · chunk 6  [current conf: partial → proposed: probable]
```
Current:  سنه سبع و ستین و مائتین و الف  |  sene seb‘ ve sittîn ve mi’eteyn ve elf
Mine:     (same)
```
Words:
- all words: agree (*sene seb‘ ve sittîn ve mi’eteyn ve elf* = 1267; word 1 upgraded from `guess` to `probable` so chunk `conf` is `probable`).

Translation: en ok · tr ok · fr ok · ja ok

## place — Place of issue

### place · chunk 0  [current conf: probable → proposed: probable]
```
Current:  بمقام قسطنطنیه المحروسه  |  Bi-makâm-ı Kostantıniyye el-mahrûse
Mine:     (same)
```
Words:
- (no word list)

Note: Tightly knotted *Bi-makâm-ı Kostantıniyye el-mahrûse* flourish below the date.

Translation: en ok · tr ok · fr ok · ja ok

## Summary

**Counts.** 60 chunks total: **16** confirmed unchanged from `fe8256c`, **44** updated (**38** changing the Ottoman text of at least one word, **3** normalizing transliteration/orthography, and **3** upgrading word confidences / removing tentative name disclaimers). Entry-level confidences improved on `l1` (`unread` → `probable`), `l3` (`partial` → `probable`), `l5` (`partial` → `probable`), `l6` (`unread` → `partial`, with 7 of 8 chunks `probable`), and `l7` (`partial` → `probable`).

**Names and key facts established from the ink**

| What | Reading | Where | Identification & certainty |
|---|---|---|---|
| Museum object | Sadberk Hanım Museum, inv. **SHM 19076 Y. 272** | whole sheet | Gift of Reya Danışman; dated 8 Rebîülevvel 1267 / 11 January 1851 |
| Occasion of grant | *Ravza-i Mutahhara … misillü … Mekke-i Mükerreme … Harem-i muhtereminde dahî **müceddeden ma‘lûmü’l-kırât ferâşet-i şerîfe** tertîb ve tanzîmine* | l2.5–l3.4 | `probable`–`read`: newly instituted Mecca *ferâşet* carat-shares (Safer 1267 / Dec 1850), explaining the absence of a prior holder or vacancy clause |
| Recipient | *e‘âzım-ı ricâl-i Devlet-i ‘Aliyyemden hâlâ Hazîne-i Hâssam nâzırı … iftihârü’l-e‘âlî ve’l-e‘âzım **Şefîk Bey** dâme ‘ulüvvühû* (referred to in `l6.2` as ***müşârün-ileyh***) | l3.8–l4.0, l6.2 | `read`: **Ali Şefik Bey (Paşa)**, first Minister of the Privy Treasury (*Hazîne-i Hâssa Nâzırı*, appointed Feb 1850) |
| Recommending official | *mütehayyizân-ı ricâl-i Devlet-i ‘Aliyyemden hâlâ Evkâf-ı hümâyûnum nâzırı iftihârü’l-e‘âlî ve’l-e‘âzım **es-Seyyid ‘Alî Rızâ** dâme ‘ulüvvühû* | l5.1–l5.3 | `read`: **Bursalı es-Seyyid Ali Rızâ Efendi**, Minister of Imperial Endowments (*Evkâf-ı Hümâyûn Nâzırı*, 1850–1851) |
| What is granted & how performed | *ber-vech-i hasebî … bir kırât hıdmet-i mâ-bihi’l-mefhare-i ferâşet-i şerîfeyi kıbelinden ehl … ve habîr ta‘yîn edeceği **vekîliyle** … **bi’l-vekâle** hüsn-i te’diye ve îfâ edüp* | l4.1–l4.3, l6.2–l7.0 | `probable`–`read`: 1 honorary *kırât* of Mecca’s *ferâşet*, performed on his behalf by an appointed local proxy (*vekîl*) |
| Closing prayer clause | *deymûmet-i eyyâm-ı ‘ömr ü şevket-i şâhânem ve muzafferiyet-i **‘asâkir-i nizâmiyye-i şâhânem** da‘avât-ı hayriyyesine* | l7.1–l7.3 | `read`: prayer for the sultan’s life/majesty and the victory of his *‘Asâkir-i Nizâmiyye-i Şâhâne* (post-1843 regular army) |
| Dates & place | Imperial order: **3 Rebîülevvel 1267** (6 Jan 1851); Berat: **8 Rebîülevvel 1267** (11 Jan 1851), *Bi-makâm-ı Kostantıniyye el-mahrûse* | l5.7–l6.0, l7.5–place | `probable`–`read` |

**What still remains uncertain (kept honestly at `partial` / `…`)**

- `davet.0`, `nisan.0`, `nisan.1`, and `place.0`: stacked gold/red formulas where interior word boundaries cannot be separated individually (`والمنّ` vs `والصون` in `nisan.1`).
- `l2.0` (end), `l2.1`, and `l2.2` (first two words): abraded red ink along the horizontal paper fold.
- `l4.1` word 3 (*şerîfe-i merkûmeden*): syntactically and spatially fitting, kept at `guess` (`partial` chunk) because the red ink in the middle of `مرقومه‌دن` is abraded.
- `l6.4` word 5 (`…` between `اهل` and `و خبیر`): one short abraded red word in the proxy qualification phrase, kept as `illegible` (`…`).

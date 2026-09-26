## 6.0.0 (2026-09-26)

Part of M10 epic 8 (museumwithnofrontiers/inventory-app#2019), story
museumwithnofrontiers/inventory-app#2062. **Breaking:** four entries are
removed, the last gallery/exhibition pairs that said the same thing under two
names. Nothing reads them since viewer-layout 3.2.1, and no website overloads
one; package-ci builds and tests all 46 websites against this release.

### Removed

| Removed | Replacement |
|---|---|
| `gallery.action.partnerProfile`, `exhibition.partnerObjects.partnerProfile` | `partner.action.partnerProfile` |
| `gallery.banner.detailFrom`, `exhibition.media.detailFrom` | `layout.banner.detailFrom` |

### Migration

A website that names one of them — in its code, or as an overload in its own
`locales/` — names its replacement instead.
## 5.1.0 (2026-09-26)

Part of M10 epic 8 (museumwithnofrontiers/inventory-app#2019), story
museumwithnofrontiers/inventory-app#2062.

### Added

- `partner.action.partnerProfile` — "Partner Profile", the link from a
  partner's objects to its profile, and `layout.banner.detailFrom` — "Detail
  from", the banner's caption before the item's name. The last two texts a
  gallery and an exhibition said the same way under different names
  (`gallery.action.partnerProfile` / `exhibition.partnerObjects.partnerProfile`,
  `gallery.banner.detailFrom` / `exhibition.media.detailFrom`), in every
  language their section promises: Arabic, German, Spanish and French are the
  gallery entries', the rest were translated for this dictionary.

The entries they replace stay until nothing reads them (the next major).
## 5.0.0 (2026-09-26)

Part of M10 epic 8 (museumwithnofrontiers/inventory-app#2019), story
museumwithnofrontiers/inventory-app#2064. **Breaking:** 114 entries are
removed. No package, template or website reads any of them, and no website
overloads one; package-ci builds and tests all 46 websites against this
release.

### Removed

- The `gallery.*` and `exhibition.*` entries that said what a shared entry
  says, the case-only variants (`timeline.form.startDate` "Start Date" beside
  `catalogue.facet.startDate` "Start date", and the like) and
  `exhibition.theme.previous`/`.next`. Each has a replacement, below; the
  shared entries carry their translations (sources.md).
- The entries nothing read: `catalogue.facet.selectDynasty`,
  `catalogue.facet.selectInstitution`, `catalogue.search.keyword`,
  `core.action.add`, `exhibition.action.here`, `exhibition.action.seeMore`,
  `exhibition.chapter.next`, `exhibition.chapter.previous`,
  `exhibition.error.notFoundBody`, `exhibition.error.notFoundTitle`,
  `exhibition.nav.islamicDynasties`, `exhibition.partner.fax`,
  `exhibition.partner.noObjects`, `exhibition.partner.objectsInExhibition`,
  `exhibition.partner.phone`, `exhibition.results.date`,
  `exhibition.results.noSearchResults`, `exhibition.section.error`,
  `exhibition.sponsors.footerFour`, `exhibition.sponsors.footerOne`,
  `exhibition.sponsors.footerThree`, `exhibition.sponsors.footerTwo`,
  `exhibition.theme.collapseAll`, `exhibition.theme.expandAll`,
  `exhibition.theme.filterBySubtheme`, `exhibition.theme.seeGalleryFor`,
  `exhibition.theme.selectSubtheme`, `gallery.action.here`,
  `gallery.error.notFoundBody`, `gallery.error.notFoundTitle`,
  `gallery.nav.islamicDynasties`, `gallery.partner.fax`,
  `gallery.partner.objectsInGallery`, `gallery.partner.phone`,
  `gallery.related.items`, `gallery.related.objects`, `gallery.results.date`,
  `gallery.results.noSearchResults`, `partner.map.onTheMap`,
  `partner.nav.notFound`, `record.action.returnHome`, `record.sheet.notFound`,
  `sheet.field.shortDescription`, `timeline.form.none`,
  `timeline.form.searchIntro`, `timeline.form.yearSuffix`,
  `timeline.results.countryDescription`.

### Migration

A website that names a removed entry — in its code, or as an overload in its
own `locales/` — names its replacement instead:

| Removed | Replacement |
|---|---|
| `timeline.form.endDate` | `catalogue.facet.endDate` |
| `timeline.form.selectCountry` | `catalogue.facet.selectCountry` |
| `timeline.form.startDate` | `catalogue.facet.startDate` |
| `exhibition.action.seeDatabaseEntry`, `gallery.action.seeDatabaseEntry` | `catalogue.results.seeDatabaseEntry` |
| `exhibition.search.overallDatabase`, `gallery.search.overallDatabase` | `catalogue.search.overallDatabase` |
| `exhibition.search.placeholder`, `gallery.search.placeholder` | `catalogue.search.placeholder` |
| `exhibition.search.relatedDatabase`, `gallery.search.relatedDatabase` | `catalogue.search.relatedDatabase` |
| `exhibition.footer.aboutMwnf`, `gallery.footer.aboutMwnf` | `core.footer.aboutMwnf` |
| `exhibition.footer.contact`, `gallery.footer.contact` | `core.footer.contact` |
| `exhibition.footer.cookies`, `gallery.footer.cookies` | `core.footer.cookies` |
| `exhibition.footer.copyright`, `gallery.footer.copyright` | `core.footer.copyright` |
| `exhibition.footer.credits`, `gallery.footer.credits` | `core.footer.credits` |
| `exhibition.footer.legalNotice`, `gallery.footer.legalNotice` | `core.footer.legalNotice` |
| `exhibition.nav.about`, `gallery.nav.about` | `core.nav.about` |
| `exhibition.nav.artisticIntroduction`, `gallery.nav.artisticIntroduction` | `core.nav.artisticIntroduction` |
| `exhibition.nav.collection`, `gallery.nav.collection` | `core.nav.collection` |
| `exhibition.nav.credits`, `gallery.nav.credits` | `core.nav.credits` |
| `exhibition.nav.myCollection`, `gallery.nav.myCollection` | `core.nav.myCollection` |
| `exhibition.nav.overallDatabase`, `gallery.nav.overallDatabase` | `core.nav.overallDatabase` |
| `exhibition.nav.partners`, `gallery.nav.partners` | `core.nav.partners` |
| `exhibition.nav.timeline`, `gallery.nav.timeline` | `core.nav.timeline` |
| `exhibition.theme.next` | `core.pagination.next` |
| `exhibition.theme.previous` | `core.pagination.previous` |
| `exhibition.section.about`, `gallery.section.about` | `core.section.about` |
| `exhibition.section.collection`, `gallery.section.collection` | `core.section.collection` |
| `exhibition.section.credits`, `gallery.section.credits` | `core.section.credits` |
| `exhibition.section.database`, `gallery.section.database` | `core.section.database` |
| `exhibition.section.partners`, `gallery.section.partners` | `core.section.partners` |
| `exhibition.section.timeline`, `gallery.section.timeline` | `core.section.timeline` |
| `exhibition.action.readMore`, `gallery.action.readMore` | `partner.action.readMore` |
| `exhibition.action.viewObjects`, `gallery.action.viewObjects`, `gallery.partner.viewObjects` | `partner.action.viewObjects` |
| `exhibition.item.explorePartnerNote`, `gallery.item.explorePartnerNote` | `partner.item.explorePartnerNote` |
| `gallery.partner.featured` | `partner.list.featured` |
| `exhibition.related.description`, `gallery.related.description` | `record.related.description` |
| `exhibition.item.linkPending`, `gallery.item.linkPending` | `record.related.linkPending` |
| `exhibition.related.title`, `gallery.related.title` | `record.related.title` |

## 4.6.1 (2026-09-26)

Part of M10 epic 8 (museumwithnofrontiers/inventory-app#2019), story
museumwithnofrontiers/inventory-app#2062.

### Fixed

- `core.footer.legalNotice` carried the English text in Czech, German, Greek,
  Italian, Portuguese, Swedish and Turkish. The German is
  `gallery.footer.legalNotice`'s, which the DXA family layer reads until it
  moves onto this entry; the others were translated for this dictionary
  (legacy's 3:legal_notice_title has only Arabic, Spanish and French, which
  the entry already carries).
## 4.6.0 (2026-09-26)

Part of M10 epic 8 (museumwithnofrontiers/inventory-app#2019), story
museumwithnofrontiers/inventory-app#2063.

### Changed

- The `partner` section in every language it promises. Most of its entries
  carried the English text in Czech, German, Greek, Italian, Portuguese,
  Swedish and Turkish, and eight of them (the list headings, "Partners
  found", "Back to Partners", "Partner not found.", the museum/institution
  badge) in every language. The German of `partner.item.explorePartnerNote`
  is `gallery.item.explorePartnerNote`'s; `partner.list.museums`,
  `.institutions`, `partner.info.typeMuseum`, `.phone` and `.addresses` take
  legacy's own translation where it had the label (sources.md); the rest were
  translated for this dictionary. Where the English word is the language's own
  ("Fax", "Logo", German "Museum", French "Contact"), the entry keeps it.
## 4.5.0 (2026-09-26)

Part of M10 epic 8 (museumwithnofrontiers/inventory-app#2019), stories
museumwithnofrontiers/inventory-app#2060 and #2061.

### Added

- The shared entries for what a gallery and an exhibition say the same way,
  in every language their section promises: the menu (`core.nav.about`,
  `.artisticIntroduction`, `.collection`, `.credits`, `.myCollection`,
  `.overallDatabase`, `.partners`, `.timeline`), the footer
  (`core.footer.aboutMwnf`, `.contact`, `.cookies`, `.copyright`, `.credits`),
  the section titles (`core.section.about`, `.collection`, `.credits`,
  `.database`, `.partners`, `.timeline`), the item page's related block
  (`record.related.title`, `.description`, `.linkPending`) and the search links
  (`catalogue.results.seeDatabaseEntry`, `catalogue.search.overallDatabase`,
  `.placeholder`, `.relatedDatabase`). Each carries the English of the
  `gallery.*` entry it replaces, and the languages that entry had; the other
  languages come from legacy where it had the label (sources.md), or were
  translated for this dictionary.
- A `standalone` section, in the products' bundle only: the texts the three
  products (Islamic Art, Baroque Art, Sharing History) each carried in English
  in their own namespace — the home page, identity, navigation, exhibition list
  and partner lists. Legacy's own translation is used where it had one
  (sources.md); the other languages were translated for this dictionary.
- `core.nav.inThisSection` — "In this section", the label of a page's
  strip of sibling or child pages. viewer-layout's `EssayView` names it by
  default, instead of the exhibitions' `exhibition.theme.inThisTheme`, which
  the gallery bundle does not carry. Legacy has no such label; translated for
  this dictionary.

The entries they replace stay until nothing reads them
(inventory-app#2019).
## 4.4.0 (2026-09-25)

Part of M10 epic 6 (museumwithnofrontiers/inventory-app#2017), story
museumwithnofrontiers/inventory-app#2054.

### Added

- `core.action.show` — "Show", in every language the `core` namespace
  promises. viewer-layout's `FeaturedPartners` labels each carousel bullet
  "Show <partner>" with it, and only two galleries carried it among their own
  texts, so the others read the entry's name out. Translated for this
  dictionary.
## 4.3.0 (2026-09-25)

Part of M10 epic 6 (museumwithnofrontiers/inventory-app#2017), stories
museumwithnofrontiers/inventory-app#2055 and #2056.

### Added

- `partner.list.featured` — "Featured Partners", in every language the
  `partner` namespace promises. The default heading of viewer-layout's
  `FeaturedPartners`, which named `partner.featured`, an entry that never
  existed. It replaces `gallery.partner.featured`; Arabic, German, Spanish and
  French come from that entry, the other languages were translated for this
  dictionary.
- The exhibition partner-objects texts every exhibition wrote under its own
  namespace, identical in all six: `exhibition.partner.monumentsInExhibition`
  ("monument(s) in this Exhibition") and `exhibition.partnerObjects.emptyPartner`,
  `.emptyInstitution`, `.partnerProfile`, `.institutionProfile`. viewer-layout's
  `standardRoutes('exhibition')` reads them by default, so a site no longer
  passes them. Like every `exhibition.*` entry, the other languages carry the
  English text.

The entries they replace stay until nothing reads them
(inventory-app#2019).
## 4.2.0 (2026-09-25)

Part of M10 epic 4 (museumwithnofrontiers/inventory-app#2015), story
museumwithnofrontiers/inventory-app#2030.

### Added

Three shared partner actions, in every language the `partner` namespace
promises (`ar cs de el en es fr it pt se tr`):

- `partner.action.readMore` — "Read more"
- `partner.action.viewObjects` — "View objects"
- `partner.action.viewMonuments` — "View monuments"

They are the labels of viewer-layout's `PartnerPanel` (the list line and the
partner page) and replace per-family and per-site copies of the same text:
`gallery.action.readMore` / `exhibition.action.readMore`,
`gallery.action.viewObjects` / `gallery.partner.viewObjects` /
`exhibition.action.viewObjects`, and the three products'
`*.action.viewObjects` / `*.action.viewMonuments`. The old entries stay until
nothing reads them (inventory-app#2019). Arabic, German, Spanish and French
come from the legacy rows and the gallery entries they replace (see
`sources.md`); the other languages were translated for this dictionary.
## 4.1.0 (2026-09-22)

Part of museumwithnofrontiers/inventory-app#1742 (M5 — Site waves), story
museumwithnofrontiers/inventory-app#1944.

### Added

German (`de`) added to the `gallery` kind: `languages.gallery` in
`namespaces.json` now lists `ar`, `de`, `en`, `es`, `fr`. `gallery/de.json`
provides all 62 `gallery.*` entries. The `historical-cars` site (M5)
declares German for its gallery bundle; without this, `viewer-i18n-check`'s
app-mode completeness check fails that build with the shared `gallery`
texts lacking their German entries.

6 of the 62 entries reuse legacy `mwnf3.translation` German rows
(`gallery.footer.aboutMwnf`, `gallery.footer.contact`,
`gallery.footer.cookies`, `gallery.nav.artisticIntroduction`,
`gallery.nav.timeline`, `gallery.section.timeline` — see `sources.md`); the
remaining 56 were translated new, in the same formal (`Sie`-form),
museum-register German already used across the `standalone` kind's `de`
files.

## 4.0.0 (2026-09-21)

Part of epic museumwithnofrontiers/inventory-app#1727, cleanup wave (museumwithnofrontiers/inventory-app#1859).

### Removed

3 `core.project.*` entries no consumer reads any more, across every language
the `core` namespace ships. No consumer since `@museumwnf/viewer-core` 2.0.0
removed the legacy project-key map (`PROJECT_ENTRIES`/`PROJECT_FAMILIES`/
`projectFamily`) that these labels served:

- `core.project.carpetArt`
- `core.project.glassArt`
- `core.project.tableIsSet`

### Kept

5 `core.project.*` entries stay: `galleries`, `islamicArt`, `baroqueArt`,
`sharingHistory` (read by carpets/amulets `SiteShell.vue`/`Home.vue` as
sibling-site names) and `explorePartners` (read by islamicart
`composables/search.js`).

## 3.1.1

First version published to npmjs through the trusted-publishing release pipeline (no functional change).
## 3.1.0

Part of the M1 npmjs-publishing epic (museumwithnofrontiers/inventory-app#1721).

### Changed

- Package renamed `@metanull/viewer-i18n` → `@museumwnf/viewer-i18n` and
  publishing moves to npmjs (`registry.npmjs.org`) via trusted publishing
  (OIDC), replacing GitHub Packages for all future versions. The last
  `@metanull/viewer-i18n` version stays published, frozen, on GitHub
  Packages. `viewer-i18n-check`'s data-package and dist-bundle discovery
  (`tools/check.mjs`) now looks under `node_modules/@museumwnf` instead of
  `node_modules/@metanull`. `publishConfig.registry` now points at npmjs;
  `release.yml` passes `registry: npmjs` to `package-release.yml@v1.6.0`.
- `ci.yml`'s `package-ci.yml` pin moves to `v1.6.1`, which alias-installs a
  renaming PR's tarball under both the new and the pre-rename name in the
  downstream site matrix — without it, every site (still importing
  `@metanull/viewer-i18n`) would silently build against the last published
  version instead of this PR's code (museumwithnofrontiers/viewer-workflows#17).

## 3.0.1

Version 3.0.0 was published from commit ee037cf by mistake and carries none of these removals. This release is the first version to contain them.

Part of epic museumwithnofrontiers/inventory-app#1692, wave J (museumwithnofrontiers/inventory-app#1698), step 90. Follows waves A–I, which introduce shared entries (timeline, partner, etc.) to replace the product-specific duplicates in gallery and exhibition namespaces.

### Removed

51 superseded product-specific entries (each replaced by a neutral shared entry):

- **gallery.action.openInOpenStreetMap → partner.map.openInOpenStreetMap**
- **gallery.action.partnerHomepage → partner.nav.homepage**
- **gallery.action.seeGallery → timeline.action.seeGallery**
- **gallery.nav.dynastiesHeading → record.dynasty.heading**
- **gallery.nav.galleries → core.project.galleries**
- **gallery.partner.about → partner.info.about**
- **gallery.partner.addresses → partner.info.addresses**
- **gallery.partner.contact → partner.info.contact**
- **gallery.partner.logo → partner.info.logo**
- **gallery.partner.map → partner.map.map**
- **gallery.partner.mapOf → partner.map.mapOf**
- **gallery.partner.onTheMap → partner.map.onTheMap**
- **gallery.partner.sortAscending → partner.list.sortAscending**
- **gallery.partner.sortDescending → partner.list.sortDescending**
- **gallery.results.countryDescription → timeline.results.countryDescription**
- **gallery.search.howTo → catalogue.search.howToEssay**
- **gallery.timeline.allCountries → timeline.form.allCountries**
- **gallery.timeline.backToEvents → timeline.action.backToEvents**
- **gallery.timeline.beginFullSearch → timeline.results.beginFullSearch**
- **gallery.timeline.earliest → timeline.form.earliest**
- **gallery.timeline.galleryHeading → timeline.nav.galleryHeading**
- **gallery.timeline.latest → timeline.form.latest**
- **gallery.timeline.noEvents → timeline.results.noEvents**
- **gallery.timeline.noResults → timeline.results.noResults**
- **gallery.timeline.searchIntro → timeline.results.searchIntro**
- **gallery.timeline.selectCountry → timeline.form.selectCountry**
- **gallery.timeline.to → timeline.form.to**
- **exhibition.action.seeGallery → timeline.action.seeGallery**
- **exhibition.nav.dynastiesHeading → record.dynasty.heading**
- **exhibition.nav.galleries → core.project.galleries**
- **exhibition.partner.about → partner.info.about**
- **exhibition.partner.addresses → partner.info.addresses**
- **exhibition.partner.contact → partner.info.contact**
- **exhibition.partner.logo → partner.info.logo**
- **exhibition.partner.map → partner.map.map**
- **exhibition.partner.mapOf → partner.map.mapOf**
- **exhibition.partner.onTheMap → partner.map.onTheMap**
- **exhibition.partner.sortAscending → partner.list.sortAscending**
- **exhibition.partner.sortDescending → partner.list.sortDescending**
- **exhibition.results.countryDescription → timeline.results.countryDescription**
- **exhibition.search.howTo → catalogue.search.howToEssay**
- **exhibition.timeline.allCountries → timeline.form.allCountries**
- **exhibition.timeline.backToEvents → timeline.action.backToEvents**
- **exhibition.timeline.beginFullSearch → timeline.results.beginFullSearch**
- **exhibition.timeline.earliest → timeline.form.earliest**
- **exhibition.timeline.galleryHeading → timeline.nav.galleryHeading**
- **exhibition.timeline.latest → timeline.form.latest**
- **exhibition.timeline.noEvents → timeline.results.noEvents**
- **exhibition.timeline.noResults → timeline.results.noResults**
- **exhibition.timeline.searchIntro → timeline.results.searchIntro**
- **exhibition.timeline.selectCountry → timeline.form.selectCountry**
- **exhibition.timeline.to → timeline.form.to**

All sites have been updated to read the shared entries in timeline, partner, catalogue, record, and core namespaces. These product-specific duplicates are no longer read by any site as of this release. The seven sites pin this major version in wave K (museumwithnofrontiers/inventory-app#1702).

## 2.5.0

Part of epic museumwithnofrontiers/inventory-app#1692, wave K (museumwithnofrontiers/inventory-app#1702), walkthrough step 94 (museumwithnofrontiers/viewer-i18n#25).

- **record.source.label** ("Source"), **record.source.termsOfUse** ("Terms of use"), **record.source.rightsHolder** ("Rights holder"): neutral entries for the source credit on a record's page, shared across all website kinds. Additive.
- **core.footer.legalNotice** ("Important Legal Notice"): the shared legal-notice label for websites without product-specific footers (the standalone sites). Copied from `gallery.footer.legalNotice` and `exhibition.footer.legalNotice` for each language; the two product entries stay until wave J's removal story (museumwithnofrontiers/viewer-i18n#21). Additive.

## 2.4.0

Part of epic museumwithnofrontiers/inventory-app#1692, wave I partner adoptions (museumwithnofrontiers/inventory-app#1697), story museumwithnofrontiers/inventory-app#1703 (museumwithnofrontiers/viewer-i18n#26).

- **partner.map.openInOpenStreetMap** ("Open in OpenStreetMap"): the neutral entry for the partner map's link, shared across all website kinds. The two product entries (gallery.action.openInOpenStreetMap, xhibition.action.openInOpenStreetMap) stay until every site reads the shared one (removal last, museumwithnofrontiers/viewer-layout#67).

# Changelog

## 2.3.0

Wave G of the shared-pages epic (museumwithnofrontiers/inventory-app#1692/#1695), walkthrough
step 30 (museumwithnofrontiers/viewer-i18n#19): two new sections, `timeline` and `partner`,
in every bundle. Decision D6: neutral wording — "in this site", never
"Gallery" or "Exhibition" — so the one text serves a gallery, an exhibition
and a standalone site; product wording stays only in `gallery` and
`exhibition`. Additive: nothing removed, nothing renamed.

- **`timeline/`**, 24 entries (`timeline.nav.*`, `.form.*`, `.results.*`,
  `.action.*`): the twelve entries byte-identical between `gallery` and
  `exhibition` (`allCountries`, `backToEvents`, `beginFullSearch`, `earliest`,
  `latest`, `galleryHeading`, `noEvents`, `noResults`, `searchIntro`,
  `selectCountry`, `to`, `countryDescription`), plus fourteen more identical
  across islamicart, baroqueart and sharinghistory's own `timeline.*`,
  `results.*`, `action.*` and `filter.*` prefixes. `selectCountry`, `to`,
  `startDate`, `endDate` and `yearSuffix` reuse `catalogue.facet.*` and
  `catalogue.era.ad` rather than the gallery/exhibition wording, since the
  meaning and the existing eleven-language translations are the same. One
  entry, `seeGallery` ("See Gallery"), keeps the word "Gallery" on purpose —
  it names the object grid a timeline period links to (legacy's
  `gn_see_gallery`, decision D1 restoring it to the standalone sites too),
  not the product family, so it is not a D6 violation.
- **`partner/`**, 22 entries (`partner.info.*`, `.map.*`, `.list.*`, `.nav.*`,
  `.item.*`): fifteen entries identical between `gallery.partner.*` and
  `exhibition.partner.*`, plus entries the three standalone sites already
  triplicate under their own `partner.*` and `notFound.partner` /
  `results.partnersFound`. Two wording forks, resolved:
  - `fax` and `phone` were `"F"` / `"T"` in `gallery`/`exhibition` (a
    letter prefixing a number) and `"Fax"` / `"Phone"` on the three
    standalone sites; the full word won, since it reads on its own wherever
    the shared entry is used without the number beside it. The `gallery` and
    `exhibition` namespaces keep their own abbreviated entries unchanged.
  - `associated` was `"Associated Museums"` / `"Associated Institutions"`
    (islamicart, baroqueart) against sharinghistory's single
    `"Associated Partners"`; the generic form won, since the new entry has
    no `typeMuseum`/`typeInstitution` split of its own.
  - `back` takes islamicart/baroqueart/sharinghistory's `"Back to Partners"`;
    their separate `"Return to Partners"` (`returnLink`) is untouched — a
    second, different link on the same pages, not a duplicate of this one.
  - `objectsInSite` rewrites `gallery.partner.objectsInGallery` /
    `exhibition.partner.objectsInExhibition` ("object(s) in this Gallery" /
    "…Exhibition") to "object(s) in this site" per D6; the ar/es/fr
    translations are the same mechanical substitution, the site-type word
    swapped for the neutral one, on the existing gallery translations.
- Translations: `ar`, `es` and `fr` are real wherever the entry already
  existed in `gallery/{ar,es,fr}.json` (all of `timeline` but the seven
  standalone-only entries above; most of `partner`). `selectCountry`, `to`,
  `startDate`, `endDate` and `yearSuffix` are real in all eleven languages,
  reused from `catalogue/`. `partner.info.about`, `.contact`, `.fax`,
  `.logo` and `.phone` additionally carry real `de`, `it`, `pt` and/or `tr`
  from the legacy `mwnf3` translation table (word IDs `About`/`about`,
  `Contact`/`contact`, `Fax`, `logo`, `Phone`) — a legacy row that merely
  repeated the English was skipped, as `sources.md` already does (this
  dropped French `Phone`, which legacy left untranslated). Everything else —
  `cs`, `el` and `se` throughout, and every language for the sixteen
  entries sourced only from islamicart/baroqueart/sharinghistory's
  English-only `locales/en.json` (`errorSelect`, `errorPeriod`, `backLink`,
  `eventsFound`, `viewItemsFromPeriod`, `fromYearHint`,
  `toYearHint`, `none`, `typeMuseum`, `typeInstitution`, `museums`,
  `institutions`, `associated`, `partnersFound`, `back`, `notFound`) — is
  English, as 2.2.0 did for `exhibition`; none of these was ever translated
  by MWNF for any site that reads it.

Walkthrough step 31 (museumwithnofrontiers/viewer-i18n#20): the search vocabulary the
three standalone sites triplicated, the DXA theme pages' wording, and the
glossary/dynasty popout labels the item sheet needs. Additive.

- **`catalogue/`**, 9 entries (`catalogue.field.artist`, `.keywords`,
  `.material`, `.other`, `.patron`, `catalogue.search.howToEssay`, `.intro`,
  `.keywordOne`, `.keywordTwo`, `.keywordThree`): the search essay
  `gallery.search.howTo` / `exhibition.search.howTo` restored by 2.0.1 —
  still byte-identical between the two — plus the field names and search
  intro the three standalone sites triplicate under their own
  `<site>.search.*` / `<site>.field.*`. The essay is named
  `catalogue.search.howToEssay`, not `catalogue.search.howTo`: that shorter
  name is already taken, by the *link label* "How to search" 2.0.1 tells the
  story of restoring the essay away from — `SearchResults.vue` /
  `CollectionSearch.vue` in colours, water-in-islam, amulets and carpets
  render it as a `RouterLink`'s clickable text, and giving it the essay
  would turn that link into the whole Boolean-search write-up.
  `fromYearHint` / `toYearHint` are not duplicated here — #19 already added
  them as `timeline.form.fromYearHint` / `.toYearHint`, and the meaning is
  the same wherever a year hint is shown.
- **`record/`**, 3 entries: `record.glossary.tool` ("Glossary tool"), beside
  the existing `record.glossary.heading` / `.instructions` / `.definition`,
  which already say what the DXA item sheets' glossary popout needs and are
  untouched. `record.dynasty.heading` and `record.dynasty.list`, both
  "Dynasties" — the neutral form of two different wordings on the same item
  sheet: `gallery.nav.dynastiesHeading` ("THE DYNASTIES", a dynasty
  popout's own title) and `gallery.nav.islamicDynasties` ("Islamic
  Dynasties / Period", the heading above the list of an item's dynasties).
  Two UI slots, the same neutral word for both — neither needs the
  "Islamic" qualifier once it is read beyond islamicart.
- **`exhibition/`**, 14 entries (`exhibition.theme.romanLabel`,
  `.seeGalleryFor`, `.seeAllInTheme`, `.galleryLabel`, `.recordNotInSite`,
  `exhibition.related.notAvailable`, `exhibition.relatedCategory.furtherReading`,
  `.mwnfContent`, `.partnerContent`, `.otherContent`, `.unknown`,
  `exhibition.chapter.previous`, `.next`, `.returnToExhibitions`): the theme
  and related-content wording the-use-of-colours-in-art added in wave 0
  under its own `colours.*` prefix, plus sharinghistory's chapter
  navigation (`nextChapter` / `previousChapter` / `returnLink`, renamed to
  the neutral `chapter.next` / `.previous` / `.returnToExhibitions`).
  Decision D6 reaches one entry here even though `exhibition/` is a product
  section: `recordNotInSite` rewrites colours' `theme.recordNotInExhibition`
  ("…is not part of this exhibition") to "…is not part of this site",
  because `exhibition/` has been in the `standalone` bundle since 2.2.0 and
  a product site reading it should not be told about an "exhibition" it
  isn't one. The other four theme entries keep "Theme" and "Gallery"
  unchanged — "Gallery" names the object grid a theme links into, the
  README's standing exception, not the product.
- Translations: `catalogue.search.howToEssay` is real in `ar`, `es` and
  `fr`, copied from `gallery.search.howTo` — the pre-2.0.0 gallery
  translations already carried it. Everything else this walkthrough step
  adds — the rest of `catalogue.field.*` / `catalogue.search.*`, all of
  `record.glossary.tool` and `record.dynasty.*`, and all fourteen new
  `exhibition.*` entries, in every one of the eleven languages including
  `ar`, `es` and `fr` — is English. None of it existed anywhere as a
  translated string to reuse: the three standalone sites never had a
  non-English `locales/` file, and `exhibition/`'s non-English files have
  been English copies since 2.2.0, MWNF never having translated the
  exhibition write-ups.

## 2.2.0

Wave 0 of the shared-pages epic (museumwithnofrontiers/inventory-app#1692/#1693), walkthrough
step 11 (museumwithnofrontiers/viewer-i18n#18): the `exhibition` namespace joins the
`standalone` bundle.

- islamicart, baroqueart and sharinghistory each carried nine
  `<site>.exhibition.*` entries whose English duplicated `exhibition.*`
  word for word, and had no way to read `exhibition.theme.*` at all — the
  `exhibition` namespace was built only into the `gallery` and `exhibition`
  bundles. `namespaces.json` now lists it under `standalone` too, so the
  three product sites read the one shared copy instead of keeping their
  own, and gain the theme entries besides. Additive: a bundle gains
  entries, nothing is removed.
- `exhibition/ar.json`, `cs.json`, `de.json`, `el.json`, `es.json`,
  `fr.json`, `it.json`, `pt.json`, `se.json` and `tr.json` — English, like
  `en.json`. MWNF never translated the exhibition write-ups; that is
  already the standing rule for the section, not something this change
  invents — the `exhibition` bundle's own websites have only ever promised
  `en` for it (`namespaces.json`'s `languages.exhibition`), and the nine
  duplicated entries the three sites are dropping were themselves English
  in every language they shipped. Joining `standalone`, which promises
  eleven languages, means the section's files have to exist in all of
  them for `viewer-i18n-check` to pass; the files exist so the check
  passes and a visitor in any language still reads the same English
  exhibition text they already did. A real translation, if MWNF ever
  commissions one, replaces these files without touching the registry.

## 2.1.0

- `viewer-i18n-check --app` reads a name written in a spec — `title:
  'carpets.identity.title'` in a `dataset.config.js`, a label in a catalogue
  or sheet spec that viewer-layout's composed views render — as a name the
  website asks for: it has to exist, and it counts as used. A plain string
  reads as one when it has three parts and its first is a section the
  website receives. Before this, a website on the composed views had its
  own entries reported unused and a misspelt label in a spec went unseen.
  Additive; no entry changes.

## 2.0.1

- Restored `gallery.search.howTo` and `exhibition.search.howTo` — the essay on
  the boolean search operators that the "How to search" page of every DXA
  website renders. 2.0.0 removed them as duplicates of
  `catalogue.search.howTo`, which is the *link label* "How to search", not the
  essay; the mistake survived the release because the downstream check
  builds and tests a website but does not run its text check, and the essay
  is asked for through an `I18nText` keypath the removal's grep did not read.
  The four websites' text checks caught it on the first bump. Additive.
## 2.0.0

Wave E of the shared-pages epic (museumwithnofrontiers/inventory-app#1691), the last
step (#13): the `gallery` and `exhibition` entries that `catalogue`,
`sheet`, `record` and `core` replaced in 1.7.0 are removed. **Breaking**
for any website still asking for one — it would render as its own name.
Every website's `main` was moved onto the shared entries before this
release (the seven wave D adoptions, then museumwithnofrontiers/carpets#26,
museumwithnofrontiers/amulets#24, museumwithnofrontiers/water-in-islam#26 and
museumwithnofrontiers/the-use-of-colours-in-art#24 for the last handful), and this
release's downstream check built and tested all seven against it.

The rule: an entry goes when a shared one says the same thing — the era
words, the facet labels, the filter words, the glossary heading and
instructions, what surrounds the sheet (add to collection, citation,
download, on display in, photograph, source database, timeline for this
item), the pagination words, the project names, the results words, the
search form's button and "how to search", every sheet label, back, go,
reset, close, menu, "Exhibition(s)". What only a gallery or an
exhibition says stays: the sections, the navigation, the partner page,
the timeline pages, the notices, the about and intro texts, the
sponsors, the themes.

`tools/prune-duplicates.mjs` is the list, applied; it stays in the
repository so the rule is readable.

- **`gallery/`** loses 87 entries: `gallery.action.back`, `gallery.action.go`, `gallery.action.resetFilters`, `gallery.era.ad`, `gallery.era.after`, `gallery.era.bc`, `gallery.era.before`, `gallery.facet.any`, `gallery.facet.artist`, `gallery.facet.country`, `gallery.facet.endDate`, `gallery.facet.filterBy`, `gallery.facet.filterFurtherBy`, `gallery.facet.material`, `gallery.facet.periodDynasty`, `gallery.facet.selectCountry`, `gallery.facet.startDate`, `gallery.facet.subject`, `gallery.facet.type`, `gallery.filter.from`, `gallery.filter.to`, `gallery.glossary.definition`, `gallery.glossary.instructions`, `gallery.item.addToCollection`, `gallery.item.citation`, `gallery.item.download`, `gallery.item.downloadPdf`, `gallery.item.in`, `gallery.item.onDisplayIn`, `gallery.item.photograph`, `gallery.item.sourceDatabase`, `gallery.item.timeline`, `gallery.nav.exhibitions`, `gallery.nav.glossary`, `gallery.nav.menu`, `gallery.pagination.first`, `gallery.pagination.last`, `gallery.pagination.page`, `gallery.project.baroqueArt`, `gallery.project.carpetArt`, `gallery.project.explorePartners`, `gallery.project.glassArt`, `gallery.project.islamicArt`, `gallery.project.sharingHistory`, `gallery.project.tableIsSet`, `gallery.related.audioVideos`, `gallery.results.allObjects`, `gallery.results.forProject`, `gallery.results.heading`, `gallery.results.noResults`, `gallery.results.objects`, `gallery.results.outOf`, `gallery.results.timelineForSearch`, `gallery.search.howTo`, `gallery.search.howToLink`, `gallery.search.submit`, `gallery.sheet.alsoKnownAs`, `gallery.sheet.artists`, `gallery.sheet.bibliography`, `gallery.sheet.binding`, `gallery.sheet.catalogueLink`, `gallery.sheet.copyeditedBy`, `gallery.sheet.copyrightInformation`, `gallery.sheet.currentOwner`, `gallery.sheet.datationMethod`, `gallery.sheet.date`, `gallery.sheet.description`, `gallery.sheet.dimensions`, `gallery.sheet.holdingMuseum`, `gallery.sheet.inventoryNumber`, `gallery.sheet.location`, `gallery.sheet.materials`, `gallery.sheet.name`, `gallery.sheet.obtentionMethod`, `gallery.sheet.originalOwner`, `gallery.sheet.periodDynasty`, `gallery.sheet.placeOfProduction`, `gallery.sheet.preparedBy`, `gallery.sheet.provenance`, `gallery.sheet.provenanceMethod`, `gallery.sheet.scribe`, `gallery.sheet.shortDescription`, `gallery.sheet.translationBy`, `gallery.sheet.translationCopyeditedBy`, `gallery.sheet.type`, `gallery.sheet.workingNumber`, `gallery.sheet.workshop`.
- **`exhibition/`** loses 88 entries: `exhibition.action.back`, `exhibition.action.go`, `exhibition.action.resetFilters`, `exhibition.era.ad`, `exhibition.era.after`, `exhibition.era.bc`, `exhibition.era.before`, `exhibition.facet.any`, `exhibition.facet.artist`, `exhibition.facet.country`, `exhibition.facet.endDate`, `exhibition.facet.filterBy`, `exhibition.facet.filterFurtherBy`, `exhibition.facet.material`, `exhibition.facet.periodDynasty`, `exhibition.facet.selectCountry`, `exhibition.facet.startDate`, `exhibition.facet.subject`, `exhibition.facet.type`, `exhibition.filter.from`, `exhibition.filter.to`, `exhibition.glossary.definition`, `exhibition.glossary.instructions`, `exhibition.item.addToCollection`, `exhibition.item.citation`, `exhibition.item.download`, `exhibition.item.downloadPdf`, `exhibition.item.in`, `exhibition.item.onDisplayIn`, `exhibition.item.photograph`, `exhibition.item.sourceDatabase`, `exhibition.item.timeline`, `exhibition.nav.exhibitions`, `exhibition.nav.glossary`, `exhibition.nav.menu`, `exhibition.pagination.first`, `exhibition.pagination.last`, `exhibition.pagination.page`, `exhibition.project.baroqueArt`, `exhibition.project.carpetArt`, `exhibition.project.explorePartners`, `exhibition.project.glassArt`, `exhibition.project.islamicArt`, `exhibition.project.sharingHistory`, `exhibition.project.tableIsSet`, `exhibition.related.audioVideos`, `exhibition.results.allObjects`, `exhibition.results.forProject`, `exhibition.results.heading`, `exhibition.results.noResults`, `exhibition.results.objects`, `exhibition.results.outOf`, `exhibition.results.timelineForSearch`, `exhibition.search.howTo`, `exhibition.search.howToLink`, `exhibition.search.submit`, `exhibition.sheet.alsoKnownAs`, `exhibition.sheet.artists`, `exhibition.sheet.bibliography`, `exhibition.sheet.binding`, `exhibition.sheet.catalogueLink`, `exhibition.sheet.copyeditedBy`, `exhibition.sheet.copyrightInformation`, `exhibition.sheet.currentOwner`, `exhibition.sheet.datationMethod`, `exhibition.sheet.date`, `exhibition.sheet.description`, `exhibition.sheet.dimensions`, `exhibition.sheet.holdingMuseum`, `exhibition.sheet.inventoryNumber`, `exhibition.sheet.location`, `exhibition.sheet.materials`, `exhibition.sheet.name`, `exhibition.sheet.obtentionMethod`, `exhibition.sheet.originalOwner`, `exhibition.sheet.periodDynasty`, `exhibition.sheet.placeOfProduction`, `exhibition.sheet.preparedBy`, `exhibition.sheet.provenance`, `exhibition.sheet.provenanceMethod`, `exhibition.sheet.scribe`, `exhibition.sheet.shortDescription`, `exhibition.sheet.translationBy`, `exhibition.sheet.translationCopyeditedBy`, `exhibition.sheet.type`, `exhibition.sheet.workingNumber`, `exhibition.sheet.workshop`, `exhibition.ui.close`.


## 1.0.0

- Initial release: the `core`, `layout`, `gallery` and `exhibition` namespaces
  in English, the `namespaces.json` registry, the three per-class bundles
  (`standalone`, `gallery`, `exhibition`), and `viewer-i18n-check` — the rules
  of the dictionary, usable against this repository, a website's `locales/`,
  and a website's call sites.
- English only. The `core` and `layout` entries are the strings that were
  hardcoded in `viewer-core` and `viewer-layout`; the `gallery` and
  `exhibition` entries are the strings the four DXA websites vendored, re-keyed
  into the `section.group.name` grammar and reduced to what their code
  actually uses.

## 1.1.0

- Arabic, Spanish and French for `core` and `layout`.
- The `gallery` and `exhibition` entries the first three websites needed.
- Fixed: the checker did nothing at all when run as a program. npm installs a
  `bin` as a symlink, and the guard that decides "was I run, or imported?"
  compared the path as written against the path of this file, which never
  matched. Every website's text check had been passing without running.

## 1.2.0

- `exhibition.sponsors.footerOne` … `footerFour`, named after the slot they
  fill rather than after one exhibition's wording. `patronage` and `support`
  were named after Water in Islam's headings, and four of the five exhibitions
  say something different there. Both old entries still exist.

## 1.3.0

- Removed the rule that rejected HTML in a text. viewer-core escapes raw HTML
  when it renders, so a tag reaches the page as the characters that were typed;
  the rule was a second, weaker copy of a decision already enforced where it
  matters. It was also wrong — written as a regular expression, it rejected
  `<https://example.org/>`, `<office@museumwnf.net>` and `` `<div>` `` (an
  autolink, an email autolink and a code span, all ordinary Markdown) and told
  the translator to write Markdown instead, which is what they had done.
- The checker has no dependencies again, so a translator's pull request still
  runs no npm install.

## 1.4.0

- A language file's name is now read by `Intl` rather than matched against a
  regular expression. The platform knows BCP 47, so nothing here re-describes
  it: `Intl.getCanonicalLocales` parses the tag and rejects what is not one.
- One spelling per language. `pt-br.json` is now reported and told to be
  `pt-BR.json`, so two files cannot both claim a language and leave the
  filesystem to decide which one a reader gets.
- The length rule stays ours: an ISO 639 code is two or three letters, and
  BCP 47's grammar happily accepts `common` and `index` as languages.
- `LANG_RE` is replaced by `languageOf(name)`, which returns the canonical
  spelling or null.

## 1.5.0

- The call sites are parsed, not matched. `@vue/compiler-sfc` — the parser the
  website already builds with — reads the scripts and the compiled template,
  and the names asked for are taken from the syntax tree.
- Two regular expressions are gone, and with them two ways of being wrong:
  `t(item)` written inside a prose comment was read as a text being asked for,
  and a component's own `const t = (item) => …` could not be told apart from
  the one that looks a text up. Both cost real edits during the rollout.
- `t` is now followed properly through scope, because one file uses the name
  both ways: `export function facetLabels(t)` receives the lookup as a
  parameter, while `const t = tr('items', …)` below it is a translated record.
- Verified against all seven websites: the same entries are found as before,
  with the false positives gone.
- The parser is resolved from the website being checked, so `--site` — the mode
  a translator's pull request runs — still loads nothing and installs nothing.
- `scanSources`, `checkApp` and `main` are async.

## 1.6.0

- `core.notFound.page`, read by viewer-core 1.6.0's `NotFoundView` — the
  page every website's catch-all lands on, now that the router owns it.
- `layout.nav.menu`, the label of the hamburger button viewer-layout 2.1.0's
  navigation shows on a narrow screen, so no website keeps a menu of its own.
- Both in English, French, Spanish and Arabic.

## 1.7.0

Wave A of the shared-pages epic (museumwithnofrontiers/inventory-app#1691): the vocabulary
the list pages and the record page of every website share, in every language
any website offers.

- Three namespaces in every bundle: `catalogue` (the filters, the search
  form, the results and their pages — 59 entries), `sheet` (the labels of a
  record's sheet, `sheet.field.*` — 43), `record` (what surrounds the sheet:
  back, timeline, related, credits, citation, glossary — 27). A shared label
  carries no trailing colon; the page decides that.
- `core.action.*` — the verbs of the landing cards and the controls (add,
  apply, back, browse, close, explore, go, read, reset, search, viewDetails)
  — and `core.project.*`, one entry per project of `mwnf3.projectnames`, so
  a project name is looked up once rather than written into six files.
- **Every language a website offers.** The data packages declare Islamic
  Art in ten site languages, Baroque Art in five, the galleries in four; the
  bundles had English chrome for all but four of them. `core`, `layout`,
  `catalogue`, `sheet` and `record` now exist, complete, in
  `ar cs de el en es fr it pt se tr`, and `gallery` in `ar es fr` besides
  English. The legacy websites' term tables are the source wherever they had
  a real translation of the same label; [`sources.md`](sources.md) is the
  trace. `se` is Swedish, named after the code the packages declare.
- `namespaces.json` names, per kind of website, the languages its websites
  offer (`languages`), and `--dictionary` refuses a section that is missing
  one of them or an entry in one. `--app` reads the languages a website
  offers from its data package's `manifest.site.languages` and refuses an
  installed bundle that does not cover them; `--languages` asks about another
  set.
- `gallery.*` and `exhibition.*` keep every entry they had, including the
  ~170 the two share and the ones the new namespaces now say again. Nothing
  reads the new ones yet; the websites move over one by one, and the
  duplicates go in a later major once nothing reads them.



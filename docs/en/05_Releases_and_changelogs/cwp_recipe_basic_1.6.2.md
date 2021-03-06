# 1.6.2

This release includes SilverStripe 3.6.7, which contains a critical security fix for CVE-2019-5715 (SS-2018-021). See
the [related blog post](https://www.silverstripe.org/download/security-releases/ss-2018-021) for details.

This recipe supersedes CWP recipe 1.6.1, which contains a conflict between packages silverstripe/multivaluefield and
symbiote/silverstripe-gridfieldextensions resulting in the package being installed twice. silverstripe/multivaluefield
was renamed to symbiote/silverstripe-gridfieldextensions, but must remain as the former in CWP 1.6. This problem does
not affect CWP recipes newer than 1.6.

We recommend upgrading to use the latest version of CWP if possible.

The changelog below contains all changes from CWP 1.6.1 as well as 1.6.2.

<!--- Changes below this line will be automatically regenerated -->

## Change Log

### Security

 * 2019-01-10 [c44f06cdf](https://github.com/silverstripe/silverstripe-framework/commit/c44f06cdf10387a987e4efb096ff06b3bb4495ef) Patch SQL Injection vulnerability when arrays are assigned to DataObject Fields (Aaron Carlino) - See [ss-2018-021](https://www.silverstripe.org/download/security-releases/ss-2018-021)
 * 2018-12-06 [bbd1a51](https://github.com/silverstripe-australia/silverstripe-multivaluefield/commit/bbd1a5194e61a77f149254124076313a629cf6c9) Adjust MultiValueField to work with the new scalarValueOnly method (Maxime Rainville) - See [ss-2018-021](https://www.silverstripe.org/download/security-releases/ss-2018-021)
 * 2018-09-26 [598edd913](https://github.com/silverstripe/silverstripe-framework/commit/598edd91341f389d7b919ec1201e03d2aba4d284) Add confirmation token to dev/build (Loz Calver) - See [ss-2018-019](https://www.silverstripe.org/download/security-releases/ss-2018-019)
 * 2018-05-08 [19fdebfa2](https://github.com/silverstripe/silverstripe-framework/commit/19fdebfa245506626561bc9626d9ac325acb14da) Remove dotm, potm, jar, css, js, xltm from default File.allowed_extensions (Robbie Averill) - See [ss-2018-014](https://www.silverstripe.org/download/security-releases/ss-2018-014)
 * 2018-04-11 [577138882](https://github.com/silverstripe/silverstripe-framework/commit/577138882163e4b8782ea043487944d30d88e753) Restrict non-admins from being assigned to admin groups (Damian Mooyman) - See [ss-2018-001](https://www.silverstripe.org/download/security-releases/ss-2018-001)
 * 2017-11-30 [6ba00e829](https://github.com/silverstripe/silverstripe-framework/commit/6ba00e829a9fb360dfe5cb0bc3d4544016c82357) Prevent disclosure of sensitive information via LoginAttempt (Damian Mooyman) - See [ss-2017-009](https://www.silverstripe.org/download/security-releases/ss-2017-009)
 * 2017-11-30 [db54112f3](https://github.com/silverstripe/silverstripe-framework/commit/db54112f3cca012e33257c782dffd7154bf663a5) Fix user agent invalidation on session startup (Damian Mooyman) - See [ss-2017-006](https://www.silverstripe.org/download/security-releases/ss-2017-006)
 * 2017-11-29 [22ccf3e2f](https://github.com/silverstripe/silverstripe-framework/commit/22ccf3e2f9092f51e7f7288ce108598c6f17b49c) Ensure xls formulae are safely sanitised on output (Damian Mooyman) - See [ss-2017-007](https://www.silverstripe.org/download/security-releases/ss-2017-007)
 * 2017-11-21 [0f2049d4d](https://github.com/silverstripe/silverstripe-framework/commit/0f2049d4d466e05f5d7f07fc63580836de8c6bff) Fix SQL injection in search engine (Daniel Hensby) - See [ss-2017-008](https://www.silverstripe.org/download/security-releases/ss-2017-008)
 * 2017-09-04 [f0262a8fd](https://github.com/silverstripe/silverstripe-framework/commit/f0262a8fd9ab5fb51b178ace3c3487351217f5a0) User enumeration via timing attack mitigated (Daniel Hensby) - See [ss-2017-005](https://www.silverstripe.org/download/security-releases/ss-2017-005)
 * 2017-05-25 [25b77a2ff](https://github.com/silverstripe/silverstripe-framework/commit/25b77a2ff8deabe8e8894002b9a5647eaec27b0a) SVG uploads disabled by default (Daniel Hensby) - See [ss-2017-017](https://www.silverstripe.org/download/security-releases/ss-2017-017)

### Features and Enhancements

 * 2017-08-24 [fdd501182](https://github.com/silverstripe/silverstripe-framework/commit/fdd501182e8403ef082c2954bb66e0b8b6dd7b71) Ability to override SS_TemplateManifest via Injector (fixes #7305) (Patrick Nelson)

### Bugfixes

 * 2019-02-20 [4d15355](https://github.com/silverstripe/cwp-recipe-basic/commit/4d15355a41b36819a85c311bd49b45346e8d67ce) Fix userforms to 4.3.1 (Robbie Averill)
 * 2019-01-23 [746c0679a](https://github.com/silverstripe/silverstripe-framework/commit/746c0679ad1d6ceac03d2adf167367f0ca2259cd) Injector may instantiate prototypes as if they're singletons (fixes #8567) (Loz Calver)
 * 2018-11-15 [86701b8cd](https://github.com/silverstripe/silverstripe-framework/commit/86701b8cd0cd5f8de813a7c9347e7c8055d878f4) Redirect loop with multiple URL tokens (fixes #8607) (Loz Calver)
 * 2018-06-04 [41e601a03](https://github.com/silverstripe/silverstripe-framework/commit/41e601a036307065d9ea2ba8862f67be738d402f) Regression from #8009 (Daniel Hensby)
 * 2018-06-01 [ce1db58](https://github.com/silverstripe/cwp/commit/ce1db58045b6b1cfcfda8cc2ef7d88d1a3e0f17d) Fix broken link (#92) (Raissa North)
 * 2018-06-01 [1012ccb](https://github.com/silverstripe/cwp/commit/1012ccbb4c231caae30faa398c4aca935c5a3048) Fix broken link (Raissa North)
 * 2018-06-01 [af89140](https://github.com/silverstripe/cwp/commit/af8914063d3a3a8298ef6c3936f72ddd51d7174d) Fix broken link in developer docs (#91) (Raissa North)
 * 2018-06-01 [60a98be](https://github.com/silverstripe/cwp/commit/60a98be6391ec70f7fc6c4847ed2c9f60a44686c) Fix broken links in developer docs (Raissa North)
 * 2018-05-29 [1cbf27e0f](https://github.com/silverstripe/silverstripe-framework/commit/1cbf27e0f47c3547914b03193d0f5f77c87ff8d5) PHP 5.3 compat for referencing $this in closure, and make method public for same reason (Robbie Averill)
 * 2018-05-18 [c7ab8df](https://github.com/silverstripe/cwp/commit/c7ab8df9d6b6deeaf05a66d026b348f0e784872d) Fix broken links (Raissa North)
 * 2018-04-22 [dca8ae5](https://github.com/silverstripe/cwp/commit/dca8ae53a678a9de964dc3b5bbc11c71fcd7b5d3) fix regex issue in performance docs (Tomas Cantwell)
 * 2018-04-17 [af3a9f3ec](https://github.com/silverstripe/silverstripe-framework/commit/af3a9f3ec8a5465f841c5aa8ee1faf40c1b76bf4) Duplicating many_many relationships looses the extra fields (fixes #7973) (UndefinedOffset)
 * 2018-03-15 [d17d93f7](https://github.com/silverstripe/silverstripe-cms/commit/d17d93f784a6e01f3d396c55adc623d69a90261a) Remove SearchForm results() function from allowed_actions (Steve Dixon)
 * 2018-02-16 [86addea1d](https://github.com/silverstripe/silverstripe-framework/commit/86addea1d2a7b2e28ae8115279ae358bcb46648a) Split HTML manipulation to onadd, so elements are not accidentally duplicated (Christopher Joe)
 * 2018-02-13 [c767e472d](https://github.com/silverstripe/silverstripe-framework/commit/c767e472dc494408460ef47c27b8d34475da4ac6) DataObject singleton creation (Jonathon Menz)
 * 2018-01-26 [416915b08](https://github.com/silverstripe/silverstripe-framework/commit/416915b08248285083518850ad8d015ca8ed25c2) tableName is blank in CompositeDBField-&gt;addToQuery (Dominik Beerbohm)
 * 2018-01-25 [cf69d0486](https://github.com/silverstripe/silverstripe-framework/commit/cf69d048665befa90eb43146f86cde984b876b3a) Fix ping including requirements (Damian Mooyman)
 * 2018-01-24 [c2cd6b383](https://github.com/silverstripe/silverstripe-framework/commit/c2cd6b3832c6bc4775b2742df593b445c2aca391) Fix Member_GroupSet::removeAll() (fixes #3948) (Loz Calver)
 * 2018-01-24 [f2b4c192e](https://github.com/silverstripe/silverstripe-framework/commit/f2b4c192ec4d70779f7c667a976e741a7f3a26c5) Fix UploadField cuts off “Save” button (closes #2862) (Loz Calver)
 * 2018-01-23 [7384e3fc2](https://github.com/silverstripe/silverstripe-framework/commit/7384e3fc25987742ea08af74b704857a936e8ec0) Gridfields with dropdowns having lots of overflow (Scott Hutchinson)
 * 2018-01-09 [2ef4a2d4e](https://github.com/silverstripe/silverstripe-framework/commit/2ef4a2d4ee86577b00311e65bbeb0439f7aaa1fc) , adding a missing return statement. (Nathan)
 * 2017-12-21 [44930f211](https://github.com/silverstripe/silverstripe-framework/commit/44930f211be3f658fc92f2d5318255de03078701) Allow HTML 5 input tags in FunctionalTest form submissions (Daniel Hensby)
 * 2017-12-14 [81150c592](https://github.com/silverstripe/silverstripe-framework/commit/81150c59225dbf1e95bb0b4dbcfbe18346f2bdff) Use PHP 5.3 array syntax (Daniel Hensby)
 * 2017-12-05 [8477de15](https://github.com/silverstripe/silverstripe-siteconfig/commit/8477de15203c4c80ca55365200fa3c7c031d70d8) Remove unused Behat tests from 3.6 branch (Robbie Averill)
 * 2017-11-30 [84d7afb34](https://github.com/silverstripe/silverstripe-framework/commit/84d7afb3477885e9d69f2ac10838179efc1d3b91) Use baseDataClass for allVersions as with other methods (Daniel Hensby)
 * 2017-11-24 [09a003bc1](https://github.com/silverstripe/silverstripe-framework/commit/09a003bc13390359fa717a4256f9278303d59544) Fix deprecated usage of getMock in unit tests (Daniel Hensby)
 * 2017-11-23 [2ad3cc07d](https://github.com/silverstripe/silverstripe-framework/commit/2ad3cc07d583041e23a5dca0d53ffbdf8c9cd0d0) Update meber passwordencryption to default on password change (Daniel Hensby)
 * 2017-11-22 [ef6d86f2c](https://github.com/silverstripe/silverstripe-framework/commit/ef6d86f2c695d319f9c07ccd9f4d93e83263e356) Allow lowercase and uppercase delcaration of legacy Int class (Daniel Hensby)
 * 2017-11-22 [ec8ad45](https://github.com/silverstripe/cwp/commit/ec8ad45609a1dc00899f34c7d48235d91f86a149) fix: added missing image for private modules (Tomas Cantwell)
 * 2017-11-16 [dda14e895](https://github.com/silverstripe/silverstripe-framework/commit/dda14e89596a0de0b70eace27f7015bc0bb40669) Fix HTTP::get_mime_type with uppercase filenames. (Roman Schmid)
 * 2017-11-16 [52f0eadd3](https://github.com/silverstripe/silverstripe-framework/commit/52f0eadd3b1ad37806a95b6dd05427add3166cc5) for #7606: Ensure the object we're handling is actually an Image instance before calling methods specific to that class (e.g. in case of using SVG's in &lt;img&gt; tag which may be File instances). (Patrick Nelson)
 * 2017-11-15 [ce3fd370f](https://github.com/silverstripe/silverstripe-framework/commit/ce3fd370fb07ffc18742323b0dd99f30cf28cf14) ManyMany link table joined with LEFT JOIN (Daniel Hensby)
 * 2017-11-09 [1053de7ec](https://github.com/silverstripe/silverstripe-framework/commit/1053de7ec39d1a2ce6826ea2db8f55114755098d) Don't redirect in force_redirect() in CLI (Damian Mooyman)
 * 2017-10-25 [cbac37559](https://github.com/silverstripe/silverstripe-framework/commit/cbac3755909bc5d72d923b07747fd6a98e2215dc) Helpful warning when phpunit bootstrap appears misconfigured (Daniel Hensby)
 * 2017-10-25 [32cef975e](https://github.com/silverstripe/silverstripe-framework/commit/32cef975ef6c816d8b5bc953cffbd18492686281) Use self::inst() for Injector/Config nest methods (Daniel Hensby)
 * 2017-10-19 [a73d5b41](https://github.com/silverstripe/silverstripe-cms/commit/a73d5b4177be445128a6fa42e20dd8df13eaf554) revert to this button after archiving (Christopher Joe)
 * 2017-10-12 [fd39faee](https://github.com/silverstripe/silverstripe-cms/commit/fd39faeefd5241cf96313e968142183de767c51b) UploadField overwriteWarning isn't working in AssetAdmin (Jason)
 * 2017-10-09 [264cec123](https://github.com/silverstripe/silverstripe-framework/commit/264cec1239ee8d75e67c5402970a91cf58e50539) Dont use var_export for cache key generation as it fails on circular references (Daniel Hensby)
 * 2017-10-04 [24e190ea](https://github.com/silverstripe/silverstripe-cms/commit/24e190ea8265d16445a3210f7b06de191e474004) Fix: TreeDropdownField showing broken page icons (fixes silverstripe/silverstripe-framework#7420) (Loz Calver)
 * 2017-09-28 [378c7fa](https://github.com/silverstripe-australia/silverstripe-multivaluefield/commit/378c7fa70461cbb36cb5bba664695dbb28f4286d) Return self for setValue (Daniel Hensby)
 * 2017-09-26 [ebe1de8d8](https://github.com/silverstripe/silverstripe-framework/commit/ebe1de8d8b5bc739e74b1001aec3110b6175a303) Fix ArrayList sort error with old (supported) PHP (Dylan Wagstaff)
 * 2017-09-12 [0aac4ddb](https://github.com/silverstripe/silverstripe-cms/commit/0aac4ddb7ecf0f17eda8add235017c10c9f57255) Default LoginForm generated from default_authenticator (Daniel Hensby)
 * 2017-09-12 [091d99f59](https://github.com/silverstripe/silverstripe-framework/commit/091d99f599dcacf6aef2ad1df48311c2399f150c) Authenticators are more resilient to incomplete configuration (Daniel Hensby)
 * 2017-08-28 [7b200a2a6](https://github.com/silverstripe/silverstripe-framework/commit/7b200a2a642a78bffcf0a2f417a4757fb216ecfb) Fix add combinedFiles to clear logic (Christopher Joe)
 * 2017-08-16 [eb80a5f9e](https://github.com/silverstripe/silverstripe-framework/commit/eb80a5f9e89e69480edc7f1c9c66cc7403f547f1) LastEdited no longer updated on skipped writes (Daniel Hensby)
 * 2017-08-14 [b04a1ab41](https://github.com/silverstripe/silverstripe-framework/commit/b04a1ab41c4051923e9d9a9af5dedfa5a3ef67d8) Fix Truncate Error Issue when using views in a Unittest. (James Pluck)
 * 2017-08-13 [2f579b64c](https://github.com/silverstripe/silverstripe-framework/commit/2f579b64cb9cb8986489e312b253dba5061e304b) Files without extensions (folders) do not have a trailing period added (Robbie Averill)
 * 2017-08-06 [59b28f7d5](https://github.com/silverstripe/silverstripe-framework/commit/59b28f7d5bcefd477766611a99643f121af3dc56) Fixes #7181 to config system for userland config of node display limits. (Russell Michell)
 * 2017-07-26 [31c5eebda](https://github.com/silverstripe/silverstripe-framework/commit/31c5eebda089867d61546106b36ca20b21a00026) Avoid JS errors for HTMLEditorFields in small holders (Daniel Hensby)
 * 2017-07-26 [82c0632f4](https://github.com/silverstripe/silverstripe-framework/commit/82c0632f46e00a251d287811652429036d200eff) Fix: Use Config API for MemberAuthenticator::$migrate_legacy_hashes (fixes #7208) (Loz Calver)
 * 2017-07-19 [292aaf653](https://github.com/silverstripe/silverstripe-framework/commit/292aaf65301b2be4bb5e6e1505ccbe98b8ade67f) Cache IDs grouped by site first (Daniel Hensby)
 * 2017-07-18 [b77274c1a](https://github.com/silverstripe/silverstripe-framework/commit/b77274c1a3c3ab8cfa0abf939aa2e4735e534171) Add unique prefix to cache stores to prevent cache leak (Daniel Hensby)
 * 2017-07-17 [515a7cb5](https://github.com/silverstripe/silverstripe-cms/commit/515a7cb569f0cf90787b44fca8845760b539fabe) Make sure VirtualPage renders correct templates (Daniel Hensby)
 * 2017-07-10 [960a0f834](https://github.com/silverstripe/silverstripe-framework/commit/960a0f8343e5ff8379906c2476af4b74da0fd9c9) Fix: Make File::ini2bytes() compliant with binary prefixes (fixes #7145) (Loz Calver)
 * 2017-07-09 [8f2aaf5](https://github.com/silverstripe/cwp/commit/8f2aaf5bc276628a60285157fdcd7c035b41f095) Fixed link formats in performance guide docs (Ingo Schommer)
 * 2017-07-06 [a6db16b22](https://github.com/silverstripe/silverstripe-framework/commit/a6db16b2298738e1ef1329329cbef7c6b33f993e) Fix OS X issue with `Convert::html2raw`, `HTMLText::FirstSentence`, `HTMLText::Summary` and `Text::FirstSentence`. (Roman Schmid)
 * 2017-07-06 [a8860d9](https://github.com/silverstripe/cwp/commit/a8860d90495e51de90b65f7ff0334803156dc3ae) Fix formatting errors (Glen Peek)
 * 2017-07-06 [3572328](https://github.com/silverstripe/cwp/commit/357232873526970d85c0ef7c5c327ada32cbdce0) Fix getBaseStyles examples (Glen Peek)
 * 2017-07-04 [00f1ad5d6](https://github.com/silverstripe/silverstripe-framework/commit/00f1ad5d692f0a44b58bb216e5378e51dc96243d) Fixes #7116 Improves server requirements docs viz: OpCaches. (Russell Michell)
 * 2017-06-29 [79a7b1016](https://github.com/silverstripe/silverstripe-framework/commit/79a7b1016e6046af4f07fcd8bfb40773d1066b7e) add missing $rootCall param from LeftAndMain (Daniel Hensby)
 * 2017-06-20 [e2116a70e](https://github.com/silverstripe/silverstripe-framework/commit/e2116a70ef34433bfe712b4164ae416a76d4430d) Text colour in GridField filter headers for dropdown fields (Robbie Averill)
 * 2017-06-14 [b33a16a](https://github.com/silverstripe/cwp/commit/b33a16a6520e577faaa09630925ffc12b3aa93f4) Fix ADFS docs to account for DR instances (John)
 * 2017-06-14 [2afe018dc](https://github.com/silverstripe/silverstripe-framework/commit/2afe018dc7e380ac84f8e1f7986ce0247e9a254b) Ensure HasManyList foreign ID filter includes table name (fixes #7023) (Loz Calver)
 * 2017-06-14 [1073eca2f](https://github.com/silverstripe/silverstripe-framework/commit/1073eca2fac1b05c0e20b02aea78e8a2f550cfe5) Bugfix: Complex (curly) syntax (Marcz Hermo)
 * 2017-06-14 [fd57bd910](https://github.com/silverstripe/silverstripe-framework/commit/fd57bd9100634682fc5b2d9f493e3c54ce0444ad) Update help link from 3.5 to 3.6 (Robbie Averill)
 * 2017-06-12 [53c84d93d](https://github.com/silverstripe/silverstripe-framework/commit/53c84d93da0f0681fdcb3a061ebe529fd3cd9a9e) Fix changetracker checkbox bugs (Brian Cairns)
 * 2017-06-12 [f0c00bfb7](https://github.com/silverstripe/silverstripe-framework/commit/f0c00bfb7819c0350fa882f899d0c820a2aefa81) Fixing language typo in docs (3Dgoo)
 * 2017-06-12 [a5c84b12a](https://github.com/silverstripe/silverstripe-framework/commit/a5c84b12ab3c0759f696fc48fee3475bab6b3e20) Order of conditionals for getting default admin (Daniel Hensby)
 * 2017-06-06 [4ad2cae86](https://github.com/silverstripe/silverstripe-framework/commit/4ad2cae8642d21e37b5132e4040ca45d2d66c193) Upload_Validator failed to fetch max size from PHP ini values (fixes #6999) (Loz Calver)
 * 2017-06-05 [5f5bfa5e7](https://github.com/silverstripe/silverstripe-framework/commit/5f5bfa5e7045cc96f89fca417f0a7d99dc662fab) Fix create temp folder if it does not exist (Christopher Joe)
 * 2017-06-02 [a52ed03b4](https://github.com/silverstripe/silverstripe-framework/commit/a52ed03b49b8f62573eb3e295bfde84d1ef68f46) Upgrade old style constructors that were missed (Daniel Hensby)
 * 2017-06-02 [4b9d5dceb](https://github.com/silverstripe/silverstripe-framework/commit/4b9d5dceb892a9c41925d058d953a8849b407276) Fix tinymce image selection issue in newer versions of Chrome (Christopher Joe)
 * 2017-05-29 [b4368196d](https://github.com/silverstripe/silverstripe-framework/commit/b4368196d1bcee9fd1714b044c8ae6580c7941c9) Use plural name for ModelAdmin tab name (Robbie Averill)
 * 2017-05-09 [3dd303679](https://github.com/silverstripe/silverstripe-framework/commit/3dd3036792962d5384a72aa0132a64aca7d2ebc2) Ensure GridState_Component is added to GridField config even if we set config with GridField::setConfig (Klemen Dolinsek)
 * 2016-10-21 [8e5bb6fbd](https://github.com/silverstripe/silverstripe-framework/commit/8e5bb6fbdce0b2ca2d08a45534df2264db5e6b12) Fix : relObject() should return null if one of the node is null (Jason)
 * 2016-08-15 [0fbe9c7](https://github.com/silverstripe/cwp/commit/0fbe9c7ee974f1f36b4723a4914231c346d5940d) fix formatting (Jake Ovenden)
 * 2016-08-04 [2fa550e](https://github.com/silverstripe/cwp/commit/2fa550eacf2f0fee8e93ccc26165fe3ecbcb688e) fix typo (Jake Ovenden)
 * 2016-03-20 [805c38f10](https://github.com/silverstripe/silverstripe-framework/commit/805c38f107e7e332d2846407e0a89cade1d33ed1) don't try and switch out of context of the tab system (Stevie Mayhew)
 * 2016-03-15 [22b3a71ec](https://github.com/silverstripe/silverstripe-framework/commit/22b3a71ec0c8cd8c38030fa0bf5449abefafe8a3) fixing val reference to url in https hotlink (Denise Rivera)
 * 2015-04-22 [1f63637b9](https://github.com/silverstripe/silverstripe-framework/commit/1f63637b9369d4644a92523ada5d1a5dc0576c12) for #4095, TinyMCE not able to modify props of embed media (bug 1) and invalid HTML inserted (bug 2) (Patrick Nelson)

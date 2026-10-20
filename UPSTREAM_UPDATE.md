# Upstream update: Bnyro/GermanProviders

> This file is generated automatically. The Nuvio JavaScript providers are NOT overwritten automatically.

## Commits

- 41e7d9f huhu: migrate to new API endpoints
- ab3823c ci: bump actions versions
- 6e90e61 xcine: remove service (all sites dead)

## Changed Kotlin files

### hdfilme

- M HDFilme/src/main/kotlin/com/bnyro/HDFilme.kt

### huhuto

- M HuhuTo/src/main/kotlin/com/bnyro/HuhuTo.kt
- D HuhuTo/src/main/kotlin/com/bnyro/HuhuToExtractor.kt
- D HuhuTo/src/main/kotlin/com/bnyro/HuhuToLIve.kt
- M HuhuTo/src/main/kotlin/com/bnyro/HuhuToPlugin.kt

### Unmapped / needs review

- D Xcine/src/main/kotlin/com/bnyro/KinoKisteClub.kt
- D Xcine/src/main/kotlin/com/bnyro/Movie4k.kt
- D Xcine/src/main/kotlin/com/bnyro/Streamcloud.kt
- D Xcine/src/main/kotlin/com/bnyro/XCineBase.kt
- D Xcine/src/main/kotlin/com/bnyro/XCineExtractors.kt
- D Xcine/src/main/kotlin/com/bnyro/XCinePlugin.kt
- D Xcine/src/main/kotlin/com/bnyro/XcineRU.kt

## Other changed files

- M .github/workflows/build.yml
- M HuhuTo/build.gradle.kts
- D Xcine/build.gradle.kts
- D Xcine/src/main/AndroidManifest.xml
- M build.gradle.kts

## Nuvio files to review

- src/hdfilme/index.js → likely review target
- src/huhuto/index.js → likely review target

## Upstream comparison

- Previous: 7670925f8026ae1a094fff5a5e253fa157316a6c
- Current: 41e7d9f2283f35aa3ff749dd9f8e73c4e28ea625
- Compare: https://github.com/Bnyro/GermanProviders/compare/7670925f8026ae1a094fff5a5e253fa157316a6c...41e7d9f2283f35aa3ff749dd9f8e73c4e28ea625

## Porting procedure

1. Review the upstream Kotlin diff.
2. Check the corresponding src/<provider>/index.js.
3. Port only the functional changes that apply to Nuvio.
4. Run `npm ci && npm run build && npm test`.
5. Test the affected provider in Nuvio before merging.

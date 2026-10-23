# Upstream update: Bnyro/GermanProviders

> This file is generated automatically. The Nuvio JavaScript providers are NOT overwritten automatically.

## Commits

- bf02f1f hdfilme: fix crashes when series has no stream sources available
- 3811024 moflix: set user agent to something that is not cloudflared
- b98e22b filmfrei: rewrite provider from scratch (new website layout)

## Changed Kotlin files

### filmfrei24

- M FilmFrei24/src/main/kotlin/com/bnyro/FilmFrei.kt

### hdfilme

- M HDFilme/src/main/kotlin/com/bnyro/HDFilme.kt

### moflix

- M Moflix/src/main/kotlin/com/bnyro/Moflix.kt

## Other changed files

- M FilmFrei24/build.gradle.kts
- M HDFilme/build.gradle.kts
- M Moflix/build.gradle.kts

## Nuvio files to review

- src/filmfrei24/index.js → likely review target
- src/hdfilme/index.js → likely review target
- src/moflix/index.js → likely review target

## Upstream comparison

- Previous: 3fe86ddf4dc789392cf53f4c66716c17c4fb0f36
- Current: bf02f1f8da8478d6513eb5678b3f380bdb226521
- Compare: https://github.com/Bnyro/GermanProviders/compare/3fe86ddf4dc789392cf53f4c66716c17c4fb0f36...bf02f1f8da8478d6513eb5678b3f380bdb226521

## Porting procedure

1. Review the upstream Kotlin diff.
2. Check the corresponding src/<provider>/index.js.
3. Port only the functional changes that apply to Nuvio.
4. Run `npm ci && npm run build && npm test`.
5. Test the affected provider in Nuvio before merging.

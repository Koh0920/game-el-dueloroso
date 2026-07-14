# El Dueloroso (Game Boy homebrew) — Ato game capsule

A static-web "click and play" capsule for [Ato](https://ato.run): a Dockerfile
that serves EmulatorJS + the game's freely-licensed ROM. Emulation runs
client-side (WebAssembly).

License: GPL-3.0 (Adrián J.G.). Full attributions in `site/licenses/`.

The ROM is NOT stored here. The Dockerfile fetches the v1.2 release asset from
the author's GitHub repository and verifies SHA-256
`cdce1719ba652df43ca0d2f818f9f082afd21fadaa24e5d71f88f02c8b9ba760`.

The player is pinned to EmulatorJS v4.2.3. Its distribution zip, Gambatte npm
package, and source tarball are each SHA-256 verified; the source tarball digest
is `7dde1d271379d884bd433a1153d6f24b027180363141a300bb94cb81a287d6d1`.
The capsule also ships local EmulatorJS/Gambatte license texts and the Gambatte
package notice. Both Docker base images are pinned by immutable digest.

Run `tests/verify-reproducibility.sh` for the repository's static supply-chain
checks.

Not affiliated with, endorsed by, or connected to Nintendo / id Software / Bethesda.

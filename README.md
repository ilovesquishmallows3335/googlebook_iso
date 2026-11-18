# gbOS86 build workflow

1. Create a new GitHub repo (or fork linuxkid473/gbos-x86).
2. Copy `.github/workflows/build.yml` into it and push.
3. Actions tab -> "build-gbos86" -> Run workflow.
4. Download the artifact, then rebuild the image:

       cat gbOS86.img.zst.part-* | zstd -d > gbOS86.img

5. Flash with balenaEtcher / Rufus / dd. Boot with Secure Boot off.

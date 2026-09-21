# reciters

Quran recitations: full-surah recordings, the per-ayah splits cut from them,
and the timestamp files that line the two up.

```
reciters/<Reciter_Name>/<Surah>.mp3        the full recording
reciters/<Reciter_Name>/<Surah>/N.mp3      ayah N, cut from it
reciters/<Reciter_Name>/<Surah>/*.vtt|srt  where each ayah falls in the full recording
```

The mp3s are tracked with Git LFS, so a clone needs `git lfs install` first or
it yields pointer files. The Audacity projects the mp3s are exported from are
hundreds of MB each and stay local — see `.gitignore`.

## Quran Studio

The memorization app that used to live in `quran-studio/` here has moved to its
own repository: **[byStrange/quran-studio](https://github.com/byStrange/quran-studio)**.
It was never about these recordings — it reads its audio from the quran.com
catalogue — and sharing a repo meant one set of tags, one CI configuration and
one issue tracker for two unrelated things. The history came with it; this
repo's history still holds every commit up to the split.

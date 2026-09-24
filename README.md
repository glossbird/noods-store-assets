# NOODS Store Assets

Marketing images for NOODS Operator listings on the Steam Item Store: icons and
store screenshots, one folder per Operator per version.

This repo is public because Steam fetches these images over HTTPS when a
catalog is uploaded. Nothing else here is meant for an outside reader.

```
archive/<operator>/v<version>/
  icon.png
  icon_large.png
  store_image_1.png
  ...
```

Images are Git LFS, so URLs must use `media.githubusercontent.com/media/`.
The `raw.githubusercontent.com` host returns the LFS pointer file with a 200
status instead of the image.

Folders are added by the graduation export tool. Nothing here is edited by
hand, and a published version is never changed after the fact: a corrected
image goes in a new version folder, because the old URL may already be live
on a store listing.

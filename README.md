# vue-img-file-name-dd-repro

## Steps to reproduce
1. `yarn install`
2. `yarn run serve`
3. Navigate to the served page
4. Open web console
5. Note that the logo image served is suffixed by `logo.$HASH..png` instead of `logo.$HASH.png`
6. Try again with version `5.0.0-beta.6` (package.json)
7. Note that the logo image served is `logo.$HASH.png`, as it should be

## What is expected?
Image file name should be `logo.$HASH.png` (excl. file hash from the name)

## What is actually happening?
Image file name is `logo.$HASH..png` (excl. file hash from the name)

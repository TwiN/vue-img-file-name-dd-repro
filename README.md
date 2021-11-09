# vue-img-file-name-dd-repro

## Steps to reproduce
1. `yarn install`
2. `yarn run serve`
3. Navigate to the served page
4. Open web console
5. Note that the logo image served is suffixed by `..png` instead of `.png`
6. Try again with version `5.0.0-beta.6` (package.json)
7. Note that the logo image served is suffixed by `.png`, as it should be

## What is expected?
Image file name should be `logo.png` (excl. file hash from the name)

## What is actually happening?
Image file name is `logo..png` (excl. file hash from the name)

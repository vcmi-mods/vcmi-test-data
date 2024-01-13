# vcmi-test-data

Test data needed to run automatic unit tests for VCMI engine. The data is for VCMI Github Actions internal use only.

# h3_assets.zip
AES256 encrypted zip: https://askubuntu.com/a/1125254/838763

Compress:
put into h3_assets folder Data of HOMM3 without VIDOE.VID 
7za a -tzip -p -mem=AES256 h3_assets.zip h3_assets

Extract:
7za x h3_assets.zip -p$PASSWORD

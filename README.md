
rm -rf site
rm -rf playground-techdocs

git clone https://github.com/c4rth/playground-techdocs.git


# Python

## create venv
python3 -m venv ./py-mkdocs   
source ./py-mkdocs/bin/activate

## install mkdocs & c°
python3 -m pip install zensical mkdocs mkdocs-techdocs-core mkdocs-section-index mkdocs-git-revision-date-localized-plugin zensical


# Techdocs CLI

## MkDocs

npx @techdocs/cli generate --source-dir ./sample001 --output-dir ./site/ --no-docker --verbose --defaultPlugin

npx @techdocs/cli publish --publisher-type azureBlobStorage --storage-name techdocs-storage --entity default/component/ext-generated-component --azureAccountName stblobcarth

## Zensical

npx @techdocs/cli generate --source-dir ./sample-zensical --output-dir ./site/ --no-docker --verbose --engine zensical

npx @techdocs/cli publish --publisher-type azureBlobStorage --storage-name techdocs-storage --entity default/component/sample-zensical --azureAccountName stblobcarth

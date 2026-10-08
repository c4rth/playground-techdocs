
rm -rf site
rm -rf playground-techdocs

git clone https://github.com/c4rth/playground-techdocs.git


# Python

## create venv
python3 -m venv ./py-mkdocs   
source ./py-mkdocs/bin/activate

## install mkdocs & c°
python3 -m pip install mkdocs mkdocs-techdocs-core mkdocs-section-index


# Techdocs CLU

npx @techdocs/cli generate --source-dir ./sample001 --output-dir ./site/ --no-docker --verbose --defaultPlugin

npx @techdocs/cli publish --publisher-type azureBlobStorage --storage-name techdocs-storage --entity default/component/ext-generated-component --azureAccountName stblobcarth

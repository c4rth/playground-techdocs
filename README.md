
rm -rf site
rm -rf playground-techdocs

git clone https://github.com/c4rth/playground-techdocs.git

techdocs-cli generate --source-dir ./sample001 --output-dir ./site/ --no-docker --verbose

techdocs-cli publish --publisher-type azureBlobStorage --storage-name techdocs-storage --entity default/component/ext-generated-component --azureAccountName stblobcarth


# Python
source ./py-mkdocs/bin/activate

## install mkdocs
python3 -m pip install mkdocs mkdocs-techdocs-core mkdocs-section-index
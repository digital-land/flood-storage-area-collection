# Flood storage area collection  ⚠️ Centralised

[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/digital-land/brownfield-land/blob/master/LICENSE)
[![Run pipeline](https://github.com/digital-land/flood-storage-area-collection/actions/workflows/run.yml/badge.svg)](https://github.com/digital-land/flood-storage-area-collection/actions/workflows/run.yml)

A collection of flood storage areas collected from the Environment Agency.

The national dataset is in a format consistent with other Digital Land datasets as defined by the [flood-storage-area schema](https://github.com/digital-land/specification/blob/main/content/dataset/flood-storage-area.md?plain=1).


# Updating the collection

We recommend working in [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) before installing the python [requirements](requirements.txt), [makerules](https://github.com/digital-land/makerules) and other dependencies. Requires Make v4.0 or above.

    $ make makerules
    $ make init
    $ make collect

# Nightly collection

The collection is [updated nightly](https://github.com/digital-land/flood-storage-area-collection/actions) by the [GitHub Action](.github/workflows/run.yml).

# Building the national dataset

The collected files can then be converted into a national dataset:

    $ make

# Licence

The software in this project is open source and covered by the [LICENSE](LICENSE) file.

Individual datasets copied into this repository may have specific copyright and licensing, otherwise all content and data in this repository is
[© Crown copyright](http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/copyright-and-re-use/crown-copyright/)
and available under the terms of the [Open Government 3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) licence.
Installation::

    $ pip install https://github.com/dbrnz/flatmap-datamaker/releases/download/0.1.0/datamaker-0.1.0-py3-none-any.whl


Usage::

    $ mapdatamaker --help

    usage: mapdatamaker [-h] WORKSPACE COMMIT MANIFEST DATASET

    Create a SPARC Dataset of a flatmap's sources on PMR

    positional arguments:
      WORKSPACE   URL of a PMR workspace containing a flatmap manifest
      COMMIT      SHA of workspace commit to use for dataset
      MANIFEST    name of flatmap manifest in workspace
      DATASET     full mame for resulting dataset

    optional arguments:
      -h, --help  show this help message and exit


Example::

    $ mapdatamaker \
             https://models.physiomeproject.org/workspace/62f \
             1018a30afc1a675fcc6aa504204a0652ca059dff \
             manifest.json \
             dataset.zip
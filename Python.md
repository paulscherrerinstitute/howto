# Overview
This document describes how to use and work with  the central (Anaconda) Python Controls provide and supports on all GFA Linux systems.

Right now Controls supports a Python 2.7 and 3.5 installation. By default, none of these Python environments are loaded by default (because of various reasons).

It is highly recommended to use Python 3.5. This is especially true for new Python applications.

To use these installations execute following commands:

Python 3.5:
```bash
source /opt/gfa/python 3.5
```

Python 2.7:
```bash
source /opt/gfa/python 2.7
```

Note: While sourcing `/opt/gfa/python` your `PATH` variable will be expanded to include the central Python. If there is a `PYTHONPATH` this variables gets unset.

# Packages
Provided Packages
To show the installed packages and their respective version number use:

```bash
conda list
```

Missing/Updating Packages
In case packages are missing or need to be upgraded please contact daq[at]psi.ch .

New Packages
In case you want to provide an own package please contact daq[at]psi.ch .

# Environments
(Anaconda) Python Environments are a nice way of having customized Python environments e.g. for a specific application, testing or application development.

These are the commands available to work with conda environments:

List existing environments
```bash
conda env list
```

Activate environment
```bash
source activate <my environment>
```

Deactivate environment
```bash
source deactivate
```

## Central Environments
Central environments are hosted at the same location as the base Python distribution.

Central environments are a good option for extensive Python applications as well as for beamlines and/or groups. To request a central environment, the responsible for that environment should provide a package list and a name for the environment. This request has to be filed to daq[at]psi.ch. Each central environment needs to have a responsible specified!

# msi-utils

This Python package helps with investigating or analyzing MSI tools by providing information that is helpful when you need to extract info from a MSI (Windows Installer) file.

## Getting Started

To get started, you will need to have a Windows MSI installer available that you want to investigate.  Also you will will need to install this package.

### Installing

You can install this package via `pip` by running the following command:

```
pip install msi-utils
```

You can also install from this repository by first cloning this repo and then running:

```
python3 setup.py install
```

## Using

There are several different ways you can use the cmdline tool portion of `msi-utils`.  Here are the possible commands you can use:

```
msi-utils dump tables ~/my_file.msi 
msi-utils dump streams ~/my_file.msi 
msi-utils dump signature ~/my_file.msi 

msi-utils extract msi ~/my_file.msi 
msi-utils extract stream ~/my_file.msi "stream_name01"

msi-utils get streams ~/my_file.msi
msi-utils get tables ~/my_file.msi
msi-utils get summary ~/my_file.msi
```

## Built With

* [carcass](https://github.com/MSAdministrator/carcass) - Python packaging template

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. 

## Authors

* Josh Rickard - *Initial work* - [MSAdministrator](https://github.com/MSAdministrator)

See also the list of [contributors](https://github.com/MSAdministrator/msi-utils/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details

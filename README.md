# vhdldep

[![CI status](https://github.com/dominiksalvet/vhdldep/workflows/CI/badge.svg)](https://github.com/dominiksalvet/vhdldep/commits)
[![GitPack](https://img.shields.io/badge/-GitPack-571997)](https://github.com/dominiksalvet/gitpack)
[![standard-readme compliant](https://img.shields.io/badge/readme_style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)

> Simple VHDL dependency generator.

The development of VHDL projects very often involves building multiple VHDL files. Based on designed architecture, some files must be built before others. That might cause problems with finding the correct build order. And that is exactly where vhdldep comes in handy.

Vhdldep analyzes use statements of given VHDL files and returns their **file dependencies in a makefile format**. That output can be easily used to determine the correct build order to help automate building VHDL projects.

## Install

Vhdldep uses [GitPack](https://github.com/dominiksalvet/gitpack). Local installation/update:

```sh
gitpack install github.com/dominiksalvet/vhdldep
```

## Usage

Get **VHDL file dependencies**:

```
vhdldep <file>
```

With **custom prefix** for generated paths:

```
vhdldep -p <prefix> <file>
```

### Example

<p align="center">
    <img src="img/example.png" alt="vhdldep example">
</p>

The *alu.vhdl* file has been borrowed from the [Limen Alpha](https://github.com/dominiksalvet/limen-alpha) processor.

## Contributing

Do you want to contribute? Do you have any questions? Then the [*CONTRIBUTING.md*](CONTRIBUTING.md) file is here for you.

## License

This project is licensed under the [MIT License](LICENSE).

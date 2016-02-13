WPILib Mirror
=============

This repository is meant to be a clone of `~/wpilib` in a typical install.
This allows teams to pull a mirror quickly, for automated testing.

Usage
=====

In your `.travis.yml`, add the following line:

```yaml
install:
- git clone https://github.com/chopshop-166/wpilib-mirror.git ~/wpilib && ~/wpilib/bootstrap
```

Changes to Base WPILib
======================

* This `README.md`
* `build.properties` has the team number removed
	* This should be set in the team's repository
* `.gitattributes`
	* Allows file tracking using [git lfs][], which should be a bit less of a data burden
* `bootstrap`
	* Bash script to download [git lfs][] an use it to pull binary files

[git lfs]: https://git-lfs.github.com/

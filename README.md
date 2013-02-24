# Unitify

> A CLI to run Unit tests and create code coverage reports using PHPUnit.

`PHPUnit` is a really great PHP Unit Testing framework. But have you ever wondered why the CLI is so ugly?

`Unitify` is a more beautiful and structured alternative that works with PHPUnit internally.

## How to use

You can download and install the CLI like so:

	$ php -r "$(curl -fsSkL raw.github.com/vis7mac/unitify/master/install)"

After that, you should be able to access the binary `unitify`.

## Requirements

The only change to your repository might be the addition of a `phpunit.xml` file in the root of the repository.

You can find more information on this here: <http://www.phpunit.de/manual/current/en/appendixes.configuration.html>

## FAQs

- "What does 'Determined the PHPUnit testing root' mean?"
	
	Unitify auto-detects the root of your installation based on the `phpunit.xml` file. So you can be in any subdirectory of your repository and Unitify finds the way back for you and runs `phpunit` there.

- "Can I change the installation path of Unitify?"
	
	Yes, of course. Simply add the path to the installation script:
	
		$ php -r "$(curl -fsSkL raw.github.com/vis7mac/unitify/master/install)" PATH
	
	You can also install an existing installation to a new path:
	
		$ unitify install PATH
	
	`Unitify` is a one-file binary without any library files and does not require anything but an installed `phpunit`. So you can basically install it everywhere in your `$PATH`.

### Contact

If you have any further questions, don't hesitate to contact me: <lukas@lu-x.me>
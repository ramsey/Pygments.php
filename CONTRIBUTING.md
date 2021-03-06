# Contributing

Contributions are welcome. We accept pull requests on [GitHub](https://github.com/ramsey/pygments).

This project adheres to a [Contributor Code of Conduct](https://github.com/ramsey/pygments/blob/master/CODE_OF_CONDUCT.md). By participating in this project and its community, you are expected to uphold this code.

## Team members

* [Ben Ramsey](https://github.com/ramsey) - maintainer of the ramsey/pygments package
* [Kazuyuki Hayashi](https://github.com/kzykhys) - original author of [Pygments.php](https://github.com/kzykhys/Pygments.php)

## Communication Channels

You can find help and discussion in the following places:

* GitHub Issues: <https://github.com/ramsey/pygments/issues>
* Wiki: <https://github.com/ramsey/pygments/wiki>

## Reporting Bugs

Bugs are tracked in our project's [issue tracker](https://github.com/ramsey/pygments/issues).

When submitting a bug report, please include enough information for us to reproduce the bug. A good bug report includes the following sections:

* Expected outcome
* Actual outcome
* Steps to reproduce, including sample code
* Any other information that will help us debug and reproduce the issue, including stack traces, system/environment information, and screenshots

**Please do not include passwords or any personally identifiable information in your bug report and sample code.**

## Fixing Bugs

We welcome pull requests to fix bugs!

If you see a bug report that you'd like to fix, please feel free to do so. Following the directions and guidelines described in the "Adding New Features" section below, you may create bugfix branches and send us pull requests.

## Adding New Features

If you have an idea for a new feature, it's a good idea to check out our [issues](https://github.com/ramsey/pygments/issues) or active [pull requests](https://github.com/ramsey/pygments/pulls) first to see if the feature is already being worked on. If not, feel free to submit an issue first, asking whether the feature is beneficial to the project. This will save you from doing a lot of development work only to have your feature rejected. We don't enjoy rejecting your hard work, but some features just don't fit with the goals of the project.

When you do begin working on your feature, here are some guidelines to consider:

* Your pull request description should clearly detail the changes you have made. We will use this description to update our CHANGELOG. If there is no description or it does not adequately describe your feature, we will ask you to update the description.
* We following the **[PSR-2 coding standard](http://www.php-fig.org/psr/psr-2/)**. Please ensure your code does, too.
* Please **write tests** for any new features you add.
* Please **ensure that tests pass** before submitting your pull request. We have Travis CI automatically running tests for pull requests. However, running the tests locally will help save time.
* **Use topic/feature branches.** Please do not ask us to pull from your master branch.
* **Submit one feature per pull request.** If you have multiple features you wish to submit, please break them up into separate pull requests.
* **Send coherent history**. Make sure each individual commit in your pull request is meaningful. If you had to make multiple intermediate commits while developing, please squash them before submitting.

## Running Tests

All tests must pass before we will accept a pull request. If tests do not pass, it will result in a complete build failure. Please run the following command to ensure tests pass before opening your pull request:

```
composer test
```

Keep in mind that we test against multiple versions of PHP, Python, and Pygments. Check out [PHPBrew](https://github.com/phpbrew/phpbrew) for running multiple versions of PHP and [virtualenv](http://docs.python-guide.org/en/latest/dev/virtualenvs/) for running multiple versions of Python and Pygments. When using these tools, you may switch between environments to run the tests. Our [GitHub Actions](https://github.com/ramsey/pygments/blob/.github/workflows/continuous-integration.yml) configuration has more information about the versions of PHP, Python, and Pygments we test against.

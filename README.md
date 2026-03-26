# Robot Framework Manual

:construction: Under development!

Robot Framework Manual is planned to replace the current
[Robot Framework User Guide](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html)
and also current [API docs](https://robot-framework.readthedocs.org/)
will be migrated into it.

See the generated pages at https://pekkaklarck.github.io/manual/.

## Contribution guidelines

Whether you’ve found a typo, outdated instructions, or missing information, any contribution is highly valuable and welcome!

Common practice for submitting
contribution is via [pull requests](https://github.com/robotframework/robotframework/blob/master/CONTRIBUTING.rst#pull-requests).

#### Requirements

- python3.13 or higher

You can check your currently installed Python version by
running the command:

    python3 --version

The rest of the dependencies are defined in `requirements.txt` file, and
will be explained in the later sections.

### Setting up Development Environment

#### Create Python virtual environment

Create a Python virtual environment in the root of the project, to avoid system-wide installation of dependencies, and to keep the development environment isolated:

    python3 -m venv .venv

#### Activate the virtual environment

    source .venv/bin/activate

#### Install dependencies

    pip3 install --upgrade pip
    pip3 install -r requirements.txt

Now you should have all dependencies installed, including `mkdocs`, which
is required to build the webpages. You can verify the installation
by running:

    mkdocs --version

#### Preview the manual - WHY NOT WORKING? Use properdocs?

Robot Framework manual pages are written in Markdown, and the website is built
using [mkdocs-material](https://squidfunk.github.io/mkdocs-material/).

To live preview the changes, start the webserver (in the previously activated virtual environment):

    mkdocs serve

The manual can then be previewed in your favorite browser, at http://127.0.0.1:8000/manual/, and changes will be reflected as you modify the contents of the Markdown pages.

#### Exiting development environment

To stop the webserver, use key combination:

    Ctrl + C

To exit Python virtual environment, type the command:

    deactivate

#### Where to get help

If you need guidance or help with getting started with contribution (or have a suggesion or would like to discuss about the manual), don't hesitate to reach out the [#manual](https://robotframework.slack.com/archives/C063Y9GEMUP) channel on Slack.

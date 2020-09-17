<a href="https://www.bernardi.cloud/">
    <img src=".readme-files/update-check-logo-72.png" alt="Update Check logo" title="Update Check" align="right" height="72" />
</a>

# Update Check
> Command line tool to receive notifications about available applications update

[![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)](https://www.python.org)
[![License](https://img.shields.io/github/license/bernarpa/update-check.svg)](https://opensource.org/licenses/AGPL-3.0)
[![GitHub issues](https://img.shields.io/github/issues/bernarpa/update-check.svg)](https://github.com/bernarpa/update-check/issues)

## Table of contents

- [Why Update Check](#why-update-check)
- [Supported applications](#supported-applications)
- [Usage](#usage)
- [License](#license)

## Why Update Check

I have some instances of Jira and Confluence that I like to keep up to date, lest being an easy target for crackers and script kiddies which, I'm told, infest the Internet in the wild. Of course I ~~wisely decided to use a pre-existing tool which requires just some tweaking~~ took the occasion to write some Python code to ~~pay my daily tribute to the universal entropy~~ keep myself sharp.

## Supported applications

  - Jira
  - Confluence

## Usage

Firstly, create a `settings.py` configuration file by using `settings.py-sample` as template.

Secondly, you might want to schedule the program to run once per day with cron. For example:

    # Update check
    0 7 * * * /home/rnd/anaconda3/bin/python /home/rnd/github/update-check/update-check

The script will send an email if an available update is detected; the email will contain information about the current software version and about the new one.

## License

Update Check is licensed under the terms of the GNU Affero General Public License version 3.

<!-- How to generate this file
```shell
npx --yes github-action-readme-generator@v1.7.2
```
-->
<div align="center" width="100%">
<!-- start title -->

# <img src="doc/assets/branding.svg" width="60px" align="center" alt="branding<icon:check-circle color:blue>" /> GitHub Action: WordPress Plugin Integration Test

<!-- end title -->
<!-- start badges -->

<a href="https://github.com/holyhope/test-wordpress-plugin-github-action/releases/latest"><img src="https://img.shields.io/github/v/release/holyhope/test-wordpress-plugin-github-action?display_name=tag&sort=semver&logo=github&style=flat-square" alt="Release" /></a><a href="https://github.com/holyhope/test-wordpress-plugin-github-action/releases/latest"><img src="https://img.shields.io/github/release-date/holyhope/test-wordpress-plugin-github-action?display_name=tag&sort=semver&logo=github&style=flat-square" alt="Release" /></a><img src="https://img.shields.io/github/last-commit/holyhope/test-wordpress-plugin-github-action?logo=github&style=flat-square" alt="Commit" /><a href="https://github.com/holyhope/test-wordpress-plugin-github-action/issues"><img src="https://img.shields.io/github/issues/holyhope/test-wordpress-plugin-github-action?logo=github&style=flat-square" alt="Open Issues" /></a><img src="https://img.shields.io/github/downloads/holyhope/test-wordpress-plugin-github-action/total?logo=github&style=flat-square" alt="Downloads" />

<!-- end badges -->
</div>

<!-- start description -->

Test a WordPress plugin using PHPUnit.

<!-- end description -->

<!-- start contents -->

This action tests a WordPress plugin in a environment that is similar to a real WordPress site. It installs WordPress, activates the plugin, and runs the tests.

<!-- end contents -->

## Usage

<!-- start usage -->

```yaml
- uses: holyhope/test-wordpress-plugin-github-action@main
  with:
    # Description: WordPress version
    #
    # Default: latest
    wordpress_version: ""

    # Description: PHP version
    #
    # Default: 8.2
    php_version: ""

    # Description: PHP version
    #
    # Default: imagick
    php_extensions: ""

    # Description: Path to the WordPress plugin
    #
    # Default: .
    plugin_dir: ""

    # Description: Plugin slug
    #
    plugin_slug: ""

    # Description: PHPUnit configuration file
    #
    # Default: phpunit.xml
    phpunit_config: ""
```

<!-- end usage -->

## Inputs

<!-- start inputs -->

| **<b>Input</b>**                      | **<b>Description</b>**       | **<b>Default</b>**       | **<b>Required</b>** |
| ------------------------------------- | ---------------------------- | ------------------------ | ------------------- |
| <b><code>wordpress_version</code></b> | WordPress version            | <code>latest</code>      | **false**           |
| <b><code>php_version</code></b>       | PHP version                  | <code>8.2</code>         | **false**           |
| <b><code>php_extensions</code></b>    | PHP version                  | <code>imagick</code>     | **false**           |
| <b><code>plugin_dir</code></b>        | Path to the WordPress plugin | <code>.</code>           | **false**           |
| <b><code>plugin_slug</code></b>       | Plugin slug                  |                          | **true**            |
| <b><code>phpunit_config</code></b>    | PHPUnit configuration file   | <code>phpunit.xml</code> | **false**           |

<!-- end inputs -->
<!-- start outputs -->

| **<b>Output</b>**                | **<b>Description</b>**   |
| -------------------------------- | ------------------------ |
| <b><code>junit_report</code></b> | Path to the JUnit report |

<!-- end outputs -->

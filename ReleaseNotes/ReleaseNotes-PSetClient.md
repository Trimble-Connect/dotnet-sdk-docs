# Trimble Connect PSet Service Client .NET Release Notes

## [2.0.17-beta] - 2020-08-07
* Using portable debug symbols.
* Updated the `Trimble.Connect.Client.Common` dependency to the latest version (1.0.48-beta).

## [2.0.16-beta] - 2020-08-07
* Updated the release notes link.
* Updated the `Trimble.Connect.Client.Common` dependency to the latest version (1.0.47-beta).

## [2.0.15-beta] - 2020-07-29
* Generating NuGet symbols package in the new (snupkg) format.

## [2.0.14-beta] - 2020-07-29
* No longer supporting uap10.0 target (uap platform specific target deprecated as .netstandard 2.0 target should work for uap platforms from 10.0.16299 onwards).

## [2.0.13-beta] - 2020-07-27
* Created beta version NuGet package.

## [2.0.12] - 2020-07-27
* No longer supporting .NET Standard 1.4.

## [2.0.11] - 2020-07-06
* Updated dependencies: `Trimble.Connect.Client.Common` (1.0.43), `Trimble.Identity.OAuth.Password` (1.0.7).
* Excluded leftover files from SonarQube scans from the WhiteSource scans.

## [2.0.10] - 2020-07-02
* Fixed comparison to default value for arguments of type RequestType (fixing Sonar bugs).

## [2.0.9] - 2020-07-01
* Added configuration file for WhiteSource scan.
* Prevented StyleCop from propagating to consuming modules.
* Using the leatest version (1.0.41) of the **_`Trimble.Connect.Client.Common`_** module.

## [2.0.8] - 2020-07-01
* Added support for change sets.
* Added tests for generic requests and extended requests (forward compatibility mechanism).

## [2.0.7] - 2020-06-30
* Removed previously supported obsolete batch get request.
* Added model classes, request methods and tests related to the recommended generic batch get functionality.

## [2.0.6] - 2020-06-23
* Added model classes, request methods and tests related to PSet instances.
* Added tests for libraries, PSet definitions and PSet instances related to subscribing to notifications.

## [2.0.5] - 2020-06-09
* Added more tests related to PSet definitions.

## [2.0.4] - 2020-06-09
* Added model classes, request methods and tests related to PSet definitions.

## [2.0.3] - 2020-06-04
* Using the latest version (1.0.40) of the **_`Trimble.Connect.Client.Common`_** module.
* Support for .NET Core 2.0.
* Updated NuGet package references.
* Incorporated the latest infrastructure changes to align with the Organizer SDK.
* Re-organized source files in both the main project and the test project to follow the standardized folder structure used in other .NET SDK projects.
* Added **_`PSetModel`_** base class for model classes.
* Added **_`PSetReuqest`_** base class for request classes.
* Added model classes, request methods and tests related to libraries.
* Added model classes, request methods and tests related to library policies.
* Added model classes, request methods and tests related to miscellaneous functionality (me endpoint, subscribe to notifications).

## [2.0.2] - 2020-04-29
* Removed the Test namespace.
* Using PROD TID credentials for the tests.
* Using the latest version (1.0.16) of the **_`Trimble.Conect.Client.Common`_** module.
* Changed default assembly file version from x.y.0.0 to x.y.9999.9999 to make debug builds distinguishable from official builds.
* Changed the user agent literal for this module from `pset-client` to `tc-client-pset`.

## [2.0.1] - 2020-04-08
* Adapted the code to use the leatest version (1.0.11) of the **_`Trimble.Connect.Client.Common`_** module.
* Grouped the parameters of the methods that implement requests.
* Re-organized source files into subfolders.
* Fixed StyleCop warnings and enabled automatic StyleCop scans during build.
* Updated release notes.

## [2.0.0] - 2020-03-30
* Breaking changes to the public interface compared to previous versions (v1.0.*):
* Simplified the PSet .NET API: removed controller classes and made the major functionality accessible directly through the **_`PSetClient`_** class.
* The PSet client class has received a shorter name: **_`PSetClient`_**.
* Switched to standardized names for methods that launch requests against the PSet REST API:
* General naming convention for method prefixes is: **_`Get`_**, **_`BatchGet`_**, **_`List`_**, **_`Create`_**, **_`Update`_**, **_`Delete`_**
* For resources that don't have separate create and update methods (like policies, linksets, psets) the prefix for the create/update method is **_`Put`_**
* For asynchronous methods the **_`Async`_** suffix is used.
* In general all the data model class names and all the client method names that launch requests to the PSet service have been aligned with the [PSet service documentation](https://app.swaggerhub.com/apis/Trimble-Connect/pset-prod/v1).

## [1.0.2] - 2020-03-25
* Using Trimble Connect .NET Client Common module (code common to CDM services has moved into this module)
* Cleaned up references
* Fixed StyleCop warnings

## [1.0.1]
* Fix: comments.

## [1.0.0]
* Initial version of PSet Definition service.
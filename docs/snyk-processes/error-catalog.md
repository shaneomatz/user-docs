# Error Catalog

## Snyk Error Codes

The error codes in the table below describe the codes that you may encounter while working with the [Snyk API](../snyk-api-info/) or [CLI](../snyk-cli/). When errors are encountered using the API, they will also have an appropriate [HTTP status code](https://en.wikipedia.org/wiki/List\_of\_HTTP\_status\_codes). If you encounter errors without an error code, use the HTTP status code to determine the appropriate action.

***

## [Snyk](https://docs.snyk.io/introducing-snyk)

#### [SNYK-0001](error-catalog.md#snyk-0001-too-many-requests) - Too many requests

The service has received too many requests and will be throttled.

**HTTP Status:** [429](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/429)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-0002](error-catalog.md#snyk-0002-not-implemented) - Not implemented

The server either does not recognize the request method, or it lacks the ability to fulfil the request.

**HTTP Status:** [501](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/501)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-0003](error-catalog.md#snyk-0003-bad-request) - Bad request

The server cannot or will not process the request due to an apparent client error (e.g. malformed request syntax, size too large, invalid request message framing, or deceptive request routing).

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-004](error-catalog.md#snyk-004-timeout-error) - Timeout error

The server did not receive a timely response from the upstream server.

**HTTP Status:** [504](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/504)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-005](error-catalog.md#snyk-005-unauthorised-error) - Unauthorised error

Authentication failed or has not been provided.

**HTTP Status:** [401](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/401)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-9999](error-catalog.md#snyk-9999-server-error) - Server error

An unexpected server error was encountered.

**HTTP Status:** [500](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500)

**Exit Code:** N/A

**Help Links:**

***

## [Open Source Languages & Package Managers](https://docs.snyk.io/products/snyk-open-source/language-and-package-manager-support)

#### [SNYK-OS-0001](error-catalog.md#snyk-os-0001-unsupported-ecosystem) - Unsupported Ecosystem

The language or package manager is not supported.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

* [https://docs.snyk.io/products/snyk-open-source/language-and-package-manager-support](https://docs.snyk.io/products/snyk-open-source/language-and-package-manager-support)

#### [SNYK-OS-0002](error-catalog.md#snyk-os-0002-unable-to-parse-manifest-file) - Unable to parse manifest file

The provided manifest file could not be parsed.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OS-0003](error-catalog.md#snyk-os-0003-lock-file-out-of-sync-with-manifest-file) - Lock file out of sync with manifest file

Some of the dependencies that are expected to be in the lock file are missing - this usually indicates that the lock file is out of sync with the provided manifest file. Please re-sync the lock file and try again.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

***

## Builds

#### [SNYK-OS-8001](error-catalog.md#snyk-os-8001-invalid-request) - Invalid request

The provided request payload is not valid for the selected ecosystem. Please review the API documentation.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

* [https://apidocs.snyk.io/](https://apidocs.snyk.io/)

#### [SNYK-OS-8002](error-catalog.md#snyk-os-8002-build-environment-not-found) - Build environment not found

The build environment for the provided context could not be found. Please ensure you have created the build environment first.

**HTTP Status:** [404](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/404)

**Exit Code:** N/A

**Help Links:**

***

## [PURL Vulnerabilities](https://docs.snyk.io/introducing-snyk/getting-started-snyk-intel-vuln-db-access#about-the-snyk-vulnerability-database)

#### [SNYK-OSSI-1040](error-catalog.md#snyk-ossi-1040-your-organisation-is-not-authorised-to-perform-this-action) - Your organisation is not authorised to perform this action

You likely don’t have access to the Beta. To get access, you can request access to the Beta through your account manager or team.

**HTTP Status:** [403](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/403)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-1050](error-catalog.md#snyk-ossi-1050-authorization-request-failure) - Authorization request failure

Unexpected error when authenticating. Please try again, and if you continue to experience issues please contact support.

**HTTP Status:** [500](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2010](error-catalog.md#snyk-ossi-2010-invalid-purl-has-been-provided) - Invalid PURL has been provided

Please make sure that the purl you’ve provided is valid. Please see the Package URL specification link for further information.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

* [https://github.com/package-url/purl-spec/blob/master/PURL-SPECIFICATION.rst](https://github.com/package-url/purl-spec/blob/master/PURL-SPECIFICATION.rst)

#### [SNYK-OSSI-2011](error-catalog.md#snyk-ossi-2011-ensure-you-specify-a-namespace-in-the-purl-and-then-try-again) - Ensure you specify a namespace in the purl and then try again

You have requested a package type which requires a namespace (eg. maven group id). Please supply the namespace in order to retrieve the package correctly.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

* [https://github.com/package-url/purl-spec/blob/master/PURL-SPECIFICATION.rst](https://github.com/package-url/purl-spec/blob/master/PURL-SPECIFICATION.rst)

#### [SNYK-OSSI-2020](error-catalog.md#snyk-ossi-2020-ecosystem-is-not-supported) - Ecosystem is not supported

Ensure that the package type is a supported type.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2021](error-catalog.md#snyk-ossi-2021-purl-components-required) - Purl components required

Currently we require a list of components of the package url specification. The purl supplied by the user did not specify all the components which we currently require.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2022](error-catalog.md#snyk-ossi-2022-you-have-submitted-a-purl-with-components-which-are-not-supported) - You have submitted a purl with components which are not supported

Please remove the component which is not supported, and try to make the request again. The endpoint only accepts particular components.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2030](error-catalog.md#snyk-ossi-2030-requested-package-not-found) - Requested package not found

The package you’ve specified in the purl can not be found in our vulnerability database. Please check that the package name, ecosystem and version are correct and then try again.

**HTTP Status:** [404](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/404)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2031](error-catalog.md#snyk-ossi-2031-vulnerability-service-is-currently-not-available) - Vulnerability service is currently not available

This issue is unexpected, and the service should recover quickly. If not, please contact support.

**HTTP Status:** [503](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/503)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2032](error-catalog.md#snyk-ossi-2032-this-issue-is-unexpected-and-the-service-should-recover-quickly-if-not-please-contact-support) - This issue is unexpected and the service should recover quickly if not please contact support

An unexpected error occurred. Please try again, and if you continue to experience issues please contact support.

**HTTP Status:** [500](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2033](error-catalog.md#snyk-ossi-2033-this-issue-is-unexpected-and-the-service-should-recover-quickly-if-not-please-contact-support) - This issue is unexpected and the service should recover quickly if not please contact support

An unexpected error occurred with the vulnerability service. Please try again, and if you continue to experience issues please contact support.

**HTTP Status:** [500](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2040](error-catalog.md#snyk-ossi-2040-an-error-was-experienced-by-the-service-when-processing-the-request) - An error was experienced by the service when processing the request

This issue is unexpected, and the service should recover quickly. If not, please contact support.

**HTTP Status:** [500](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500)

**Exit Code:** N/A

**Help Links:**

#### [SNYK-OSSI-2041](error-catalog.md#snyk-ossi-2041-invalid-pagination-parameters) - Invalid pagination parameters

Please ensure the supplied pagination limit is > 1 and <= 1000, and that the offset is >= 0.

**HTTP Status:** [400](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400)

**Exit Code:** N/A

**Help Links:**

***

Genererated at 2022-09-29T13:20:03.354Z
# Change Log - @autorest/common

This log was last generated on Tue, 16 Nov 2021 17:26:36 GMT and should not be manually modified.

## 1.4.0
Tue, 16 Nov 2021 17:26:36 GMT

### Minor changes

- **Removed** identitySourceMapping
- **Added** progress bar reporting to the logger

### Patches

- **Fix** Issue with coloring [] wrapped elements

## 1.3.0
Wed, 08 Sep 2021 15:39:22 GMT

### Minor changes

- **Added** New logger pipeline
- Added coloring for markdown ``` code blocks
- Add `color` utility to style markdown to cli format
- **Update** to new path mapping sourcemap functionality

## 1.2.0
Mon, 19 Jul 2021 15:15:41 GMT

### Minor changes

- **Moved** literate-yaml logic to @autorest/configuration
- Drop support for node 10

### Patches

- **Added** utils `isDefined`

## 1.1.4
Mon, 10 May 2021 18:01:37 GMT

### Patches

- **Fix** Keep order of property when merging to allow interpolation from same file

## 1.1.3
Fri, 09 Apr 2021 19:53:22 GMT

_Version update only_

## 1.1.2
Thu, 01 Apr 2021 15:46:41 GMT

### Patches

- **Added** configuration for usage of @azure/logger in libraries

## 1.1.1
Tue, 16 Mar 2021 15:52:56 GMT

### Patches

- Add `trackWarning` functionality to logger
- **Fix** Max call stack issue with loading very large swagger
- Bump dependencies versions

## 1.1.0
Fri, 05 Mar 2021 16:31:29 GMT

### Minor changes

- **Update** merge functionality to be able to take interpolation context. Default to the higher priority element otherwise
- **Update** Merging functionality to accept an array merging strategy to decide order of merging

## 1.0.3
Fri, 26 Feb 2021 21:50:13 GMT

### Patches

- **Update** Autorest logger definition

## 1.0.2
Sat, 20 Feb 2021 17:49:35 GMT

### Patches

- **Fix** Revert use of flatMap which is not available on node 10

## 1.0.1
Fri, 19 Feb 2021 21:42:09 GMT

### Patches

- Initial release, include code extract from @autorest/core around merging object and reading yaml/config


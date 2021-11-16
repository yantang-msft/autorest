# Change Log - @autorest/core

This log was last generated on Tue, 16 Nov 2021 17:26:36 GMT and should not be manually modified.

## 3.7.0
Tue, 16 Nov 2021 17:26:36 GMT

### Minor changes

- **Updated** `--help` to use configuration schema and be consistent
- **Added** Support for sourcemap in autorest extensions
- Add installation status of extension with a progress bar.
- Improve error reporting when extension fails to install.

### Patches

- **Fix** --help crash
- **Internal** Remove use of extension method `.last`
- **Fix** Nullable on certain properties during tree shaking

## 3.6.6
Mon, 11 Oct 2021 21:01:13 GMT

### Patches

- **Fix** Unreferenced discriminated union option being removed

## 3.6.5
Wed, 06 Oct 2021 17:36:17 GMT

### Patches

- **Fix** exit code always 0

## 3.6.4
Tue, 05 Oct 2021 16:39:50 GMT

### Patches

- **Fix** `message-format` not being respected

## 3.6.3
Thu, 23 Sep 2021 19:51:32 GMT

### Patches

- **Added** `include-x-ms-examples-original-file` flag to activate `x-ms-original-file` injection in `x-ms-examples`

## 3.6.2
Fri, 17 Sep 2021 17:52:01 GMT

### Patches

- **Fix** Deduplicating enums dropped `format` property

## 3.6.1
Thu, 16 Sep 2021 18:49:17 GMT

### Patches

- **Fix** Deduplicating `boolean` enums changed type to `string`

## 3.6.0
Wed, 08 Sep 2021 15:39:22 GMT

### Minor changes

- **Uptake** New logger
- Uptake new changes to Swagger->OpenApi3 converter
- `x-ms-examples` loaded via $ref will save orignal location with `x-ms-original-file` extension property
- Keep `x-` extension properties when merging enums
- **Perf** Small perf improvement for components cleaner plugin
-  **Update** to new path mapping sourcemap functionality
- **Remove** quick-check plugin

### Patches

- **Perf** Minor perf in merger plugin
- **Perf** Minor performance improvement in allof cleaner plugin
- Log error when directive where clause is invalid
- Improve erorr message for directive when there is an error in the transform code
- **Fix** Error in config loading would not be logged as the logging session would not be awaited on

## 3.5.0
Mon, 19 Jul 2021 15:15:41 GMT

### Minor changes

- **Added** `debug` flag to directive to enable additional logging
- **Added** support for changing end of line of generated files with new `eol` config.
- **Feature** Resolve relative servers url using spec host
- Allow suppressing warnings without source
- Drop support for node 10
- **Perf** Memory usage improvements
- **Perf** Unload sourcemap from memory if not used

### Patches

- **Added** Flag to skip sourcemap generation
- **Fix** sourcemap for multiple plugins
- **Fix** Issue in directive manipulator preventing multiple directive to run on OpenApi3 documents

## 3.4.5
Thu, 03 Jun 2021 22:37:55 GMT

### Patches

- Blaming files not loaded by autorest

## 3.4.4
Wed, 26 May 2021 18:31:17 GMT

### Patches

- **Bump** @autorest/configuration with fix with yarn/cli.js not found

## 3.4.3
Thu, 20 May 2021 16:41:13 GMT

### Patches

- **Added** $ref sibling validation
- **Fix** Keep `x-` extension next to $ref when tree shaking properties
- **Bump** @autorest/configuration version
- **Added** warning when using `x-ms-code-generation-settings` which is not supported in autorest v3

## 3.4.2
Mon, 10 May 2021 18:01:37 GMT

### Patches

- Update dependencies to include fix for interpolating config value from previous value in same file

## 3.4.1
Tue, 04 May 2021 18:18:45 GMT

### Patches

- **Fix** Uncaught promise exception

## 3.4.0
Tue, 27 Apr 2021 17:48:43 GMT

### Minor changes

- **Updated** CLI Parsing to uptake logic moved to @autorest/configuration and use config validation

### Patches

- **Fix** Default license header containing uninterpolated {generator}
- **Fix** Tree Shaking number enums same as string enum. This allows those enum to get a better auto generated name if no name is provided
- **Perf** improvement to multi api merger

## 3.3.2
Fri, 16 Apr 2021 15:18:54 GMT

### Patches

- **Merge x-ms-paths into paths during multi-api-merger step"

## 3.3.1
Tue, 13 Apr 2021 15:34:55 GMT

### Patches

- **Package update** update schema package for fix with $ref

## 3.3.0
Fri, 09 Apr 2021 19:53:22 GMT

### Minor changes

- **Added** Semantic validator plugin 
- **Feature** Add sourcemap support for errors providing original location of problem
- **Added** support for emitting statistics of the specs and resuting model

### Patches

- **Added** [SemanticValidator] Path parameters validation to the semantic validator
- **Internal** Refactor plugins

## 3.2.4
Fri, 02 Apr 2021 15:18:00 GMT

### Patches

- **Update** @autorest/configuration to take fix for broken interactive plugin

## 3.2.2
Thu, 01 Apr 2021 15:46:41 GMT

### Patches

- Bump @azure-tools/uri version to ~3.1.1
- **Cleanup** Migrated use of require -> es6 imports
- **Added** configure @azure/logger according to debug/verbose flags
- **Added** New normalize-identity plugin to support multi openapi3 files output
- **Added** New config/flag `--output-converted-oai3` to output openapi3 files right after conversion from Swager 2.0
- Update to simplified configuration loader interface

## 3.2.1
Tue, 16 Mar 2021 19:28:18 GMT

### Patches

- **Update** @azure-tools/data-store

## 3.2.0
Tue, 16 Mar 2021 15:52:56 GMT

### Minor changes

- Update swagger schema validator to use new system(`ajv` & `ajv-errors`) providing more relevant information

### Patches

- **Fix** enum deduplicator to prevent crash when using allOf in enums
- **Handle** Discrimnator mapping. Make sure the refs are updated
- **Fix** Cannot read property 'pass-thru' of undefined crash
- Bump dependencies versions

## 3.1.3
Wed, 10 Mar 2021 02:02:59 GMT

### Patches

- **Update** @autorest/configuration to uptake directives array fix

## 3.1.2
Mon, 08 Mar 2021 18:07:37 GMT

### Patches

- Set @autorest/typescript default version to 'latest'
- **Update** @autorest/configuration dependency to update `--require` cli load order fix

## 3.1.1
Fri, 05 Mar 2021 16:31:29 GMT

### Patches

- **Rename** trenton plugin to terraform
- **Fix** Handle using extension properties(x-) under components in OpenAPI3
- **Update** @autorest/configuration dependency to uptake various configuration loading fixes

## 3.1.0
Fri, 26 Feb 2021 21:50:13 GMT

### Minor changes

- **Remove** legacy CLI functionality(Using arguments with single dash).

### Patches

- **Update** Moved configuration loading from @autorest/core and redesign
- **Fix** issue when using properties with `$ref` as name where it would try to resolve a reference.

## 3.0.6375
Sat, 20 Feb 2021 17:49:35 GMT

### Patches

- **Fix** Revert use of flatMap which is not available on node 10

## 3.0.6374
Fri, 19 Feb 2021 21:42:09 GMT

### Patches

- Bundle jsonpath in webpack
- Extract some section into @autorest/core
- Rethink config
- **Fix** problem not resolving the yarn/cli.js file
- **Fix** Components cleaner not removing external non used headers but remove their schemas
- **Revert** removal of header-text config getter

## 3.0.6373
Thu, 11 Feb 2021 18:03:07 GMT

### Patches

- **Fix** Configuration for csharp causing pipeline stage not found error
- **Improvement** Provide a more detail error message when pipeline can't find a stage.
- **Update** @azure-tools/extension to ~3.1.272 and bundle it in the webpack file

## 3.0.6372
Tue, 09 Feb 2021 22:00:21 GMT

### Patches

- **Fix** Issue where it was not possible to override a config flag defined in the same markdown config. Markdown configuration loading now treats yaml code block in increasing priority order.
- **Update** @azure-tools/extension to newer version that will log errors when installing packages.

## 3.0.6371
Mon, 08 Feb 2021 23:06:15 GMT

### Patches

- Internal: Migrate bundling system to webpack
- Update csharp generator to default to v3. Use `--v2` to revert to previous version

## 3.0.6370
Thu, 04 Feb 2021 19:05:18 GMT

### Patches

- Internal: Moved source to src/ folder
- Refactoring: Cleanup of code running transform directives
- Internal code linting fixes
- Internal: Add some tests to the tree shaker

## 3.0.x
Tue, 4 Feb 2020 00:00:00 GMT

### Patches

- rebuild to pick up latest data-store to fix the caching filename size
- OAI2-to-OAI3 converter update in perks.
- TransformerViaPointer was turning null into {} 
- rebuild to fix NPM publishing problem.
- remove additionalProperties: false so v2 generators don't choke.
- rebuild to pick up perks change to fix multibyte utf8 over byte boundary problem
- rebuild to pick up a perks change to support turning underscore in semver to dash on gh releases
- rebuild to pick up newer extension library that supports python interpreter detection
- force rebuild to pick up fix in oai2 converter
- update the oai2-to-oai3 converter (parameterized host parameters should be client parameters if they are $ref'd)


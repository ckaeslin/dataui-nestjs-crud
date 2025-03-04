## [5.2.4] - 2023-06-01

- d6d3c4eb - Merge pull requestfrom xTCry/class-transform-options
  Support
- 96043ecb - Implement `$not` operator in `search`

## [5.1.13] - 2023-06-01

- d6d3c4eb - Merge pull requestfrom xTCry/class-transform-options
  Support
- 96043ecb - Implement `$not` operator in `search`

## [5.2.3] - 2023-03-16

### Features

- Support passing options to class-transformer
- Support auth and extra parameters in CrudRequest, thanks to [gantispam](https://github.com/gantispam)

## [5.2.2] - 2022-12-05

### Features

- Switch to typeorm 0.3.6

## [5.1.2] - 2022-05-24

### Fix deps

- 0028dba0 - Merge pull request #9 from H4ad/fix/deps
  fix(deps): upgrade all dependencies, thanks to [Vinicius Lourenço](https://github.com/H4ad)

## [5.1.2] - 2022-05-24

### Fix deps

- 0028dba0 - Merge pull request #9 from H4ad/fix/deps
  fix(deps): upgrade all dependencies, thanks to [Vinicius Lourenço](https://github.com/H4ad)

## [5.1.1] - 2022-01-11

### Fix

- 56d49d3 - Merge remote-tracking branch 'dschoeni/fix/117-eager-breaks-update', thanks to [Dschoeni](https://github.com/dschoeni)

## [5.1.0] - 2021-12-08

### Features

- 0692be2 - feat: add custom operators, thanks to [Darkein](https://github.com/Darkein)

## [5.0.17] - 2021-11-28

### Bug Fixes

- 041f761 - fix(crud-typeorm): bug ability to use search and filter features with nested entities

## [5.0.16] - 2021-11-28

### Bug Fixes

- bd28914 - fix(typeorm-crud): fix(typeorm): correct quotes for column identifiers when driver is mariadb
- 91e2bae - fix(typeorm-crud): fix sql injection check looping on the first regex
- b5f05c7 - fix(typeorm-crud): add warning when using disallowed relation
- e17847f - fix(crud-update): make updateOneBase dto type partial
- 0d1eed2 - fix(auth): fix filter for user in meController
- 0f3fd22 - fix(swagger): fix constant when getting swagger extra models
- 3e1e5ca - fix(crud): typo fix getMayRouteOptions -> getManyRouteOptions
- 453d438 - (origin/master) feat(readme): update readme
- 6cc1c28 - feat(readme): update release readme

## [5.0.15] - 2021-11-28

### Bug Fixes

- **crud** - Fix select boolean type in join option [#4](https://github.com/dataui/crud/pull/4))

## [5.0.14] - 2021-11-27

### Bug Fixes

- **typeorm** - fixed cache - do not use cache when updating resources [#3](https://github.com/dataui/crud/pull/3))

## [5.0.13] - 2021-11-27

Update readme to include release steps

## [5.0.12] - 2021-11-27

Migrate repo from nestjsx to rewiko

## [4.6.2] - 2020-05-14

### Bug Fixes

- **typeorm** - fixed selected fields on joins [#510](https://github.com/nestjsx/crud/issues/510)). Kudos to @jbrousseau for finding this bug

## [4.6.1] - 2020-05-08

### Bug Fixes

- **typeorm** - fixed query generation when a column display name differs from its name in db [#401](https://github.com/nestjsx/crud/issues/401)). Kudos to @farhad2161 for finding this bug

## [4.6.0] - 2020-05-07

### Features

- **crud**/**typeorm** - added `select` (boolean) to `join` options which allows to join relation but not select it ([#218](https://github.com/nestjsx/crud/issues/218))

### Bug Fixes

- **typeorm** - fixed column identifier for MySQL ([#401](https://github.com/nestjsx/crud/issues/401))
- **typeorm** - fixed nested relations aliases, filtering, sorting ([#419](https://github.com/nestjsx/crud/issues/419), [#450](https://github.com/nestjsx/crud/issues/450), [#267](https://github.com/nestjsx/crud/issues/267), [#385](https://github.com/nestjsx/crud/issues/385))

## [4.5.0] - 2020-05-01

### Improvements

- **crud** - added enum support for params Swagger. Kudos to @tbrannam

### Bug Fixes

- **crud** - fixed auth property definition. Kudos to @lafeuil
- **typeorm** - fixed request generation with aliases ([#321](https://github.com/nestjsx/crud/issues/321), [#401](https://github.com/nestjsx/crud/issues/401)). Kudos to @joennlae

## [4.4.5] - 2020-04-18

## Deps

- **crud** fixted imports

## [4.4.4] - 2020-04-18

### Deps

- **dev** fixted lerna

## [4.4.3] - 2020-04-18

### Bug Fixes

- **crud** fixed returning `pageCount` in some cases ([#465](https://github.com/nestjsx/crud/pull/465))
- **typeorm** fixed critical bug with possible SQL injections when using query `?sort=` (big kudos to João Maurício)
- **typeorm** fixed filter conditions for LIKE/iLIKE operators ([#395](https://github.com/nestjsx/crud/pull/395))

## [4.4.2] - 2020-03-17

### Bug Fixes

- **crud** fixed custom routes params caused by NestJs v7 breaking changes ([#443](https://github.com/nestjsx/crud/issues/443))

## [4.4.1] - 2019-12-28

### Bug Fixes

- **crud** fixed `CrudRequestInterceptor` validation status code from 500 to 400 ([#374](https://github.com/nestjsx/crud/issues/374), [#247](https://github.com/nestjsx/crud/issues/247))

## [4.4.0] - 2019-12-27

### Features

- **crud** added `serialize` to the global options

## [4.3.0] - 2019-12-21

### Features

- **crud** added `dto` to the `CrudOptions` ([#132](https://github.com/nestjsx/crud/issues/132))
- **crud** added `serialize` to the `CrudOptions`
- **crud** added `search` query param and a new search condition api
- **crud** added new condition operators: `$eqL`, `$neL`, `$startsL`, `$endsL`, `$contL`, `$exclL`, `$inL`, `$notinL` for case insensitive queries ([#77](https://github.com/nestjsx/crud/issues/77))
- **crud** added `@crudAuth()` class decorator for authorized requests

### Improvements

- **crud** `CrudRequestInterceptor` can be used for both crud and non-crud controllers or for custom routes within crud controller
- **crud** support `@nestjs/swagger` major versions: v3 and v4 ([#340](https://github.com/nestjsx/crud/issues/340))
- **crud** added `returnShallow` option to the `CrudOptions.routes` `createOneBase`, `updateOneBase`, `replaceOneBase` methods ([#158](https://github.com/nestjsx/crud/issues/158))
- **crud** added `alias` to the `CrudOptions.join` ([#350](https://github.com/nestjsx/crud/issues/55))
- **crud** added `alwaysPaginate` to the `CrudOptions.query`, can be used globally as well ([#213](https://github.com/nestjsx/crud/issues/213))
- **crud** `CrudOptions.query.filter` can be a function that returns transformed `search` object
- **crud** added `disabled` for an objects withing `CrudOptions.params`
- **request** query builder: now uses [qs](https://www.npmjs.com/package/qs) package
- **request** query builder: `filter` and `or` methods can accept array of filter objects
- **typeorm** changed visibility of all methods ([#226](https://github.com/nestjsx/crud/issues/226))
- **typeorm** use `ILIKE` for PostgreSQL ([#212](https://github.com/nestjsx/crud/issues/212))

### Bug Fixes

- **crud** swagger: fixed response models ([#350](https://github.com/nestjsx/crud/issues/350))
- **crud** swagger: fixed query params ([#196](https://github.com/nestjsx/crud/issues/196))
- **crud** swagger: fixed renamed params ([#283](https://github.com/nestjsx/crud/issues/283))
- **crud** swagger: fixed swagger method decoration on overridden methods
- **crud** query parser: fixed parsing integers when it's a big int
- **typeorm** fixed load embedded entities ([#138](https://github.com/nestjsx/crud/issues/138))
- **typeorm** fixed left join issues ([#31](https://github.com/nestjsx/crud/issues/31), [#98](https://github.com/nestjsx/crud/issues/98))
- **typeorm** fixed composite key joins ([#238](https://github.com/nestjsx/crud/issues/238))
- **typeorm** fixed entity events ([#51](https://github.com/nestjsx/crud/issues/51))
- **typeorm** all methods return entity instances ([#259](https://github.com/nestjsx/crud/issues/259))

## [4.2.0] - 2019-07-26

### Features

- **crud** added support for older versions of `UUID` ([#186])

### Bug Fixes

- **crud** fixed `BulkDto` swagger description ([#159])
- **crud** fixed `CrudRequestInterceptor` request parsing
- **requests** added `@nestjsx/util` as a dependency ([#184])
- **requests** fixed condition operators mapping ([#148])
- **requests** fixed ISO date string validation ([#161])
- **typeorm** fixed filtering and sorting by nested fields ([#105])
- **typeorm** fixed `too many nested levels` exception ([#87])
- **typeorm** fixed pagination `pageCount` ([#179])

### Deps

- **dev** updated deps

## [4.1.0] - 2019-06-27

### Features

- **crud** added `PUT` request handling ([#107])
- **requests** added creating request builder with params ([#131])
- **requests** improved query params naming parsing ([#101])

### Bug Fixes

- **crud** set decorators after Swagger so metadata can be overwritten
- **requests** added support for ISO-8610 date strings

## [4.0.1] - 2019-06-21

### Bug Fixes

- **requests** fixed query parser to properly accept numbers and booleans ([#97])

## [4.0.0] - 2019-06-12

### BREAKING CHANGES

- **crud:** changed `CrudOptions` ([docs](https://github.com/nestjsx/crud/wiki/Controllers#options))
- **crud:** remove decorators: `@ParsedOptions`, `@ParsedParams`, `@ParsedQuery`. Add decorator `@ParsedRequest` instead.
- **crud:** change interfaces
- **services:** remove `RestfulOptions` from services
- **services:** changed base abstract class

### Features

- **repo:** refactor to monorepository
- **docs:** new [documentation](https://github.com/nestjsx/crud/wiki)
- **packages:** totally refactor `@nestjsx/crud` to be service (ORM) agnostic
- **packages:** add `@nestjsx/crud-typeorm` ([docs](https://github.com/nestjsx/crud/wiki/ServiceTypeorm))
- **packages:** add `@nestjsx/crud-request` ([docs](https://github.com/nestjsx/crud/wiki/Requests#description), [#53])
- **crud:** add global options ([docs](https://github.com/nestjsx/crud/wiki/Controllers#global-options), [#64])
- **crud:** add eager relations option ([#54], [#67])

### Bug Fixes

- several fixes

[4.6.2]: https://github.com/nestjsx/crud/compare/v4.6.1...v4.6.2
[4.6.1]: https://github.com/nestjsx/crud/compare/v4.6.0...v4.6.1
[4.6.0]: https://github.com/nestjsx/crud/compare/v4.5.0...v4.6.0
[4.5.0]: https://github.com/nestjsx/crud/compare/v4.4.5...v4.5.0
[4.4.5]: https://github.com/nestjsx/crud/compare/v4.4.4...v4.4.5
[4.4.4]: https://github.com/nestjsx/crud/compare/v4.4.3...v4.4.4
[4.4.3]: https://github.com/nestjsx/crud/compare/v4.4.2...v4.4.3
[4.4.2]: https://github.com/nestjsx/crud/compare/v4.4.1...v4.4.2
[4.4.1]: https://github.com/nestjsx/crud/compare/v4.4.0...v4.4.1
[4.4.0]: https://github.com/nestjsx/crud/compare/v4.3.0...v4.4.0
[4.3.0]: https://github.com/nestjsx/crud/compare/v4.2.0...v4.3.0
[4.2.0]: https://github.com/nestjsx/crud/compare/v4.1.0...v4.2.0
[4.1.0]: https://github.com/nestjsx/crud/compare/v4.0.1...v4.1.0
[4.0.1]: https://github.com/nestjsx/crud/compare/v4.0.0...v4.0.1
[4.0.0]: https://github.com/nestjsx/crud/compare/v.3.2.0...v4.0.0
[#97]: https://github.com/nestjsx/crud/issues/97
[#53]: https://github.com/nestjsx/crud/issues/53
[#64]: https://github.com/nestjsx/crud/issues/64
[#54]: https://github.com/nestjsx/crud/issues/54
[#67]: https://github.com/nestjsx/crud/issues/67
[#107]: https://github.com/nestjsx/crud/issues/107
[#131]: https://github.com/nestjsx/crud/issues/131
[#101]: https://github.com/nestjsx/crud/issues/101
[#186]: https://github.com/nestjsx/crud/pull/186
[#184]: https://github.com/nestjsx/crud/issues/184
[#148]: https://github.com/nestjsx/crud/issues/148
[#105]: https://github.com/nestjsx/crud/issues/105
[#87]: https://github.com/nestjsx/crud/issues/87
[#159]: https://github.com/nestjsx/crud/issues/159
[#161]: https://github.com/nestjsx/crud/issues/161
[#179]: https://github.com/nestjsx/crud/issues/179

CHANGELOG
=========

This changelog references the relevant changes done in this project.

This project adheres to [Semantic Versioning](http://semver.org/) 
and to the [CHANGELOG recommendations](http://keepachangelog.com/).


## [Unreleased]



## [0.2.3] - 2016-08-23

### Added
- Add booking duration in booking price
- Add DQL MySQL timestamp diff function
- Add ReportBundle support

### Fixed
- Fix flash bags on review manager 
- Fix duration computing without time range 

### Changed
- CS 

### Deprecated



## [0.2.2] - 2016-07-06

### Added
- Add Min/Max listing duration informations on listing show page
- Add time picker in time type fields
- Add timepicker parameter

### Fixed
- Fix error occurring when a date is filled without the other one
- Fix error occurring when a time is filled without the other one
- Fix CS in common.js > getNbUnReadMessages
- Fix Translate manager with missing key or secret param
- Fix ie edge/ipad timepicker compatibility

### Changed
- Reduce number of twig core extension service args
- Factorize and simplify Javascript date and time management
- Fontello icons code
- Remove unused glyphicons halflings
- Remove "updated at" column in admin booking list
- Change default time_unit parameter to 60 min

### Deprecated
- Fix TimeRange form type sf 2.8 depreciation
- Remove TimeHidden form type


## [0.2.1] - 2016-06-28

### Fixed
- Fix sensio/distribution-bundle / composer 1.1.0 type hint compatibility
- Fix google map infobox.js remote access disabled
- Disable manual translations on listing and user edition when there is only one locale available on platform
- Set SMS default locale equal to app default locale
- Add booking status "new" criteria to SMS booking acceptation

### Changed
- Change listing search by categories by including listings without categories
- Update doc/index.rst


## [0.2.0] - 2016-04-08

### Added
- Add DoctrineMigrationBundle
      
### Changed
- Change version of sonata-project/doctrine-orm-admin-bundle to dev-master instead 2.3 to resolve AuditBlockService
- Change version of sonata-project/admin-bundle to 2.4@dev instead 2.3 to resolve AuditBlockService
- Change version of "knplabs/doctrine-behaviors" from dev-master to ^1.3 release
- Change version of "hwi/oauth-bundle" from "0.4.*@dev" to "^0.4"
- Update "egeloen/ckeditor-bundle" from "~3.0" to "^4.0"
- Update "helios-ag/fm-elfinder-bundle" from "~5.0" to "^6.0"
- Update "fzaninotto/faker" from "1.5.*@dev" to "^1.5"
- Update "jms/di-extra-bundle" from "1.4.*@dev" to "^1.7"
- Update "willdurand/geocoder-bundle" from "3.1.*@dev" to "^4.1"
- Change CocoricoGeoBundle to be compatible with "willdurand/geocoder-bundle" 4.1
- Change credit link
- Change doc index.rst
- Change listing_search_min_result value from 5 to 1
- Change page fixture description

### Deprecated

See https://gist.github.com/mickaelandrieu/5211d0047e7a6fbff925 and 
https://github.com/symfony/symfony/blob/2.8/UPGRADE-3.0.md

- Renamed AbstractType::setDefaultOptions to AbstractType::configureOptions
- Renamed AbstractType::getName to AbstractType::getBlockPrefix
- Renamed @translator service to @translator.default
- Replace @request service call by Request object injection in the action method
- Replace form.csrf_provider service call by security.csrf.token_manager service call
- Replace intention option by csrf_token_id option in security.yml 
- Replace intention form option resolver by csrf_token_id in forms
- Replace Twig initRuntime method by adding needs_environment = true in filters arg functions
- Replace setNormalizers by setNormalizer
- Change setAllowedValues to modify one option at a time
- Add `choices_as_values => true `to the ChoiceType and flip keys and values of choices option
- Split security.context service into security.authorization_checker and security.token_storage
- Rename `precision` option to `scale`
- Remove scope from service definitions
- Replace `sameas` by `same as` in Twig templates
- Replace `form` tag by twig `form_start` function 
- ... 

### Fixed
- Add `__toString` to Contact entity 
- Fix admin datagrid filter status for BookingPayinRefund
- Gmap Markers autoescape html
- Add custom DoctrineCurrencyAdapter to fix Lexik currency bundle convert sql request
- Listing discount editions error displaying
- Change listing category parent label in admin
- Add required attributes to page admin form fields
- Fix links translations in error pages
- Fix find bookings payed by asker when MangoPayBundle is not enabled

## [0.1.1] - 2016-04-04

### Added
- Add currency on booking amount error message 
- Add fees help in sonata admin for bank wire
- Add default currency on admin BankWire "Debited funds" field

### Fixed
- Fix duplicate error message on new booking 
- Fix bookings refusing while booking acceptation
- Fix currency format on all bills
- Fix admin currency vertical align on price fields 
- Fix admin listing "rules" field requirement 
      
### Changed
- Update documentation
- Change min listing price parameter to 1 (default currency)
- Change composer.json support section


## [0.1.0] - 2016-03-23

### Added

- First commit


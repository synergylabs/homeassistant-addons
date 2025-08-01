# Changelog

## 1.0.0b17 - 2025-08-01

### Added

- Automatically detect connectivity issues caused by ARP spoofing, and disable ARP spoofing if so

### Changed

- Fix Nest devices not detecting as IoT devices
- Fix crash when loading device details page
- Assorted other bug fixes

## 1.0.0b16 - 2025-07-30

### Added

- Added details about device sensors and privacy settings for select manufacturers

### Changed

- Add additional metrics
- Assorted other bug fixes

## 1.0.0b14 - 2025-07-21

### Changed

- Add additional privacy policies
- Fix network data table not loading on some devices

## 1.0.0b13 - 2025-07-21

### Changed

- Update privacy policies
- Fix network data table not showing

## 1.0.0b12 - 2025-07-18

### Changed

- Assorted UI improvements
- Reduce race conditions and errors
- Handle more types of DNS traffic

## 1.0.0b11 - 2025-07-08

### Changed

- Fix network data table not loading when expected

## 1.0.0b10 - 2025-07-07

### Changed

- Fix bugs resulting in traffic not being counted
- UI improvements

## 1.0.0b9 - 2025-07-02

### Changed

- Improve page load times and add more loading indicators
- Reduce race conditions in database writes

## 1.0.0b8 - 2025-07-01

### Changed

- Add additional error handling in Home Assistant scanner
- Limit log size
- Add additional status messages for log upload

## 1.0.0b7 - 2025-06-30

### Changed

- Check that add-on settings are set correctly and offer in the add-on to fix them
- Improve scanning speed by running network scans in parallel
- Require that user enable network monitoring for at least 3 devices to complete setup

### Known issues

- Banner for Error 101 shows even if all settings are correct

## 1.0.0b6 - 2025-06-27

### Changed

- Ensure all setup steps are completed before user can view full dashboard
- Switched meeting scheduling tool to Calendly

## 1.0.0b5 - 2025-06-26

### Added

- Added dialog with more details about companies in network data

### Changed

- Assorted string updates
- Assorted style updates
- Fixed loss of toggle state when navigating between network monitoring and device detail screens

## 1.0.0b4 - 2025-06-26

### Changed

- Fixed edits to device information not properly saving
- Fixed some company names displaying as None

## 1.0.0b3 - 2025-06-24

### Changed

- Bug fixes

## 1.0.0b2 - 2025-06-24

### Added

- Added study completion flow

### Changed

- Improve network scan speed and add status indicators
- Minor string updates

## 1.0.0b1 - 2025-06-23

- First beta release
- Added onboarding wizard
- Improved display of networking data
- Added ability to edit device names

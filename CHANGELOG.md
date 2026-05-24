# Changelog

All notable internal development changes for the Arlox-OKST56 Tool Suite are tracked here.

---

## v1.3.0

### Added

- Added JSON migration support for:
  - App settings
  - Dynasty registry
  - Dynasty profile files
- Added app version tracking support in JSON files.
- Added hidden subprocess handling for cleaner published app behavior.
- Added timing instrumentation for Dynasty Hub and Schedule Generator workflows.

### Changed

- Improved Dynasty Hub startup and lazy-loading performance.
- Improved Dynasty Central schedule loading behavior.
- Updated Transfer Portal import workflow to import only generated output CSVs.
- Updated published app packaging to include new Core and UI folders.

### Fixed

- Fixed Dynasty Central schedule viewer ghosting/repaint issues.
- Fixed schedule card clipping behavior.
- Fixed Week sorting in table view.
- Fixed ranked-team alphabetical sorting behavior.
- Improved Conference Realignment repaint stability.
- Improved schedule refresh stability after DB writes.

### Full Notes
See: [v1.3.0](./Release-Notes/v1.3.0.md)

---

## v1.2.0

### Added
- Kickoff Classic promotion system.
- Dynamic Kickoff Classic stadium settings.
- NEUT and NESG table rebuilding for neutral-site presentation data.
- RPCS3 extensionless USR-DATA support.
- 2002 Retro Mod preset.
- Dynasty Central Settings page.
- Schedule card layout options.
- Schedule table font size options.
- Sortable and resizable Schedule table columns.
- Onedir PyInstaller build option.

### Improved
- Schedule write performance through SCHD CSV rebuild/import workflow.
- CSV import support for shrinking tables.
- Conference Realignment division management.
- Dynasty Central logo folder handling.
- Schedule table usability and formatting.

### Fixed
- Kickoff Classic games not displaying correctly in the in-game schedule preview.
- Kickoff Classic stadium settings being capped at five entries.
- Dormant divisions appearing in the in-game conference standings UI.
- Empty divisions remaining in the DIVI table.
- Dynasty Central using CFBR logos instead of selected dynasty logo folders.
- Table view blanking after sortable day-column changes.
- Independents incorrectly triggering 11-team/12-team boundary warnings.
- Extensionless USR-DATA files being rejected by app loaders.

### Known Issues
- Kickoff Classic RLID mappings are only partially confirmed.
- Schedule generation may still occasionally require manual regeneration.
- Custom mod conference policies may need additional tuning.

### Full Notes
See: `Release-Notes/v1.2.0.md`

---

## v1.02.1

### Added
- Built-in Schedule Validation System.
- Validation Report UI popup.
- Clear Schedule Memory button.

### Improved
- Schedule Generator refresh behavior.
- Schedule audit visibility.
- Collision reporting by TGID and week.

### Fixed
- Clear Schedule Memory button layout visibility issue.
- Invalid refresh method calls in Schedule Generator.

### Known Issues
- Validator reports collisions but does not prevent them yet.
- Schedule generation can still produce under/over scheduled teams.

### Full Notes
See: `Release-Notes/v1.02.1.md`

# Changelog

All notable changes to the DoIT Communications UTM Link Builder will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

### Security
- Fixed XSS vulnerabilities by replacing `innerHTML` with safe DOM methods (`textContent`, `createTextNode`) when rendering user-provided data
  - Fixed in link history display (publication names)
  - Fixed in results display (source and medium values)

### Documentation
- Added Security section to README documenting XSS prevention, input sanitization, and data handling practices

## [1.0.0] - 2025-10-05

### Added
- Initial release of DoIT Communications UTM Link Builder
- UTM link generation for 13 communication channels across 3 categories (DoIT, University Tools, Partners)
- Link history with domain grouping and timestamps
- Accessibility features (ARIA labels, keyboard navigation, screen reader support)
- Responsive design for desktop, tablet, and mobile
- Copy functionality with clipboard API fallback for older browsers
- Automatic UTM parameter formatting (lowercase, underscore spaces, remove special chars)
- Detection and removal of existing UTM parameters from URLs

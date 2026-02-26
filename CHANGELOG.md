# Changelog

All notable changes to this project will be documented in this file.

---

## [0.2.0] - 2026-02-26

### Added

- Syntax highlighting for asset directives (v0.2):
  - `@style` / `@endstyle` — with embedded CSS highlighting
  - `@script` / `@endscript` — with embedded JavaScript highlighting
  - `@styles` / `@scripts` — render directives
- Syntax highlighting for stack directives (v0.2):
  - `@push` / `@endpush` / `@stack`
- Syntax highlighting for `@forelse` / `@empty` / `@endforelse`
- Syntax highlighting for `@stop` (alias for `@endsection`)
- Embedded CSS inside `@style` blocks
- Embedded JavaScript inside `@script` blocks
- New snippets:
  - `layout` — official LTE v0.2 view structure with `@push`, `@style`, `@script`
  - `component` — self-contained component with collocated CSS and JS
  - `forelse` — `@forelse` / `@empty` / `@endforelse` loop
  - `style` — inline CSS block
  - `script` — inline JS block with `defer`
  - `push` — `@push` / `@endpush` stack block
  - `include-data` — `@include` with data array
  - `ifelse` — `@if` / `@else` / `@endif`
  - `auth` — `@auth` / `@endauth` guard
  - `guest` — `@guest` / `@endguest` guard
- Repository URL updated to `luany-ecosystem` organisation
- Added `ast` and `compiler` keywords

### Changed

- `layout` snippet updated to official LTE v0.2 view structure

---

## [0.1.0] - 2026-02-22

### Added

- Initial release of Luany LTE extension
- Syntax highlighting for:
  - LTE directives (`@if`, `@foreach`, `@section`, etc.)
  - Echo statements `{{ }}`
  - Raw echo `{!! !!}`
  - `@php` blocks
  - LTE comments `{{-- --}}`
- Embedded PHP support inside LTE templates
- HTML inheritance support
- Basic snippets for common directives

---

## Upcoming

- IntelliSense support for view paths in `@include` and `@extends`
- Advanced directive detection
- View path autocompletion
- LSP integration
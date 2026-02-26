# Luany LTE — VS Code Extension

Official Visual Studio Code extension for **Luany Template Engine (LTE)**.

Provides syntax highlighting, embedded language support, and smart snippets for `.lte` files.

---

## ✨ Features

- 🧠 AST-based syntax highlighting
- 🎨 Embedded CSS inside `@style` blocks
- ⚡ Embedded JavaScript inside `@script` blocks
- 🐘 Embedded PHP inside `{{ }}`, `{!! !!}`, and `@php` blocks
- 🧩 Full directive support — v0.1 and v0.2
- 📦 Smart snippets for all directives

---

## 📘 Supported Directives

### Core
`@if` `@elseif` `@else` `@endif` `@unless` `@endunless`
`@foreach` `@endforeach` `@for` `@endfor` `@while` `@endwhile`
`@forelse` `@empty` `@endforelse`
`@section` `@endsection` `@yield` `@extends` `@include`
`@auth` `@endauth` `@guest` `@endguest`
`@csrf` `@method` `@php` `@endphp`

### Asset Directives (v0.2)
`@style` `@endstyle` `@script` `@endscript` `@styles` `@scripts`

### Stack Directives (v0.2)
`@push` `@endpush` `@stack`

---

## ⚡ Snippets

| Prefix | Description |
|---|---|
| `layout` | Official LTE v0.2 view structure |
| `component` | Self-contained component with CSS and JS |
| `if` | `@if` / `@endif` |
| `ifelse` | `@if` / `@else` / `@endif` |
| `foreach` | `@foreach` / `@endforeach` |
| `forelse` | `@forelse` / `@empty` / `@endforelse` |
| `section` | `@section` / `@endsection` |
| `style` | `@style` / `@endstyle` CSS block |
| `script` | `@script(defer)` / `@endscript` JS block |
| `push` | `@push` / `@endpush` stack block |
| `include` | `@include` partial |
| `include-data` | `@include` with data array |
| `csrf` | `@csrf` hidden input |
| `auth` | `@auth` / `@endauth` guard |
| `guest` | `@guest` / `@endguest` guard |

---

## 🧬 About Luany Template Engine

LTE is a structured, AST-driven template engine for PHP. Parser → AST → Compiler. Zero regex in the entire pipeline.

- `composer require luany/lte`
- [Packagist](https://packagist.org/packages/luany/lte)
- [GitHub](https://github.com/luany-ecosystem/luany-lte)

---

## 📦 Installation

1. Open VS Code
2. Go to Extensions (`Ctrl+Shift+X`)
3. Search for **Luany LTE**
4. Install

---

## 👨‍💻 Author

**António Ambrósio Ngola**
- 📧 [antoniongola.dev@gmail.com](mailto:antoniongola.dev@gmail.com)
- 🌍 Luanda, Angola 🇦🇴


---

## 🗺 Roadmap

| Version | Focus |
|---|---|
| v0.2.x | DX refinement — folding, auto-indent, Emmet, semantic scopes |
| v0.3.x | Engine AST stabilisation — `@forelse`, scope isolation, 96 unit tests |
| v1.0.0 | API freeze — production-ready |
| v1.1.0 | LSP experimental — view path autocompletion, block diagnostics |

> **Stability note:** v0.x series has stable DX and evolving engine. v1.0.0 will mark full API freeze and production readiness.

> **Folding note:** Block folding works correctly when LTE's official indentation is followed (`@style` / `@endstyle`, `@section` / `@endsection`, etc. — both markers remain visible). Full AST-based folding is planned for v0.3.x / LSP.

## 📜 License

MIT
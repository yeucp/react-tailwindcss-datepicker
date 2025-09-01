# Tailwind CSS Compatibility Guide

This library is compatible with both Tailwind CSS 3 and Tailwind CSS 4.

## Tailwind CSS 3 Setup

Standard installation as described in README.md:

```bash
npm install react-tailwindcss-datepicker
```

Use standard PostCSS configuration:

```javascript
// postcss.config.js
module.exports = {
    plugins: {
        tailwindcss: {},
        autoprefixer: {}
    }
};
```

## Tailwind CSS 4 Setup

Install the library and the additional PostCSS plugin:

```bash
npm install react-tailwindcss-datepicker
npm install @tailwindcss/postcss
```

Update your PostCSS configuration:

```javascript
// postcss.config.js
module.exports = {
    plugins: {
        "@tailwindcss/postcss": {},
        autoprefixer: {}
    }
};
```

## Features Compatibility

All features work the same across both versions:

- ✅ Date selection and range picking
- ✅ Dark mode support
- ✅ All color themes
- ✅ Custom styling via classNames prop
- ✅ All props and configurations
- ✅ TypeScript support

## Breaking Changes

**None!** This is a backward-compatible update. Existing projects using Tailwind CSS 3 will continue
to work without any changes.

## Verification

To verify compatibility, run:

```bash
npm run build  # Should work with both TW 3 and 4
npm run dev    # Development server should work
```

The library automatically detects which version of Tailwind CSS you're using and adapts accordingly.

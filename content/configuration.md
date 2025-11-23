---
title: Configuration
---

Quartz is configured through `quartz.config.ts`, a TypeScript file that exports a configuration object.

## Basic Configuration

```typescript
const config: QuartzConfig = {
  configuration: {
    pageTitle: "My Quartz Site",
    pageTitleSuffix: "",
    enableSPA: true,
    enablePopovers: true,
    baseUrl: "https://my-site.com",
    ignorePatterns: ["private", "templates", ".obsidian"],
    defaultDateType: "modified",
    // ... more options
  },
  plugins: {
    transformers: [
      Plugin.FrontMatter(),
      Plugin.SyntaxHighlighting(),
      // ... more transformers
    ],
    filters: [Plugin.RemoveDrafts()],
    emitters: [
      Plugin.ContentPage(),
      Plugin.FolderPage(),
      // ... more emitters
    ],
  },
}
```

## Theme Configuration

Customize the appearance of your site:

```typescript
theme: {
  fontOrigin: "googleFonts",
  cdnCaching: true,
  typography: {
    header: "Schibsted Grotesk",
    body: "Source Sans Pro",
    code: "IBM Plex Mono",
  },
  colors: {
    lightMode: {
      light: "#faf8f8",
      // ... color definitions
    },
    darkMode: {
      light: "#161618",
      // ... color definitions
    },
  },
}
```

## Plugins

Quartz uses a plugin system for customization. Common plugins include:

- **Transformers**: Process and transform content (FrontMatter, SyntaxHighlighting, etc.)
- **Filters**: Filter out content (RemoveDrafts, etc.)
- **Emitters**: Generate output files (ContentPage, FolderPage, etc.)

You can create custom plugins or modify existing ones to suit your needs.

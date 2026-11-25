# Events

One folder per event, named `<year>-<region>-<city>`:

- `2026-eu-amsterdam`
- `2027-eu-barcelona`

Lowercase English city names, hyphens, no accents (`sao-paulo`, not `São Paulo`). Regions are `eu` and `na`, or the country for other events (`japan`, `india`, `china`), the same way CNCF names KubeCon folders.

## Inside an event folder

```text
2027-eu-barcelona/
├── README.md     Dates, status, logo downloads, where files go
├── logos/        The event logo, sorted by format
├── theme/        Colours, fonts, backgrounds, key visual
├── launch/       The launch kit: banners and posts for every platform, Pretix and Sessionize
├── digital/      Everything on a screen after the launch
│   ├── social/   Call for speakers, speaker announcements, reminders
│   ├── website/  Website hero and share image
│   ├── av/       Livestream and recording graphics
│   └── signage/  Digital signage on the venue's screens
├── print/        Everything for a printer or supplier
│   ├── badges/
│   ├── lanyards/
│   ├── signage/
│   └── swag/
└── sponsors/     Sponsor logos and announcement graphics
```

Every event gets the same folders. The README in theme, launch, digital, print and sponsors says what goes in each, at what size and in what format.

## What to deliver

**This repo is where finished files live**, so anyone (organisers, speakers, sponsors, printers) can pick them up. Work in progress stays in [Google Drive](https://drive.google.com/drive/folders/10UNcSu6fb4xXvHCOuWO0ZrPMFtKL0Q9a) until it's signed off.

1. **Ready-to-use formats:** PNG for screens, PDF for print, SVG for anything that needs to scale.
2. **Plus the editable file**, so the next event can reuse it: Illustrator (AI) for design work, InDesign for print layouts if you prefer, and Figma for the website only. Editable files go in a `source/` folder next to the finals.
3. **Screen in sRGB, print in CMYK.** Rejekts Red is #E30613 on screen, CMYK 0 100 100 0 in print, and Pantone 485 C as a spot colour.
4. **Fonts converted to outlines or embedded** in every final file.
5. **Named the Rejekts way**, with the size when it matters (see file names below).
6. **Big files stay in Google Drive.** GitHub's upload limit is 25 MB per file, so video stays in Drive, with a note in the folder saying where.

## File names

```text
rejekts-<year>-<region>-<city>-<asset>-<variant>.<ext>
```

| Example | What it is |
| --- | --- |
| `rejekts-2027-eu-barcelona-logo-horizontal-color.svg` | Horizontal logo, colour, for light backgrounds |
| `rejekts-2027-eu-barcelona-logo-horizontal-reverse.png` | Horizontal logo, for dark backgrounds |
| `rejekts-2027-eu-barcelona-logo-stacked-black.pdf` | Stacked logo, one colour black |
| `rejekts-2027-eu-barcelona-x-banner-1500x500.png` | Launch kit file, with its size |
| `rejekts-2027-eu-barcelona-rollup-870x2270mm.pdf` | Print file, with its size and unit |

Spell `color` the US way in file names, to match CNCF and most tools.

## Event logos

| Layout | Versions |
| --- | --- |
| `horizontal` | `color`, `reverse`, `black`, `white` |
| `stacked` | `color`, `reverse`, `black`, `white` |

- **color:** for light backgrounds
- **reverse:** colour, for dark backgrounds
- **black / white:** one colour, for single-colour print (lanyards, shirts) and busy photos

Each one as **SVG**, **PNG**, **PDF** and **AI**, sorted into one folder per format (`logos/svg/`, `logos/png/`, `logos/pdf/`, `logos/ai/`) so they're easy to browse. List them with download links in the event's README.

### Export settings (Illustrator)

- **Colour:** keep Color Settings on Europe General Purpose and use the Rejekts Red swatch (CMYK 0 100 100 0). Exports come out as #E30613. See [foundations/brand](../foundations/brand/).
- **SVG:** Export As, SVG. Styling: Presentation Attributes. Font: Convert to Outlines. Decimal places: 2. Artboard trimmed to the logo.
- **PNG:** Export As, PNG, 2000 px on the long side, transparent background.
- **PDF:** Save a Copy, Adobe PDF, "High Quality Print", artboard only.

## Starting a new event

1. Copy the folders and READMEs from `2027-eu-barcelona` (everything except the files) into a new folder, and rename it.
2. Fill in its README: dates, city, who's designing.
3. Add the event logo in every layout, version and format above.

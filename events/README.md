# Events

One folder per event, named `<year>-<region>-<city>`:

- `2026-eu-amsterdam`
- `2027-eu-barcelona`

Lowercase English city names, hyphens, no accents (`sao-paulo`, not `São Paulo`). Regions are `eu` and `na`, or the country for other events (`japan`, `india`, `china`), the same way CNCF names KubeCon folders.

## Inside an event folder

```text
2027-eu-barcelona/
├── README.md        Dates, city, status, what's in the folder
├── logos/
│   ├── svg/         Every logo as SVG
│   ├── png/         Every logo as PNG
│   ├── pdf/         Every logo as PDF
│   └── ai/          Every logo as an Illustrator file
├── social/          Save the date, CFP, sponsor and speaker posts
├── web/             Website hero, share image
├── print/           Badges, lanyards, banners, signage
└── video/           Title cards, name banners, sponsor slides
```

Only make a folder once there's something to put in it.

## File names

```text
rejekts-<year>-<region>-<city>-<asset>-<variant>.<ext>
```

| Example | What it is |
| --- | --- |
| `rejekts-2027-eu-barcelona-logo-horizontal-color.svg` | Horizontal logo, colour, for light backgrounds |
| `rejekts-2027-eu-barcelona-logo-horizontal-reverse.png` | Horizontal logo, for dark backgrounds |
| `rejekts-2027-eu-barcelona-logo-stacked-black.pdf` | Stacked logo, one colour black |
| `rejekts-2027-eu-barcelona-save-the-date-1080x1350.png` | Social post, with its size |
| `rejekts-2027-eu-barcelona-rollup-850x2000mm.pdf` | Print file, with its size and unit |

Spell `color` the US way in file names, to match CNCF and most tools.

## Event logos

| Layout | Versions |
| --- | --- |
| `horizontal` | `color`, `reverse`, `black`, `white` |
| `stacked` | `color`, `reverse`, `black`, `white` |

- **color:** for light backgrounds
- **reverse:** colour, for dark backgrounds
- **black / white:** one colour, for single-colour print (lanyards, shirts) and busy photos

Each one as **SVG**, **PNG** and **PDF** in its layout folder, plus the **.ai** source in `logos/source/`.

### Export settings (Illustrator)

- **Colour:** keep Color Settings on Europe General Purpose and use the Rejekts Red swatch (CMYK 0 100 100 0). Exports come out as #E30613. See [foundations/brand](../foundations/brand/).
- **SVG:** Export As, SVG. Styling: Presentation Attributes. Font: Convert to Outlines. Decimal places: 2. Artboard trimmed to the logo.
- **PNG:** Export As, PNG, 2000 px on the long side, transparent background.
- **PDF:** Save a Copy, Adobe PDF, "High Quality Print", artboard only.

## Starting a new event

1. Copy the `2027-eu-barcelona` folder structure and rename it.
2. Fill in its README: dates, city, who's designing.
3. Add the event logo in every layout, version and format above.

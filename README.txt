OPERATION PICKING OVERVIEW — MODULE NO.1
Title/header: MONITOR DISPLAY / OPERATION PICKING OVERVIEW

Try:
1. Extract ZIP.
2. Open index.html in Chrome/Edge/Safari with internet access.
3. Upload both source files: Outstation workbook and Local & IKA workbook.
4. Click Process & Refresh.
5. Filter by Load Plan Type and Date.
6. Export dashboard PNG or filtered Excel report.

Required header titles (matched independent of column order and case/punctuation):
DO No, Est Total Carton, DO Line, Block, Inv Status, Load Plan, Date.
The app validates these headers in both files and reports missing headers.

Current calculation:
- DO count = distinct DO No.
- DO Line and Carton = sum of the corresponding numeric columns.
- Invoice groups are based on Inv Status values containing "Completed" or "Pending".
- DO % = DO count in each invoice status/block divided by total distinct DOs in the selected filters.
- Outstation and Local & IKA source files are combined for All Load Plan.
- This is a local browser prototype; no server upload, shared database, login, or saved cross-device history.
- Validate calculated totals against the official Excel Pivot before operational use.


FIXED VERSION NOTE:
Header matching has been corrected to normalize both the Excel header and its alias, so headers such as 'DO No', 'DO line', 'Est Total Carton', and 'Inv Status' are detected regardless of spaces, case, dots, underscores, or slashes.


MOBILE V3 UPDATE:
- Mobile layout tightened for iPhone screens.
- Report table uses fixed compact columns so all six columns fit without horizontal scrolling.
- Numeric quantities and percentages are rounded to whole numbers (no decimal places).


MOBILE V4 FLEXIBLE UPLOAD:
- Upload Outstation only, Local & IKA only, or both together.
- One uploaded workbook is processed on its own; two workbooks are combined.
- Detects the required seven headers by scanning the first 25 rows and normalizing punctuation, spaces, and case.
- If no file is selected, a clear prompt asks for at least one workbook.


ADMIN DASHBOARD V7-INSPIRED DESIGN V5:
- Dark green glassmorphism dashboard styling inspired by the supplied Admin Dashboard V7 reference video.
- Left glass sidebar, pill-shaped top bar, translucent panels, KPI cards, filters, and responsive compact mobile layout.
- Existing Excel upload/filter/export/chart functions retained.
- Fixed missing statusKind classifier so Completed Invoiced and Pending Invoice rows are classified safely.
- Supports Outstation only, Local & IKA only, or both workbooks.
- Whole-number display for quantities and percentages.


ADMIN DASHBOARD V7 REFERENCE V6:
- Reworked to match the supplied video more closely: slim dark forest-green glass sidebar, pale sage/cream gradient workspace, translucent light panels, rounded white KPI cards, and subtle green accents.
- Main workspace is intentionally light, not the dark full-screen green style from V5.
- Preserves upload/filter/report/export/chart behavior and compact mobile layout.


ADMIN DASHBOARD V7 TRUE LAYOUT V7:
- Rebuilt the page structure based on the supplied Admin Dashboard V7 video: fixed vertical dark green sidebar, top search/profile bar, main workspace heading/actions, separate data-source panel, filter strip, KPI stat cards, report table and analytics charts.
- Mobile collapses sidebar into a compact horizontal navigation and stacks panels/cards.
- Existing data processing, flexible single/both workbook upload, filtering, PNG/Excel export, and chart rendering IDs preserved.


ADMIN DASHBOARD REFERENCE DESIGN V8:
- Rebuilt the visual layout to closely follow the supplied reference image: dark vertical left sidebar (Home/Analytics/Reports/Settings), light mint workspace, Dashboard header with Generate Report button, four horizontal KPI cards, two side-by-side analytics panels, and bottom Recent Activity + Block Status panels.
- Added compact Data Source and Filter controls while preserving required upload workflow.
- Existing flexible single workbook or combined two-workbook upload retained.
- Report table remains available below dashboard widgets; quantities and percentages display as whole numbers.
- Mobile responsive: sidebar becomes horizontal navigation, cards become 2 columns, charts and bottom panels stack vertically.


COMPACT DESKTOP-STYLE MOBILE V9:
- Mobile retains desktop-style left navigation as a narrow fixed icon rail instead of moving the full sidebar above the dashboard.
- Compact top header, data source and filters.
- KPI cards stay in a 2x2 grid; analytics charts remain side-by-side; activity and quick-view panels remain side-by-side.
- Table columns are fixed to fit the available screen width with compact typography and no horizontal overflow.
- Smaller panel padding, card heights and chart heights to reduce excessive scrolling and oversized layout.


COMPACT KPI ROW V10:
- Four KPI cards display in one horizontal row on mobile screens.
- Added a distinct icon tile for Total DO, Completed Invoiced, Pending Invoice, and Total Cartons.
- Reduced card padding and typography to keep all four metrics visible in a narrow phone viewport.


CLEAN REPORT V11:
- Removed the two analytics chart panels and the Recent Activity / Block Status panels marked with red X in the user's screenshot, keeping the dashboard focused on the invoice report.
- Completed and Pending KPI cards now show their corresponding carton totals alongside DO percentage.
- Strengthened title and KPI typography.
- Rebuilt invoice table with grouped status summary rows, soft row backgrounds, rounded group bands, no horizontal grid lines, and a distinct grand total band for faster reading.


PC FIT & VISUAL UPDATE V12:
- Desktop/PC layout uses the full viewport height with compact header, upload panel, filters, KPI row and invoice report table so the key report can fit on one screen on typical desktop displays.
- DO percentages display one decimal place (e.g. 31.0%).
- Pending Invoice summary and block detail rows use a full-row light red treatment.
- Current Malaysia date/time is shown at the end of the report title and refreshes every second.
- Improved contrast with a clearer navy/white/emerald palette and darker typography.
- KPI icons are larger, high-contrast, embossed/3D-style tiles.


SMART FULL-WIDTH DESKTOP V13:
- Desktop content now uses the full available width after the sidebar; removes the narrow centered content canvas.
- Sidebar fixed at 220px; main dashboard expands fluidly to remaining screen width.
- Compact header, data upload, filters, four KPI cards and report table are vertically fitted into the viewport.
- Upload fields align in one desktop row; filters and cards use consistent grid spacing.
- Table fills remaining vertical space with fixed column layout and high-contrast styling.


SCROLL & STATUS TITLE FIX V14:
- Restored normal vertical page scrolling on desktop and tablet. No fixed-height clipping of the report.
- Sidebar remains sticky while the dashboard content scrolls.
- Report table can extend naturally and remains horizontally scrollable if required.
- Corrected report heading from 'Overall Block Current Order Invoice Stats' to 'Overall Block Current Order Invoice Status'.


UI DESIGN V15:
- Calm enterprise palette: deep navy navigation, cool white/blue-gray workspace, emerald completed accents, soft red pending accents, restrained gold carton accent.
- KPI cards have clearer hierarchy and larger embossed icon tiles.
- Report area is split into a wide main invoice-status table and a dedicated right-side Region Status panel, matching the user's layout sketch.
- Region Status is a clean placeholder only; no regional metrics are fabricated before the user provides Region Status rules/data.
- Responsive behavior stacks Region Status below the report on narrower screens.


BY BLOCK STATUS V16:
- Right panel renamed to By Block Status and dynamically displays Blocks E/F/G/H.
- Metrics: total unique DOs, total cartons, completed DOs, pending DOs, and completion percentage.
- Completion percentage = completed unique DOs divided by total unique DOs in each block.
- Panel updates automatically with the current Load Plan Type and Load Plan Date filters.
- Desktop sidebar narrowed to 176px; secondary text contrast increased for readability.


V17 PREMIUM CORPORATE DESIGN:
- New premium navy/white corporate design system with high-contrast dark text.
- Compact 190px desktop sidebar and responsive icon-only sidebar on narrower screens.
- Header restyled with navy gradient, dashboard subtitle, current time and green Generate Report action.
- Four KPI cards remain on one row on desktop; icon tiles are larger and use restrained blue/green/red/gold accents.
- Main invoice status table and By Block Status remain side-by-side on desktop.
- Completed rows use subtle green; Pending rows use subtle red; Grand Total uses deep navy.
- By Block Status panel uses navy title bar, clean progress bars, and high-contrast labels.
- Removed duplicate chart and recent-activity panels from the visible report canvas to prioritize the primary operational report.
- Existing Excel parsing, independent/both workbook uploads, filters, calculations, exports and date-time logic retained.

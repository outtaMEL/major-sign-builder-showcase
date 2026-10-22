# Major Sign Builder

**Exploring a more direct guide-sign design workflow from a road engineer's experience.**

Engineering product prototype by Fan Niu. My contribution centres on identifying the workflow problem, product direction, requirements and iterative review; implementation was primarily completed with AI assistance.

[Try the online editor](https://major-sign-builder.vercel.app/trial)

The anonymous trial supports editing. Saving and exporting require access beyond trial mode.

![A sample guide sign with board dimensions and geometry controls](assets/board-configuration.jpg)

*A sample sign shown with physical dimensions, border settings, corner geometry and panel styling.*

## Why I built it

While working as a road engineer, I found sign design conceptually straightforward: arranging geometry, text and spacing. The AutoCAD plug-ins I used made revisions cumbersome. A local change could affect other parts of the layout and create substantial rework.

After discovering what AI-assisted coding could help me build, I explored whether a dedicated browser editor could make the process more direct, connecting element editing, parameter adjustments, previews and CAD handoff.

## The product response

The project grew from an arrow-building prototype into a broader sign-layout workspace. It combines text, graphical elements, panels and board configuration, using millimetres for geometry and selected AS 1742/1743-related layout rules.

![A placed text group selected on the editing canvas](assets/element-layout.jpg)

*The editor represents sign content as selectable elements on a layout canvas.*

The CAD export implementation includes line and arc entities for arrow geometry, together with text and layer handling. The product aim is a design that remains useful for continued work in CAD after leaving the browser.

## Feedback from industry

I demonstrated the prototype to a friend working in the industry. Two concrete requests were:

- Point-to-point snapping between elements, followed by numerical distance entry for precise placement.
- Separate CAD layers for different elements, to support downstream organisation and editing.

This feedback supplied specific requirements for reviewing both placement interactions and the exported file. These are recorded here as feedback received.

## Industry exploration and current stage

I also explored commercialisation and tried to interest industry practitioners in the product. Those contacts did not develop into an ongoing commercial project, and I did not carry the commercial effort forward. The project remains available as a functional prototype.

The editor uses React and TypeScript, with geometry and DXF export modules. The wider application includes Supabase-related authentication and storage code and subscription integrations.

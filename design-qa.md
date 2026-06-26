**Source visual truth**
- Reference: https://www.aseng.ru/
- Source content: https://vmc34.ru/
- Browser used for visual QA: Yandex Browser via Computer Use, desktop viewport.

**Implementation checked**
- Local file: `file:///Users/kristinakarpova/Documents/VMS/index.html`
- Local server: `http://127.0.0.1:8123/`
- Deploy archive: `dist/vmc34-timeweb-static.zip`

**Visual QA notes**
- Header now follows the reference rhythm: white sticky bar, centered nav, red CTA, red underline. Top navigation now mirrors the AS route more closely: `Решения`, `Услуги`, `Продукция`, `Отрасли`, `Проекты`, `О компании`, `Карьера`; contact is handled by the separate red CTA.
- Hero now uses a wider, colder VMC industrial image with centered brand/title and a lighter AS-like overlay.
- Post-hero strip now behaves like the reference logo/client strip, but uses verified VMC component brands with strict dividers instead of copied AS client logos.
- Intro block now matches the reference pattern: full-width red band, centered white text, strong industrial pause, with actual VMC company description from the source site.
- Services now use a gray field and open engineering grid with restrained engineering indices instead of white landing-page cards; service names/texts now come from VMC source content.
- Product block no longer has text/image overlap; desktop layout is a stable two-column grid with VMC full-cycle production copy and the four project cards folded into the same product area.
- Numbers use conservative VMC facts: service directions, component brands, product groups, and full-cycle delivery.
- Numbers now include the reference-like `Больше о нас` CTA under the metrics block instead of ending as a generic stat grid.
- The former "Ключевые клиенты" label was not reused because VMC source content does not provide verified client logos.
- The former body "Отрасли и задачи" section was removed; industry links now live in the header/footer like the reference navigation structure.
- Real VMC component brands now sit directly after the numbers block as `Ключевые комплектующие`, matching the position and rhythm of the AS key-clients strip without inventing clients.
- Projects now use the four real VMC project/product labels from the source site and appear before the numbers block, so the page rhythm is closer to the AS reference structure.
- Benefits now use numbered text cells, closer to AS Engineering than generic cards, and the statements now match source VMC advantages.
- A short `Карьера` block was added before contacts to match the AS structure without inventing open vacancies.
- Contact CTA now leads to a visible static form directly under the contact image, matching the AS reference structure more closely than the previous hidden hash-modal.
- Contact data now includes VMC requisites and address from the source site.

**Intentional differences**
- No AS Engineering logos, client logos, Tilda code, remote fonts, or hotlinked assets were copied.
- VMC does not appear to have verified large customer logos/metrics on the source site, so the page uses factual VMC industries, product groups, and conservative numbers.
- Services use text numbering instead of borrowed AS icon assets to keep the site static, legal, and dependency-free for the smallest Timeweb tariff.

**Technical QA**
- `index.html` parsed successfully with Python `HTMLParser`.
- CSS brace balance: 160 opening braces, 160 closing braces.
- Local asset references checked: 9 refs, 0 missing.
- Hash links checked: 37 links, 0 missing targets.
- Forbidden external/template checks passed: no `@import`, `tilda`, `aseng`, `googleapis`, `letter-spacing`, or `vw` usage in `index.html` / `style.css`.
- Yandex Browser DOM/accessibility check confirms the updated top navigation with `Продукция`, `Отрасли`, `Проекты`, `Карьера`, the component-brand strip under hero, VMC service names, product CTA to `#projects`, project labels inside the product block, `Ключевые комплектующие`, benefits, career CTA, visible contact form fields, requisites, and the numbers CTA.
- Local HTTP checks returned `200 OK` for `/`, `/style.css`, `/assets/img/automation-panel.webp`.
- ZIP check: `dist/vmc34-timeweb-static.zip`, 18 entries, about 1.0 MB.
- ZIP excludes `design-qa.md`, `.omx`, skills, and temporary files.
- Playwright mobile viewport check was attempted, but the local CLI requires Google Chrome at `/Applications/Google Chrome.app`, which is not installed. No browser was installed as part of this static-site cleanup.

**Residual risk**
- Exact 95% visual fidelity is not claimable because AS Engineering has proprietary brand assets, client logos, and icon artwork that were intentionally not copied.
- The result is now structurally and visually aligned with the reference while preserving VMC content and static-hosting constraints.
- Mobile CSS is present, but final mobile visual QA still needs a real narrow viewport check because Playwright could not start without Chrome.

**Final result**
manual visual pass with intentional differences

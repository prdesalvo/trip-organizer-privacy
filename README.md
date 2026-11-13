# Pin and Plot website

Public product/share page: https://prdesalvo.github.io/trip-organizer-privacy/pin-and-plot/

The product page is static HTML and CSS in `pin-and-plot/`. GitHub Pages publishes
from this repository. Keep the existing root `index.md` privacy policy,
`support.md` and `_config.yml` in place: App Store Connect already links to them.

## Editing

- Edit `pin-and-plot/index.html` for page copy, links and Open Graph metadata.
- Edit `pin-and-plot/style.css` for responsive presentation. No build step or
  JavaScript dependency is needed.
- Keep the App Store button linked to app ID `6800444562`.
- Images are the app's publicly listed icon/screenshots. The Switzerland trip
  is example content. No analytics, external fonts or additional services are added.

## Messages preview

The canonical URL and `og:url` must use the public product-page URL above.
`og:image` points to `pin-and-plot/assets/share-v1.jpg`, a 1200 × 630 JPEG.
The title, description and image are present directly in HTML, without a
JavaScript requirement or redirect to the App Store. The webpage provides
a separate App Store download link and a Smart App Banner app ID.

The editable artwork composition is `tools/pin-and-plot-share.html`. Serve the
repository root with a static server, open that file at a 1200 × 630 viewport,
and export a viewport screenshot as JPEG to regenerate the preview. When
changing the image, use a new filename and update the metadata; clients may
cache link previews. Test a newly pasted URL in Messages. Do not send a GitHub
repository/blob URL or the App Store URL when expecting this page's preview.

Apple guidance: https://developer.apple.com/documentation/technotes/tn3156-create-rich-previews-for-messages

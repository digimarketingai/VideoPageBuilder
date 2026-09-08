# Chinese Restaurant Website Creator

A browser-based editor for a customizable bilingual restaurant website.

No installation, build tools, or server are needed to use the editor.

## Start

1. Save the code as `creator.html`.
2. Open it in your browser.
3. Customize the fields in the left-hand panel.
4. Check the live preview.
5. Click **Export website — index.html**.
6. Open the downloaded `index.html` and test it.

JavaScript must be enabled.

## What can be customized?

### Brand and homepage

- Restaurant name in English and Chinese
- Small introductory heading
- Main headline
- Homepage description
- Gallery and menu button text
- Accent and highlight colors
- Default language

### Menu section

- Menu heading
- Menu subtitle
- Details and back button text
- Previous and next media button text

### Every dish

- English and Chinese names
- Price
- English and Chinese descriptions
- Fallback emoji or symbol
- Multiple images and videos
- Media captions
- Position in the menu

Add or delete dishes using the editor controls.

Prices are free-form text. Examples:

- `$12.50`
- `¥68`
- `$8 / $12`
- `From $15`
- `Market price`

Leave a price empty to hide it.

### Closing section

- Closing message in both languages
- Footer text in both languages

## Images and videos

Media can be added to:

1. The main restaurant gallery
2. Each individual dish

Use **Upload** to select one or several files at once.

Or paste a direct media URL, choose **Image** or **Video**, and
click **Add URL**.

Use the up/down buttons to reorder media.
Use **Remove** to delete an item.

The caption also provides the image description used as alt text.

### Supported uploads

- Browser-readable images
- MP4 videos
- WebM videos

Some image formats and video codecs may not play in every browser.
Test your actual files in the browsers you intend to support.

The editor limits each uploaded file to 30 MB.
Keep total media size small as well.

### Direct URLs

Examples:

    https://your-domain.com/images/dumplings.jpg
    https://your-domain.com/videos/restaurant.mp4

These are examples; replace them with real links.

Use direct media file URLs, preferably HTTPS.
YouTube watch pages, TikTok pages, and cloud sharing pages are not supported.

A correctly formatted URL does not guarantee that its media will load.
The host must allow access, and the file must remain available.

### Embedded uploads versus links

Uploaded files:

- Are read locally by the editor
- Are embedded in the exported HTML and saved project
- Do not require separate media files
- Make exports larger

URL media:

- Remains hosted externally
- Requires access to its host
- May expire or stop working
- Is fetched when displayed in the editor or website

Do not use private or sensitive URLs in a publicly shared website.

## Flip effects

### Media galleries

With two or more media items, previous/next buttons appear.
Switching media uses a flip-style transition.

With one media item, it is displayed without navigation buttons.

Videos do not autoplay.
Visitors use the normal video controls.

Changing gallery items pauses the outgoing video.

### Dish cards

The details button flips the dish card to show its description.
The back button returns to the front.

Pressing Escape on the back of a card also returns it to the front.

Flipping a card pauses videos inside it.

Reduced-motion preferences disable the animation while preserving
the controls and content.

## Save your editable project

Click **Save project** to download:

    restaurant-project.json

Later:

1. Open `creator.html`.
2. Click **Load project**.
3. Select the saved JSON file.
4. Confirm replacement of the current editor contents.

The project includes uploaded media.

Edits are not automatically saved.
Save your project before closing or refreshing the editor.

An exported `index.html` is the finished website, not an editable
project file. Keep the JSON project for future changes.

## Preview

Desktop and Mobile buttons change the preview width.

Edits refresh the preview after a short delay.
Refreshing resets language selection, card position, and video playback.

The exported website starts using the default language selected
in the editor.

## Publishing

Upload the exported `index.html` to your static website host.

If you used only uploaded media, all website media is embedded.
If you used URL media, those external links must stay available.

Test the published page, especially media links and video playback.

## Important limitations

- This is a restaurant presentation website.
- It does not process orders, bookings, payments, or inventory.
- Menu prices are display text, not checkout calculations.
- Initial dish names and prices are examples.
- Large amounts of embedded media can slow the editor and website.
- Only publish media you have permission to use.

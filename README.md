# Recipes

A personal recipe collection, beginning with **Thanksgiving 2026**.

**Website:** https://eric-czech.github.io/recipes/

The site is a single, self-contained `index.html`: recipe text, CSS, and four compressed photographs are embedded in that file. It works offline and has responsive screen layouts and print styles. There are no external fonts, JavaScript libraries, package dependencies, or build steps. The Print collection button uses the browser’s built-in printing.

## Collections

- Thanksgiving 2026 — slow-cooker turkey breast with lemon-garlic gravy; stuffed butternut squash; caramelized carrot tarte Tatin with ginger; sunshine salad with carrot-ginger dressing.

Collections are represented by semantic sections inside `index.html`. Add future collections as additional sections and add links in the collection navigation. Recipe IDs provide stable links within the page.

## Editing and publishing

Edit `index.html` and push to `main`. GitHub Pages publishes the repository root. To preview locally, open `index.html` in a browser, or run:

~~~sh
python3 -m http.server 8765
~~~

Then open http://localhost:8765.

## Sources and editorial treatment

- **Slow-cooker turkey breast with lemon-garlic gravy:** Sarah DiGregorio, NYT Cooking, November 4, 2024. Transcribed from the supplied PDF. Ingredient quantities, cooking temperature, method, and smaller-batch variation are retained; formatting and wording are made consistent. The original author’s 155°F pull temperature is explicitly identified, with its broiling and resting sequence preserved.
- **Stuffed butternut squash:** Eric’s handwritten notes, November 2024. Expanded into a usable ingredient list and method. Unspecified amounts are estimates for two medium squashes. The half cup of cheese is interpreted as a quarter cup each of cheddar and Parmesan. A 10–15 minute final bake is added and identified in the recipe note.
- **Caramelized carrot tarte Tatin with ginger:** Nicole Hopper, Food & Wine, March 2025, pages 44–45. Transcribed from the supplied spread, preserving quantities, temperatures, sequence, ginger-juice note, and suggested wine pairing. Photography by Greg DuPree; food styling by Margaret Dickey; prop styling by Christina Daley.
- **Sunshine salad with carrot-ginger dressing:** Noor Murad and Yotam Ottolenghi, Ottolenghi Test Kitchen: Extra Good Things, page 150. Transcribed from the supplied spread, preserving quantities, method, storage advice, and the optional unstrained texture. The book’s unexplained “Cook time: 15 minutes” label is omitted from the displayed timing; the written method uses no heat. Photography by Elena Heatherwick.

Published recipe descriptions have been replaced with short summaries. Original source PDFs are not included. Source recipes and photographs retain their respective authors’ and publishers’ rights; this repository does not apply a blanket license to that material.

## Images

All four final images are compressed JPEG data URLs embedded in `index.html`.

- Carrot tart and salad: photograph regions extracted from the supplied scanned pages and compressed for the web.
- Turkey and squash: generated using the built-in image-generation tool, then compressed for the web. Each is identified as an AI-generated illustration in its caption.

### Generation prompts

**Turkey:** Use case: photorealistic-natural. Asset type: recipe website photograph, horizontal 3:2 composition. Create an editorial food photograph of slow-cooker turkey breast finished under a broiler, not a whole turkey. A golden brown skin-on turkey breast on a plain ivory serving platter, one end neatly carved into white-meat slices. A small ceramic jug of rustic lemon-garlic gravy beside it, a modest rosemary sprig, quiet light wooden table, soft natural window light, realistic cooked texture. Close three-quarter overhead composition; food fills the frame but entire platter visible. Restrained, home-cooked Thanksgiving mood. No stuffing, no whole bird, no legs or wings, no cranberries, no text, no labels, no watermark.

**Squash:** Use case: photorealistic-natural. Asset type: recipe website photograph, horizontal 3:2 composition. Create an editorial food photograph of two lengthwise halves of maple-roasted butternut squash on a simple ivory platter. The seed cavities and some cut surface are mounded with a coarse chopped filling of bacon, diced sunchokes, long green beans, sage, breadcrumbs, and grated cheddar and Parmesan. Top with deep golden caramelized onion ribbons. The long orange necks are lightly glazed with maple and walnut oil and dotted with toasted chopped walnuts. A little fresh parsley is scattered over the finished squash. Skin is on, flesh is tender roasted orange, visibly real food rather than perfect styling. Quiet light wooden table, soft natural window light, close three-quarter overhead view, entire food composition visible with small margins. No rice, no quinoa, no dried cranberries, no text, no labels, no watermark.

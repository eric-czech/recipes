# Recipes

A personal recipe collection, beginning with **Thanksgiving 2026**.

**Website:** https://eric-czech.github.io/recipes/

The site is a single, self-contained `index.html`: recipe text, CSS, and eight compressed images are embedded in that file. It works offline and has responsive screen layouts and print styles. There are no external fonts, JavaScript libraries, package dependencies, or build steps. The Print collection button uses the browser’s built-in printing.

## Collections

- Thanksgiving 2026 — blood orange and rosemary Paloma pitcher; cranberry cornbread focaccia; baked Brie with fig jam, crispy prosciutto and rosemary; slow-cooker turkey breast with lemon-garlic gravy; stuffed butternut squash; caramelized carrot tarte Tatin with ginger; sunshine salad with carrot-ginger dressing; Lisbon chocolate cake.

Collections are represented by semantic sections inside `index.html`. Add future collections as additional sections and add links in the collection navigation. Recipe IDs provide stable links within the page. On phones and tablets, the recipe index is a native collapsible menu and the text reflows into a single column on narrower screens. Mobile primary controls have a minimum 44-pixel tap height.

## Editing and publishing

Edit `index.html` and push to `main`. GitHub Pages publishes the repository root. To preview locally, open `index.html` in a browser, or run:

~~~sh
python3 -m http.server 8765
~~~

Then open http://localhost:8765.

## Sources and editorial treatment

- **Blood orange and rosemary Paloma pitcher:** Thanksgiving 2026 family notes, page 1. Preserves the syrup infusion, six-serving batch, quantities, and make-ahead instructions. Lime juice is listed by the source’s primary measure of one-third cup; its inconsistent three-ounce equivalent is omitted.
- **Cranberry cornbread focaccia:** Thanksgiving 2026 family notes, page 2. Transcribed from the embedded recipe image, retaining the cornmeal, cranberries, rosemary, two rises, quantities, and baking instructions.
- **Baked Brie with fig jam, crispy prosciutto and rosemary:** Thanksgiving 2026 family notes, page 3. Preserves ingredient quantities, the 350°F oven, optional scoring, serving accompaniments, and make-ahead advice. Displayed baking time follows the method’s 10–15 minutes.
- **Lisbon chocolate cake:** Dorie Greenspan, NYT Cooking, updated September 16, 2025. Transcribed from the supplied chocolate cake PDF. Quantities and all nine steps are retained, including ganache chilling, pan support, the two-hour assembled chill, and storage for up to two days.
- **Slow-cooker turkey breast with lemon-garlic gravy:** Sarah DiGregorio, NYT Cooking, November 4, 2024. Transcribed from the supplied PDF. Ingredient quantities, cooking temperature, method, and smaller-batch variation are retained; formatting and wording are made consistent. The original author’s 155°F pull temperature is explicitly identified, with its broiling and resting sequence preserved.
- **Stuffed butternut squash:** Eric’s handwritten notes, November 2024. Expanded into a usable ingredient list and method. Unspecified amounts are estimates for two medium squashes. The half cup of cheese is interpreted as a quarter cup each of cheddar and Parmesan. A 10–15 minute final bake is added and identified in the recipe note.
- **Caramelized carrot tarte Tatin with ginger:** Nicole Hopper, Food & Wine, March 2025, pages 44–45. Transcribed from the supplied spread, preserving quantities, temperatures, sequence, ginger-juice note, and suggested wine pairing. Photography by Greg DuPree; food styling by Margaret Dickey; prop styling by Christina Daley.
- **Sunshine salad with carrot-ginger dressing:** Noor Murad and Yotam Ottolenghi, Ottolenghi Test Kitchen: Extra Good Things, page 150. Transcribed from the supplied spread, preserving quantities, method, storage advice, and the optional unstrained texture. The book’s unexplained “Cook time: 15 minutes” label is omitted from the displayed timing; the written method uses no heat. Photography by Elena Heatherwick.

Published recipe descriptions have been replaced with short summaries. Original source PDFs are not included. Source recipes and photographs retain their respective authors’ and publishers’ rights; this repository does not apply a blanket license to that material.

## Images

All eight final images are compressed JPEG data URLs embedded in `index.html`.

- Focaccia: the image above the recipe in the Thanksgiving 2026 PDF, extracted and compressed for the web.
- Carrot tart and salad: regenerated using the supplied photograph regions as references. Ingredients, garnishes, and distinctive plating are retained, with lighting and framing made consistent with the other images. Original reference photography is credited in the sources above. The displayed illustrations are identified as AI-generated.
- Paloma, Brie, turkey, squash, and chocolate cake: generated using the built-in image-generation tool, then compressed for the web. Each is identified as an AI-generated illustration in its caption.

### Generation prompts

**Turkey:** Use case: photorealistic-natural. Asset type: recipe website photograph, horizontal 3:2 composition. Create an editorial food photograph of slow-cooker turkey breast finished under a broiler, not a whole turkey. A golden brown skin-on turkey breast on a plain ivory serving platter, one end neatly carved into white-meat slices. A small ceramic jug of rustic lemon-garlic gravy beside it, a modest rosemary sprig, quiet light wooden table, soft natural window light, realistic cooked texture. Close three-quarter overhead composition; food fills the frame but entire platter visible. Restrained, home-cooked Thanksgiving mood. No stuffing, no whole bird, no legs or wings, no cranberries, no text, no labels, no watermark.

**Squash:** Use case: photorealistic-natural. Asset type: recipe website photograph, horizontal 3:2 composition. Create an editorial food photograph of two lengthwise halves of maple-roasted butternut squash on a simple ivory platter. The seed cavities and some cut surface are mounded with a coarse chopped filling of bacon, diced sunchokes, long green beans, sage, breadcrumbs, and grated cheddar and Parmesan. Top with deep golden caramelized onion ribbons. The long orange necks are lightly glazed with maple and walnut oil and dotted with toasted chopped walnuts. A little fresh parsley is scattered over the finished squash. Skin is on, flesh is tender roasted orange, visibly real food rather than perfect styling. Quiet light wooden table, soft natural window light, close three-quarter overhead view, entire food composition visible with small margins. No rice, no quinoa, no dried cranberries, no text, no labels, no watermark.


**paloma:** Use case: photorealistic-natural. Asset type: family recipe website photograph, horizontal 3:2 composition. Editorial food photograph of a clear glass pitcher of blood orange and rosemary Paloma base beside two short glasses filled with reddish blood-orange cocktail, fresh ice, a blood orange wheel and one fresh rosemary sprig each. The pitcher has no ice. The recipe is blanco tequila, blood orange juice, lime juice and rosemary agave syrup, with club soda added to the glasses. Simple light wooden table, soft natural window light, modest real home serving, close three-quarter overhead view. No salted or sugared rims, no grapefruit, no text, no watermark, no decorative party props.

**brie:** Use case: photorealistic-natural. Asset type: family recipe website photograph, horizontal 3:2 composition. Editorial food photograph of a small round baked Brie wheel, roughly 8-10 ounces, on a simple ivory serving plate, topped with dark fig jam, crisp crumbled prosciutto shards and finely chopped rosemary. A small opening shows the warm creamy cheese. A whole fresh rosemary sprig as garnish, a few baguette slices and crisp apple slices beside the cheese. Quiet light wooden table, soft natural window light, realistic home-cooked food texture, close three-quarter overhead composition. No pastry wrapping, no honey pour, no nuts, no cranberries, no text, no watermark.

**chocolate-cake:** Use case: photorealistic-natural. Asset type: family recipe website photograph, horizontal 3:2 composition. Editorial food photograph of a Lisbon chocolate cake: a low round nine-inch dense brownielike chocolate cake base with a distinct soft whipped chocolate ganache mousse layer on top, finished with a generous matte dusting of unsweetened cocoa powder. One wedge removed and placed next to the cake shows the dense cake and airy mousse cross-section, both deep brown. Plain ivory serving plate on a quiet light wooden table, soft natural window light, close three-quarter overhead view. Understated real home-baked appearance. No tall sponge layers, no shiny glaze, no berries, no piped frosting, no whipped cream decorations, no text, no watermark.

**salad-refreshed:** Use case: style-transfer. Asset type: family recipe website photograph. The supplied image is the reference and edit target: sunshine salad with carrot-ginger dressing. Regenerate it as a fresh, clear food photograph consistent with the other recipe photos: soft natural window light, neutral warm wooden table, realistic crisp textures, natural saturated food colors, no washed-out book-page cast. Horizontal 3:2 image. Preserve the essential dish and plating: a wide dark-rimmed oval platter with a generous smooth vivid orange carrot-ginger dressing coating its base, smashed chunky cucumber half-moons with dark green skin and pale interiors, thin avocado crescents, very thin purple red-onion rings, Thai basil leaves, toasted white sesame seeds, and a little sesame oil. Dressing remains visibly exposed around the edge, ingredients loosely piled in the center. Show the complete platter with small margins from a close three-quarter overhead angle. Keep all ingredients; do not introduce tomatoes, radishes, citrus slices, croutons, or new garnishes. No text, no watermark. It should look like the same recipe freshly prepared, not a photograph of a printed page.

**carrot-refreshed:** Use case: style-transfer. Asset type: family recipe website photograph. The supplied image is the reference and edit target: caramelized carrot tarte Tatin with ginger. Regenerate it as a fresh, clear food photograph consistent with the other recipe photos: soft natural window light, neutral warm wooden table, realistic textures, warm natural food color without blown highlights or an oversaturated book-page cast. Horizontal 3:2 image. Preserve the essential dish and distinctive details: a round upside-down savory tart on a plain ivory plate, tightly arranged lengthwise halves of small roasted orange and red-orange carrots running in roughly parallel rows, glossy orange-ginger caramel glaze, deeply browned puff-pastry edge, a wedge cut and slightly separated, small crumbles of white feta, chopped pale toasted hazelnuts, and delicate feathery fresh dill. Whole tart and cut wedge visible, close three-quarter overhead composition. Do not replace the carrots with tomatoes or beets, do not add leafy salad or walnuts or different cheese, no new garnishes. No text, no watermark. It should look like the same recipe freshly prepared, not a photograph of a printed page.

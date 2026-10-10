### STITCH MASTER DESIGN SYSTEM — LABELTRUTH

Design a complete premium mobile application called **LabelTruth**.

LabelTruth is a food-label transparency app. Users scan packaged food barcodes or ingredient labels, and the application analyzes the product to show health score, NOVA processing level, ingredients, additives, E-numbers, hidden sugars, marketing claims and personalized considerations.

The product should feel like a real consumer application that could ship on the App Store.

VISUAL DIRECTION:

Apple-level restraint.  
Airbnb-level clarity.  
Premium health-tech aesthetic.

Use:

- warm off-white backgrounds
    
- charcoal/black primary typography
    
- restrained green accent
    
- amber and red only for semantic status indicators
    
- large editorial typography
    
- generous whitespace
    
- 20–28px rounded cards
    
- thin subtle borders
    
- extremely soft shadows
    
- sophisticated modern sans-serif typography
    
- native iOS-style controls
    
- subtle micro-interactions
    
- smooth transitions
    
- excellent accessibility and contrast
    

Avoid:

- neon colors
    
- excessive gradients
    
- glassmorphism
    
- generic AI robot imagery
    
- stock-photo-heavy layouts
    
- excessive icons
    
- cluttered dashboards
    
- overly colorful nutrition apps
    
- gamification
    
- giant decorative illustrations
    

CORE NAVIGATION:

Use a three-item bottom navigation:  
Home  
History  
Profile

Scanning is the primary action and should be visually dominant on Home rather than being a standard navigation tab.

CORE PRODUCT EXPERIENCE:

Home → Barcode Scanner OR Label Scanner → Analysis → Results.

The Results screen is the flagship screen.

RESULTS INFORMATION:

Barcode results may contain:  
product_name  
nova_upf_level  
ingredients  
flagged_additives  
health_score  
badge_color  
personalized_warning

Label image results may contain:  
product_type  
extracted_ingredients  
hidden_sugars_found  
e_numbers_found  
estimated_nova_level  
greenwashing_claims_detected  
verdict_summary  
health_score  
badge_color  
personalized_warning

History contains:  
product_name  
nova_level  
verdict  
scan id

Profile contains:  
email  
dietary_condition

DESIGN PRINCIPLE:

The application should make complex food-label information feel simple.

Users should understand the result within approximately three seconds.

Prioritize:

1. Product identity
    
2. Health score
    
3. Status
    
4. NOVA processing level
    
5. Personalized consideration
    
6. Ingredient evidence
    
7. Additives
    
8. Marketing claim review
    
9. Verdict
    

The interface should communicate information, not make exaggerated medical claims.

Create a coherent design system where every screen shares the same typography, spacing, corner radius, iconography, navigation, button styles and interaction patterns.

Design specifically for a modern iPhone mobile viewport.

The finished product should look like a polished startup product with the refinement of an Apple-designed consumer application.

Every prompt below should inherit this visual language.

- Premium minimalist mobile app
- iOS-inspired design
- White / very light warm-gray background
- Black and charcoal typography
- One restrained green accent
- Extremely subtle amber/red status colors only where semantically necessary
- Large rounded cards, approximately 20–28px radius
- Thin borders instead of heavy shadows
- Soft shadows only where needed
- SF Pro / Inter-style typography
- Large editorial headings
- Compact secondary labels
- Generous whitespace
- Beautiful micro-interactions
- No excessive gradients
- No glassmorphism everywhere
- No neon
- No generic "AI" robot imagery
- No stock food photography unless absolutely necessary
- High-end health/productivity app aesthetic
- Accessibility-conscious contrast
- Designed specifically for a modern iPhone screen
- Components should feel native to iOS
- Use realistic food/product data, not lorem ipsum

And importantly:

**Every screen must look like the same product.**

# SCREEN 01 — Splash Screen

This is extremely simple.

The app shouldn't open with some giant animated logo screaming at the user.

Think Apple.

### Visual

White/off-white background.

Centered:

**LabelTruth**

Small line beneath:

> Know what's really inside.

Very subtle animated mark — perhaps a scanning line moving through the wordmark.

---

### STITCH PROMPT — SPLASH SCREEN

Design a premium minimalist splash screen for a mobile app called **LabelTruth**, an intelligent food-label transparency app.

The screen should feel like an Apple-designed health/productivity application: extremely clean, restrained, elegant and confident.

Use a warm off-white background.

Center the LabelTruth wordmark vertically and horizontally. Use a sophisticated modern sans-serif typeface with excellent typography. Under the logo, add the small tagline:

"Know what's really inside."

Add a very subtle scanning-line animation concept around or underneath the logo, representing scanning food labels. The animation should be understated and premium, not futuristic or flashy.

No food illustrations, no AI robot imagery, no gradients, no excessive decoration.

The visual hierarchy should be extremely simple: logo first, tagline second.

Design for an iPhone mobile viewport with generous whitespace and excellent visual balance.

# SCREEN 02 — Onboarding

I'd actually keep onboarding to **2–3 screens maximum**.

Don't make the user swipe through seven screens before scanning their damn cereal 😭.

### Onboarding 1

**"Scan the label."**

Visual: elegant abstract representation of a packaged food label being scanned.

### Onboarding 2

**"See beyond the marketing."**

Explain claims vs ingredients.

### Onboarding 3

**"Make informed choices."**

Health score + NOVA + personalized considerations.

---

### STITCH PROMPT — ONBOARDING

Design a premium 3-step onboarding experience for LabelTruth, a food-label transparency app.

The onboarding should feel like a combination of Apple's product onboarding and Airbnb's editorial simplicity.

Use a warm off-white background, large typography, generous whitespace and subtle visual illustrations.

SCREEN 1:  
Headline:  
"Scan the label."

Supporting text:  
"Point your camera at a barcode or ingredient label and let LabelTruth do the reading."

Visual: an elegant minimalist food package with a scanning frame moving across its barcode/ingredient label. Avoid cartoon styling.

SCREEN 2:  
Headline:  
"See beyond the marketing."

Supporting text:  
"Compare what a package claims with what is actually listed in its ingredients."

Visual: a clean split concept showing a marketing claim such as "100% Natural" beside an ingredient list. Use restrained typography and visual contrast.

SCREEN 3:  
Headline:  
"Make informed choices."

Supporting text:  
"Understand processing, additives, sugars and ingredients at a glance."

Visual: a beautifully designed health score card with a NOVA indicator and ingredient information.

Each screen should have a small progress indicator and a single primary action.

Final screen button:  
"Start scanning"

Use subtle page transitions and micro-interactions. Do not use gradients, neon colors, excessive illustrations, or generic AI imagery.


# SCREEN 03 — Login

Because your backend has authentication, you'll need this.

But make it **extremely clean**.

### Layout

```
LabelTruth

Welcome back.

Email
[                    ]

Password
[                    ]

        Log in

Don't have an account?
Create account
```

No unnecessary social-login buttons unless your backend supports them.


# SCREEN 04 — Register

Three fields:

- Email
- Password
- Dietary condition

Dietary condition shouldn't be a boring dropdown.

Use a beautiful selection control:

```
Dietary consideration

[ None ] [ Diabetic ] [ Hypertension ]
```

Maybe expandable if backend eventually supports more.

### STITCH PROMPT — AUTHENTICATION

Design two connected authentication screens for LabelTruth: Login and Create Account.

The UI should feel premium, calm and extremely polished, inspired by Apple's native settings/authentication patterns.

LOGIN SCREEN:

Top-left LabelTruth wordmark.

Large heading:  
"Welcome back."

Supporting text:  
"See what's really inside the food you buy."

Input fields:  
"Email"  
"Password"

Primary button:  
"Log in"

Secondary text:  
"Don't have an account? Create one"

CREATE ACCOUNT SCREEN:

Heading:  
"Create your LabelTruth."

Supporting text:  
"Set up your profile for more relevant food insights."

Fields:  
"Email"  
"Password"

Section:  
"Dietary consideration"

Use three elegant selectable pills:  
"None"  
"Diabetic"  
"Hypertension"

The selected state should be obvious but understated.

Primary button:  
"Create account"

Keep the interface spacious and uncluttered. Use large corner radii, subtle borders, premium typography, warm off-white background and restrained green accent.

Do not include social login, unnecessary illustrations, or excessive decorative elements.

Design both screens for iPhone mobile.



# SCREEN 05 — HOME ⭐

**This is probably the most important screen after Results.**

This needs to make the app immediately understandable to a judge.

I'd structure it:

```
Good morning, Divya

What are you eating today?

┌───────────────────────────────┐
│                               │
│       SCAN A PRODUCT          │
│                               │
│   Barcode or ingredient      │
│          label                │
│                               │
│             ⌖                 │
└───────────────────────────────┘


Recent scans

Nutella                    48
AMBER                      NOVA 4

Corn Flakes                72
GREEN                      NOVA 3
```

But the **Scan Product card should dominate**.

Maybe two small actions inside:

**Scan barcode** | **Scan label**

### Top

Avatar / profile icon.

Maybe:

> Good evening  
> What are you curious about?

That feels more human than "Welcome to LabelTruth."

### STITCH PROMPT — HOME SCREEN

Design the primary home screen for LabelTruth, a premium food-label transparency mobile app.

The screen must immediately communicate the app's core purpose and make scanning the dominant action.

Use a warm off-white background and a highly refined iOS-inspired layout.

TOP AREA:  
Small LabelTruth wordmark on the left.  
Small circular profile button on the right.

Large editorial headline:  
"What are you eating today?"

Supporting text:  
"Scan a product to see beyond the label."

PRIMARY SCAN CARD:  
Create a large premium rounded rectangular card occupying significant visual space.

Headline:  
"Scan a product"

Supporting text:  
"Barcode or ingredient label"

Inside the card, provide two elegant actions:  
"Scan barcode"  
"Scan label"

Use a minimal scanning-frame icon rather than a generic camera icon.

The scan card should have subtle depth, a thin border and very soft shadow.

BELOW:  
Section heading:  
"Recent scans"

Display 2–3 realistic recent scan rows.

Each row should show:  
Product name  
Health score  
Status badge  
NOVA level

Example:  
Nutella  
48 / 100  
AMBER  
NOVA 4

Use restrained semantic colors: green for positive status, amber for caution, red only for serious results.

Add a bottom tab bar with exactly three destinations:  
Home  
History  
Profile

The scan action should remain the visual focus.

Overall aesthetic: Apple Health meets Airbnb. Extremely clean, premium, spacious, editorial, no clutter, no gradients, no generic dashboard widgets.



# SCREEN 07 — Barcode Scanner ⭐

This should feel **really good**.

Full-screen camera.

Darkened surroundings.

Central scanning box.

Bottom:

```
Scan a barcode

Hold the barcode inside the frame

[ Upload from Photos ]
```

When detected:

```
✓ Barcode detected

Analyzing product...
```

Then automatically call:

```
GET /scan/barcode/{barcode}?user_id=1
```

No "Submit" button.

### STITCH PROMPT — BARCODE SCANNER

Design a premium full-screen barcode scanning interface for LabelTruth.

The interface should feel like a polished native iOS camera experience.

Use a dark camera preview occupying the entire screen.

Place a large rounded rectangular barcode scanning frame in the center with subtle animated scanning motion.

Outside the scanning frame, darken the camera preview slightly to create focus.

Top-left:  
Back button.

Top-center:  
"Scan barcode"

Below the scanning frame:  
"Place the barcode inside the frame"

When a barcode is detected, transition smoothly to:

"Barcode detected"

Then:  
"Analyzing product…"

The detected barcode should trigger the backend barcode endpoint automatically; do not show a manual submit button.

Include a subtle secondary action at the bottom:  
"Use a photo instead"

The UI should be extremely minimal. No excessive icons, no futuristic HUD elements, no neon scanner effects.

Use smooth animations and haptic-feedback concepts for successful detection.

The result transition should feel fast and premium.


# SCREEN 08 — Label Camera

This is your **Gemini Vision** path.

Camera UI should be slightly different from barcode.

Instead of a barcode frame:

```
Fit the ingredient list
inside the frame
```

Maybe a rectangular document frame.

Bottom:

**Take photo**

And:

**Choose from Photos**


# SCREEN 09 — Image Preview / Confirmation

This is worth having.

After taking the photo:

```
        [PHOTO]

Looks good?

Make sure the ingredient list
is readable and in focus.

Retake          Analyze
```

This is important because garbage photos = garbage OCR.
### STITCH PROMPT — LABEL SCANNER + IMAGE CONFIRMATION

Design two connected screens for LabelTruth's ingredient-label scanning flow.

SCREEN 1 — LABEL CAMERA:

Create a full-screen native iOS-style camera interface.

Dark camera preview.

Top-left back button.

Top-center:  
"Scan ingredient label"

Center a large rounded rectangular guide frame designed around the proportions of a food ingredient list.

Inside the frame, subtle helper text:  
"Fit the ingredient list inside the frame"

Bottom:  
Large circular capture button.

Secondary button:  
"Choose from Photos"

The design should encourage the user to capture a clear, well-lit ingredient list.

SCREEN 2 — PHOTO CONFIRMATION:

Display the captured image prominently with rounded corners.

Heading:  
"Looks good?"

Supporting text:  
"Make sure the ingredient list is readable and in focus."

Bottom actions:  
"Retake"  
"Analyze"

Make "Analyze" the primary action.

When Analyze is pressed, the app uploads the image to the backend image scanning endpoint.

The visual design should be premium, minimal and calm. Avoid excessive camera UI elements.


# SCREEN 10 — ANALYZING / LOADING ⭐

This screen is important because Gemini isn't necessarily instant.

**DO NOT show a boring spinner.**

Instead make the app feel like it's actually doing something.

Something like:
```
        [ animated scanning mark ]

Reading the label

Identifying ingredients
Checking additives
Analyzing processing
Checking marketing claims

            72%
```

But don't fake exact progress if the backend doesn't provide progress.

So visually animate the stages sequentially without claiming real percentages.

### STITCH PROMPT — ANALYSIS LOADING SCREEN

Design a premium analysis/loading screen for LabelTruth.

The user has just scanned a food barcode or ingredient label.

Use a warm off-white background with a centered animated scanning motif.

Large heading:  
"Reading the label"

Below it, show a vertical sequence of analysis stages:

✓ Reading ingredients  
✓ Checking additives  
✓ Evaluating processing  
○ Reviewing marketing claims

Animate the active stage subtly.

Do NOT display a fake numerical percentage because the backend does not provide actual progress information.

Use elegant micro-animations such as text transitions, subtle scanning movement and checkmark appearance.

The screen should communicate that LabelTruth is actively analyzing the product without feeling technical or cluttered.

After analysis completes, transition smoothly into the results screen.

Apple-level restraint. No spinner-only loading screen.


# SCREEN 11 — RESULTS ⭐⭐⭐

THIS IS THE MONEY SCREEN.

This is where the judges go:

> "Oh shit, that's actually useful."

You need **one unified results design** that works for both barcode and image scans.

The information changes slightly depending on scan type.

---

## Top of Results

```
Nutella

Ferrero

                         NOVA
                          4
                    Ultra-processed
```

Then:

# 48

**Health score**

Maybe a circular score visualization.

Don't make it look like a credit score.

A beautiful large number is enough.

```
48
Health score
```

Then:

**AMBER**

---

## Personalized warning

If present:

```
Personalized consideration

This product may be relevant to
your selected dietary profile.
```

Again, avoid making the UI sound like a medical diagnosis.

---

## Processing

```
Processing

NOVA 4

Ultra-processed
```

Use a horizontal 1–4 indicator.

---

## Ingredients

```
Ingredients

Sugar
Palm Oil
Hazelnuts
Skimmed Milk Powder
...
```

Maybe "View full ingredient list."

---

## Additives

```
Additives detected

E102
Food colouring

[Learn more]
```

For every returned:

```
{
 "name": "...",
 "risk": "...",
 "note": "..."
}
```

Display the name, risk, and note.

---

## Claims

For image scan:

```
Marketing claims

"100% Natural Whole Grain"

⚠ Review ingredients
```

This is **your differentiator**.

---

## Verdict

At bottom:

```
LabelTruth verdict

[verdict_summary]
```
### STITCH PROMPT — PRODUCT RESULTS SCREEN

Design the flagship results screen for LabelTruth.

This is the most important screen in the application and should feel exceptionally polished, premium and immediately understandable.

The screen displays the result of either a barcode scan or ingredient-label scan.

TOP:  
Back button on the left.  
Small share/save icon on the right.

PRODUCT HEADER:  
Large product name.  
Small brand/product-type text underneath when available.

HEALTH SCORE:  
Create a large, elegant score section.

Example:  
"48"  
"Health score"

Display the score prominently from 0–100.

Below it show the semantic status:  
"AMBER"

Use green, amber or red only as semantic accents. Keep the majority of the interface neutral.

PERSONALIZED CONSIDERATION:  
If personalized_warning exists, display a beautifully designed subtle warning card.

Use the title:  
"Personalized consideration"

Display the returned warning text beneath it.

Do not make this look like a medical diagnosis or emergency alert.

PROCESSING CARD:  
Show:

"Processing"  
"NOVA 4"  
"Ultra-processed"

Create an elegant horizontal NOVA 1–4 indicator with level 4 emphasized.

INGREDIENTS SECTION:  
Title:  
"Ingredients"

Display the ingredient list in a highly readable format.

For barcode results, use the returned ingredients string.  
For image results, use extracted_ingredients.

Allow long ingredient lists to expand/collapse.

ADDITIVES SECTION:  
If flagged additives or E-numbers exist, show:

"Additives detected"

Each additive should be displayed as a compact card containing:  
Name  
Risk  
Note

Do not automatically imply that an additive is dangerous merely because it is present.

For image results, also show detected E-numbers.

MARKETING CLAIMS SECTION:  
For image scans, if greenwashing_claims_detected exists, display:

"Marketing claims"

Show each detected claim in quotation marks.

Visually distinguish marketing claims from ingredient evidence.

Add a small contextual label such as:  
"Compare with ingredients"

VERDICT SECTION:  
At the bottom display:

"LabelTruth verdict"

Then show the backend's verdict_summary in a highly readable editorial text block.

The screen should be vertically scrollable.

Use large section spacing, 20–28px rounded cards, thin borders, extremely subtle shadows and sophisticated typography.

The experience should feel like Apple Health meets Airbnb product detail design.

Avoid dashboard clutter. Avoid giant gradients. Avoid excessive icons. Make the health score, product identity and ingredient reality the visual hierarchy.

Design both barcode and image scan results using the same visual system.


# SCREEN 13 — Marketing Claim Detail

This is actually one of your strongest UX ideas.

Tap:

> "100% Natural Whole Grain"

Then:

```
Marketing claim

"100% Natural Whole Grain"

LabelTruth found ingredients
that deserve a closer look.

Detected:
Maltodextrin
Sugar
...

What we found
```

Again, don't state "this is illegal greenwashing" unless you have evidence.

Call it:

**"Claim review"**

not:

**"COMPANY LIED TO YOU 💀"**



# SCREEN 14 — History ⭐

This is powered directly by:

```
GET /user/history/{user_id}
```

Your backend gives:

```
{
  "id": 1,
  "product_name": "Nutella",
  "nova_level": 4,
  "verdict": "Score: 48/100 - AMBER"
}
```

So your UI can be:

```
History

Your recent scans

Today

Nutella
NOVA 4                 48 AMBER

Yesterday

Corn Flakes
NOVA 3                 72 GREEN
```

Very Apple Settings / Airbnb booking history style.
### STITCH PROMPT — HISTORY SCREEN

Design the LabelTruth scan history screen.

Use the same premium iOS-inspired visual language as the rest of the application.

Top:  
Large heading:  
"History"

Small supporting text:  
"Your recent product scans"

Organize scans chronologically with subtle date labels such as:  
"Today"  
"Yesterday"  
"Earlier"

Each history row should contain:

Product name  
NOVA level  
Health score  
Status

Example:

Nutella  
NOVA 4  
48 / 100  
AMBER

Make each row tappable with a subtle chevron.

Use generous vertical spacing and thin separators or soft rounded cards.

Do not turn this into a spreadsheet or dense data table.

Include a clean empty state if there are no scans:

"No scans yet"

"Scan your first product to start building your history."

Primary action:  
"Scan a product"

The bottom navigation should contain:  
Home  
History  
Profile

The visual style should resemble a premium Apple settings/history interface rather than a generic SaaS dashboard.


# SCREEN 15 — History Product Detail

When user taps a history entry:

```
Nutella

48 / 100
AMBER

NOVA 4

Score: 48/100 - AMBER
```

But there's a limitation:

Your history endpoint only returns the compact history record.

So if you want full product details from history, you either:

1. Store the complete scan response locally, or
2. Add a backend endpoint for retrieving a scan by ID.

For MVP, I'd just make history entries open the **same result screen if you cache the scan response locally**.


# SCREEN 16 — Profile

Keep it incredibly simple.

```
Profile

D

Your account

user@email.com

Dietary consideration

Diabetic

────────────────

Preferences

Dietary consideration >
Scan history >

────────────────

Account

Log out
```

No unnecessary gamification.


# SCREEN 17 — Edit Dietary Condition

This corresponds to:

```
PUT /user/profile/{user_id}
```

Screen:

```
Dietary consideration

Choose what LabelTruth
should keep in mind.

○ None

○ Diabetic

○ Hypertension

             Save
```

I'd make this feel like Apple Health settings.
### STITCH PROMPT — PROFILE + DIETARY SETTINGS

Design two connected screens for LabelTruth: Profile and Dietary Consideration.

PROFILE SCREEN:

Large heading:  
"Profile"

Show a simple circular avatar with the user's initial.

Display:  
Email address

Section:  
"Dietary consideration"

Show the current selection, for example:  
"Diabetic"

Below, create a settings-style list:

"Dietary consideration"  
"Scan history"

Then an Account section containing:  
"Log out"

Use native iOS-style list rows with subtle separators, rounded sections and generous whitespace.

DIETARY CONSIDERATION SCREEN:

Large heading:  
"Dietary consideration"

Supporting text:  
"Choose what LabelTruth should keep in mind when presenting personalized insights."

Show three large selectable options:

None  
Diabetic  
Hypertension

Use a refined selected state with a checkmark.

Bottom primary button:  
"Save"

The interface should be calm and trustworthy. Avoid medical-looking red warning aesthetics. This is a preference setting, not a diagnosis screen.

Use the same typography, spacing, corner radius and navigation patterns as the rest of LabelTruth.


# SCREEN 18 — Empty/Error States

You absolutely need these.

Hackathon demos **will break**.

Have designs for:

### Product not found

```
We couldn't find this product.

Try scanning the barcode again
or scan the ingredient label instead.

[Scan label]
```

### Bad image

```
We couldn't read the label.

Try taking a clearer photo
with the ingredients in focus.

[Retake photo]
```

### Server error

```
Something went wrong.

LabelTruth couldn't analyze this
product right now.

[Try again]
```

### No internet

```
You're offline.

Check your connection and try again.
```

These make the app feel _real_.
### STITCH PROMPT — ERROR AND EMPTY STATES

Design a complete set of elegant error and empty states for LabelTruth.

Create four states using the same premium visual system.

STATE 1 — PRODUCT NOT FOUND:

Heading:  
"We couldn't find this product."

Supporting text:  
"Try scanning the barcode again or scan the ingredient label instead."

Primary button:  
"Scan label"

Secondary action:  
"Try again"

STATE 2 — LABEL UNREADABLE:

Heading:  
"We couldn't read the label."

Supporting text:  
"Try taking a clearer photo with the ingredients in focus."

Primary button:  
"Retake photo"

STATE 3 — SERVER ERROR:

Heading:  
"Something went wrong."

Supporting text:  
"LabelTruth couldn't analyze this product right now."

Primary button:  
"Try again"

STATE 4 — EMPTY HISTORY:

Heading:  
"No scans yet"

Supporting text:  
"Scan your first product to start building your history."

Primary button:  
"Scan a product"

Keep illustrations extremely minimal. Prefer abstract line icons or subtle geometric scanning motifs instead of cartoon illustrations.

Use large typography, generous whitespace, warm off-white background and understated buttons.

The states should feel like carefully designed native iOS experiences rather than error pages.

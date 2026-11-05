# HHaven Shopify Theme: Setup Guide

This theme is Shopify's free Dawn theme (version 16.1.1) with the HHaven brand added: your colors, fonts, logos, photos, custom sections, and pages already filled in with your copy.

## What's included

| Part | What it is |
|---|---|
| Colors | 5 color schemes from your brand sheet: Cream, Oat, Cacao, Moss, Mist |
| Fonts | Bogart, Optima, Royale Victoria, shown with free stand-ins until web licenses are added |
| Logos | All logo files, recolored. The Apothecary logo shows in the header until you upload one |
| Photos | Your photos are bundled, so every page looks right on day one. Swap any of them in the editor |
| Custom sections | Photo and text, Quote, Numbered cards, Columns, Trust strip, Gatherings, Membership, Story text |
| Pages ready to go | Home, Our Story, The Club, Gatherings, Learn, Sourcing |

## Step by step

### 1. Upload the theme
1. In Shopify admin, go to **Online Store > Themes**.
2. Click **Add theme > Upload zip file** and choose `hhaven-theme.zip`.
3. Click **Customize** to preview before you publish.

### 2. Create the pages
Go to **Online Store > Pages** and add each page below. On the right, set **Theme template** to the one listed.

| Page title | Handle (URL) | Theme template |
|---|---|---|
| Our Story | our-story | page.story |
| The Club | the-club | page.club |
| Gatherings | gatherings | page.gatherings |
| Learn | learn | page.learn |
| Sourcing | sourcing | page.sourcing |
| Contact | contact | page.contact |
| Wholesale and Facilitators | wholesale | page |
| Shipping, Returns, and Policies | policies | page |

The page body can stay empty for the designed pages. All the content lives in the template.

### 3. Add products
- **Cusco Valley Ceremonial Cacao** and **Atlantic Forest Ceremonial Cacao**: variants ½ lb ($35) and 1 lb ($65).
- **The Tasting Set**: $65.
- **Gathering tickets**: one product per gathering. Put them in a collection with the handle `gatherings`, so the "Save my spot" buttons work.
- Paste the descriptions, prep steps, and storage notes from the mockup.

### 4. Menus
**Online Store > Navigation > Main menu:** Shop, Learn, Sourcing, Gatherings, The Club, Our Story, Journal.
**Footer menu:** FAQ, Contact, Wholesale, Policies.

### 5. Journal
Rename the default blog to **Journal** and post the bloom article first. The homepage shows your latest three posts.

### 6. Membership app
Install a membership app (compare Appstle, Seal, or Shopify Subscriptions plus a tagging app). Create the **Founding Member** product at $45/month and $450/year. Then, on The Club page, open the **HHaven membership** section and paste the product link into **Button link**.

### 7. The Founding List
This form needs no app. Each signup becomes a Shopify customer with tags such as:
`founding-list`, `zip-68022`, `interest-sauna-and-recovery`, `interest-the-cafe`

To count them for investors, go to **Customers**, filter by tag, and export.

### 8. Edit events
On the Gatherings page and the homepage, each event is a block in the **HHaven gatherings** section. Click it to change the date, title, details, and ticket link. Add or delete blocks as events come and go.

### 9. Fonts (when licensed)
Buy web licenses for Bogart, Optima, and Royale Victoria. Upload the `.woff2` files under **Edit code > Assets**. Then open `assets/hhaven.css` and follow the note at the top.

### 10. Before you launch
- Board and legal sign-off on: the Learn page, the gathering safety note, the product "Before you try it" note, and the footer disclaimer.
- Swap placeholder events and add real reviews.
- Set up Shopify Payments, Shopify Tax, shipping rates, and policies.
- Connect your domain. Turn on 2-step login for every staff account.
- Submit your sitemap in Google Search Console.

## Working on the theme with Claude Code
The theme is a git repository. Use these commands with the Shopify CLI:

```bash
shopify theme dev --store your-store.myshopify.com
```

```bash
shopify theme check
```

```bash
shopify theme push --unpublished
```

## Not tested yet
I couldn't preview the theme inside a live Shopify store from this session, because that needs your store login. The code passed Shopify's own theme check with no errors. Do the first run with `shopify theme dev` or as an unpublished theme, and send me screenshots of anything that looks off.

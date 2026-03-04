# ChipMonkeys Off Grid — Master TODO

**One list. Keep punching.**

Last updated: 2026-03-04

---

## STORE & FUNNEL

- [ ] Create `offgrid_leads` table in Supabase (email, name, source, products_interested, created_at)
- [ ] Set up Stripe products in dashboard (so orders show nice product names, not just inline price_data)
- [ ] Add product images to store page (photograph each kit, hero shots)
- [ ] Set up shipping flow — label printing, tracking numbers, notification emails
- [ ] Add shipping cost calculation to checkout (flat rate? weight-based? free over $99?)
- [ ] Build inventory tracking (even simple — just a count per product so you don't oversell)
- [ ] Write the nurture email sequence (3-4 emails after lead magnet):
  - [ ] Email 2 (Day 2): Ask about their situation — homesteading? prepping? curious? Ask about kids/family
  - [ ] Email 3 (Day 4): Share a build story / failure story — keep it real, show the process
  - [ ] Email 4 (Day 7): Soft pitch the kit — "if you want to skip the prep work"
- [ ] Wire up email automation in MBM (trigger: offgrid_lead tag → sequence)
- [ ] Add order confirmation email (post-purchase, from Brandon, personal, not transactional-looking)
- [ ] Build order fulfillment tracking page in admin (list of orders to ship)
- [ ] Add "prototype stage" badge/banner more prominently on store
- [ ] Set up abandoned cart recovery (email if they start checkout but don't finish)

## OTOs & UPSELLS (Brunson Value Ladder)

- [ ] Set up GoHighLevel membership area / Skool-style community
- [ ] Build OTO #1 page ($97 Founding Member Course) — page is built, needs GHL integration
- [ ] Record first 3-5 course modules (can be YouTube episode cuts, doesn't need to be new content)
- [ ] Build OTO #2 / downsell page ($47 just the course, no physical upgrade)
- [ ] Wire up OTO flow: checkout → OTO #1 → (decline) → downsell → thank you
- [ ] Build high-ticket application page ($997+ consulting)
- [ ] Build mastermind application page ($100k — for entrepreneurs who want to manufacture)
- [ ] Create Calendly or booking link for 1-on-1 consultations
- [ ] Write Russell Brunson funnel scripts for each OTO (or pull from Funnel Scripts account)

## YOUTUBE

- [ ] Create YouTube channel (ChipMonkeys Off Grid)
- [ ] Film Episode 1: "I'm Building a Battery From Hardware Store Materials" (hook + overview)
- [ ] Film Episode 2: "Making the Electrode — Popcorn Ball Method" (torch demo)
- [ ] Film Episode 3: "Making the Electrolyte — Scrap Iron + Acid" (dissolution time lapse)
- [ ] Film Episode 4: "Making the Membrane — Rowow Method" (brine float + casting)
- [ ] Film Episode 5: "The SEM Cell — Making Acid From Salt" (chlorine safety!)
- [ ] Film Episode 6: "Assembling the First Cell" (box + MEA + charcoal fill)
- [ ] Film Episode 7: "First Light — 4-Cell Stack Powers a Phone" (the money shot)
- [ ] Film Episode 8: "Community Electrode Challenge — Submit Your Design"
- [ ] Create channel art, thumbnails template, intro/outro
- [ ] Set up end screens and cards linking to store
- [ ] Write video descriptions with affiliate links and store links

## GITHUB & DOCS

- [ ] Create GitHub organization (ChipMonkeysOffGrid) — needs web UI, move repo from Breed2085
- [ ] Add STL files for 50mm test cell to flow-battery/stl/
- [ ] Add Fusion 360 source files to flow-battery/designs/
- [ ] Create parametric Fusion 360 model (change one dimension → everything scales)
- [ ] Design and add STL for ED water purification stack (double diode film holder)
- [ ] Add wiring diagram for 4-cell stack
- [ ] Add plumbing diagram for manifold connections
- [ ] Create printable quick-reference build card (PDF, ships with kits)
- [ ] Add community electrode designs README template
- [ ] Set up GitHub Discussions for community Q&A

## CELL DESIGN & TESTING

- [ ] Print first 50mm test cell boxes on VzBot 400
- [ ] Test PVC cement bond to ASA — pull test, leak test
- [ ] Make first batch of Rowow membranes (diode films)
- [ ] Make first popcorn ball electrodes — dial in torch technique
- [ ] Assemble first complete cell — test for leaks
- [ ] Make electrolyte batch (muriatic acid + scrap iron)
- [ ] First charge/discharge cycle — measure OCV, load voltage, current
- [ ] Test 4-cell stack — power a pump + charge a phone (Phase 1 target)
- [ ] Measure round-trip efficiency
- [ ] Long-term cycling test (100+ cycles, track capacity)
- [ ] Scale to 300mm production cell design
- [ ] Test pyrolyzed 3D printed electrode (sugar-soaked PLA, campfire kiln)

## EMAIL MARKETING

- [ ] Set up GoHighLevel for off-grid funnel (separate from MBM paint business)
- [ ] Create lead magnet delivery automation in GHL
- [ ] Create post-purchase sequence in GHL
- [ ] Create abandoned cart sequence
- [ ] Create re-engagement sequence (30-day no-open)
- [ ] Set up tagging: lead, buyer, repeat-buyer, high-value, course-member
- [ ] Integrate GHL webhook with MBM offgrid-lead API endpoint
- [ ] Set up weekly newsletter / build update email (from Brandon, personal voice)

## BUSINESS & LEGAL

- [ ] Route all off-grid revenue through ChipMonkeys Inc. C-corp
- [ ] Set up Amazon Associates payment through C-corp
- [ ] Check shipping regulations for electrolyte concentrate (HCl, hazmat ground)
- [ ] Get product liability insurance for kit sales (prototype stage disclaimer isn't enough long-term)
- [ ] Trademark "ChipMonkeys Off Grid" if serious about the brand
- [ ] Set up bookkeeping for kit costs vs revenue (even a spreadsheet to start)
- [ ] Research state sales tax requirements for Tennessee (moving there)

## COLLABORATIONS

- [ ] Reach out to Rowow — credit given, collaborate on membrane improvements
- [ ] Reach out to Night Hawk in Light — intumescent electrode, Starlite connection
- [ ] Reach out to Cody's Lab — pyrolysis expertise, carbonized electrode testing
- [ ] Reach out to FBRC — open-source flow battery community, cross-promote
- [ ] Guest on relevant podcasts (homesteading, off-grid, maker, DIY energy)

## WATER PURIFICATION (ED System)

- [ ] Grind SBA (anion) resin for anion diode films
- [ ] Make first anion diode film (AEM) — test ionic conductivity
- [ ] Design and print double diode film holder STL
- [ ] Design and print ED end caps with graphite electrode pocket
- [ ] Assemble 3-cell-pair test stack
- [ ] Test with TDS meter — measure ion removal rate
- [ ] Test EDR polarity reversal — does scale dissolve?
- [ ] Add carbon filter stage
- [ ] Add UV sterilization stage
- [ ] Test complete 3-stage system on well water

## SEM CELL (Salt Electro Mining)

- [ ] Build first SEM cell (2-gallon HDPE buckets + cation diode film)
- [ ] Source graphite electrodes
- [ ] Run first batch — measure HCl production rate
- [ ] Test fast method (iron in anode chamber)
- [ ] Collect and test NaOH byproduct — measure concentration
- [ ] Calculate economics (salt + electricity cost vs lye value)

## WEBSITE

- [ ] Design chipmonkeysinc.com/offgrid landing page (separate from MBM store?)
- [ ] Or redirect chipmonkeysinc.com/offgrid → monkeybusinessmanager.com/offgrid
- [ ] Add SSL and custom domain if needed
- [ ] Set up Google Analytics / Plausible on the offgrid funnel pages
- [ ] Set up Facebook Pixel / Meta conversion tracking for ads (later)

---

*Check one off. Add two more. That's how we win.*

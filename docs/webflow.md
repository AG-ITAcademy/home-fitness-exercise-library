# Joy2Move Exercise Library for Webflow

Add editable exercise demonstration cards to your Webflow pages. The app is free, in English, and requires no separate Joy2Move account.

## Installation and setup

Install Joy2Move Exercise Library on your Webflow site from its Marketplace listing once approved. In Webflow Designer, open Apps, choose Joy2Move Exercise Library, and select Launch App. During review, use the app installation supplied through Webflow's review process.

## Find and insert an exercise

1. Search by exercise name or alias, such as squat, wall sit or RDL. Select equipment if needed. An empty search browses the catalog.
2. Select a result and press Play to preview its 15-second demonstration.
3. Select Body, a section or a div in Designer, then choose Insert exercise card.
4. Edit the inserted heading, equipment label and styles using Webflow's normal controls.
5. Publish your page normally and test the card's Play button on the published page.

## Playback

The card loads a static player included in the app's versioned package. YouTube loads only after an explicit Play click, at the curated start timestamp, for a 15-second segment. Your browser may require a second Play click. If playback is blocked, the exercise-page link remains available.

## Remove a card

In Navigator, select the card's top-level `j2m-exercise-card` section and delete it. Undo and Redo apply to individual Webflow edits. Uninstalling the app preserves cards already added; remove unwanted sections yourself.

## Troubleshooting

- Insertion requires Design mode on the main branch and primary locale.
- Select a container instead of text, a link or a form.
- If there are no results, try a shorter name or another equipment filter.
- The catalog is bundled with each app version. Newly added exercises require an app update.
- Video playback depends on YouTube availability and the visitor's browser permissions.

## Privacy, permissions and support

Search and selection run locally. No user-entered search terms or selected exercise identifiers are sent to a remote lookup service. The app does not use the Data API, read your account or CMS, collect visitor details or credentials, or add site-wide scripts. It modifies the selected page only when you insert a card. Published cards contact YouTube after Play. Website owners should include the playback service in their own privacy disclosures.

[Privacy policy](https://www.joy2move.net/privacy-policy) · [Terms](https://www.joy2move.net/terms) · [Exercise library](https://www.joy2move.net/exercises)

Support: support@joy2move.net. Include the exercise name and a description of the issue, without passwords, private project data or medical information.

The documentation is maintained by GLOBAL PERSPECTIVE SRL. The exercise catalog, videos and Joy2Move application are not licensed by this repository's package license.

=== ContentGem – AI SEO & Topical Authority ===
Contributors: contentgem
Tags: seo, ai, topical authority, keyword clustering, content gaps
Requires at least: 6.2
Tested up to: 6.7
Requires PHP: 7.4
Stable tag: 5.0.9
License: GPL-2.0-or-later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

AI-powered topical authority analysis, keyword clustering, content gap detection, and competitor research for WordPress.

== Description ==

ContentGem helps content teams and SEO professionals build topical authority faster. It analyses your existing content, identifies gaps, clusters keywords into structured topic maps, and generates AI-assisted draft outlines — all from within the WordPress admin.

**Key features:**

* **Topical Authority Dashboard** – visualise your site's coverage of any topic.
* **Keyword Clustering** – group keywords into semantic clusters automatically.
* **Content Gap Detection** – find what your competitors cover that you don't.
* **Google Search Console Integration** – import real performance data (requires GSC authorisation).
* **AI Assistant** – generate draft outlines and content suggestions (requires an Anthropic Claude or OpenAI API key).
* **Competitor Analysis** – analyse competitor URLs you supply to discover missing angles.
* **Internal Linking Scanner** – surface orphaned posts and linking opportunities.
* **IndexNow Integration** – ping search engines on publish.

**External services used:**

ContentGem connects to the following third-party services when you configure and use the relevant features:

* **Anthropic Claude API** (`api.anthropic.com`) – used for AI draft generation and content analysis. Requires an API key you provide. [Terms of Use](https://www.anthropic.com/legal/consumer-terms) | [Privacy Policy](https://www.anthropic.com/legal/privacy)
* **OpenAI API** (`api.openai.com`) – optional alternative AI provider. Requires an API key you provide. [Terms of Use](https://openai.com/policies/terms-of-use) | [Privacy Policy](https://openai.com/policies/privacy-policy)
* **Google Search Console API** (`searchconsole.googleapis.com`, `oauth2.googleapis.com`) – used to import search performance data. Requires explicit OAuth authorisation by the site owner. [Terms of Service](https://developers.google.com/terms) | [Privacy Policy](https://policies.google.com/privacy)
* **IndexNow API** (`api.indexnow.org`) – used to notify search engines of new or updated content. Enabled only after opt-in in settings. [Documentation](https://www.indexnow.org/)
* **Freemius** – used for plugin licensing and payments. [Privacy Policy](https://freemius.com/privacy/)

No data is sent to any external service without explicit configuration and, where applicable, user authorisation. The plugin does not collect analytics or usage data on your behalf.

== Installation ==

1. Upload the `contentgem` folder to `/wp-content/plugins/`, or install via **Plugins > Add New > Upload Plugin** in WordPress admin.
2. Activate the plugin through the **Plugins** menu.
3. Navigate to **ContentGem** in the WordPress admin sidebar to start the onboarding.
4. Add your AI API key (Anthropic Claude or OpenAI) in **ContentGem > Settings** to enable AI features.
5. Optionally connect Google Search Console via **ContentGem > Settings > GSC** for performance data.

== Frequently Asked Questions ==

= Does ContentGem require an API key? =

The free tier works without an API key for basic clustering and content gap views. AI-assisted features (draft generation, AI analysis) require an Anthropic Claude or OpenAI API key, which you provide in Settings. ContentGem never stores your key beyond your own WordPress database.

= What data is sent to external services? =

Only data you actively send is transmitted. For AI features: the text or keywords you submit for analysis. For GSC: the plugin requests your own Search Console data using the OAuth token you authorise. See the Description tab for links to each service's privacy policy.

= Is the plugin compatible with my caching plugin? =

Yes. ContentGem automatically sets cache-bypass headers for its admin pages and REST API endpoints, so caching plugins will not interfere.

= Can I use ContentGem on multiple sites? =

The Free plan supports one site. The Agency plan supports multiple sites. See ContentGem > Settings for licensing options.

= Where is the source code? =

ContentGem is open-source compatible. The React frontend source is maintained at [https://github.com/contentgem/contentgem-plugin](https://github.com/contentgem/contentgem-plugin) and a link to build instructions is included in the plugin's readme on GitHub.

== Screenshots ==

1. Topical Authority Dashboard showing cluster coverage.
2. Content Gap analysis between your site and a competitor.
3. AI Assistant generating a draft outline from a cluster.
4. Google Search Console data integrated into cluster view.

== Changelog ==

= 5.0.9 =
* Added IndexNow integration for instant search engine pinging.
* Improved AI Assistant rendering performance.
* Fixed GSC OAuth property-loading issue on some server configurations.
* Added token optimisation for Claude and OpenAI API calls.

= 5.0.0 =
* Major rewrite: service-based PHP architecture.
* React-powered frontend dashboard.
* Freemius licensing integration.
* Content gap engine v2.

= 1.8.0 =
* Competitor analysis module.
* Internal linking scanner.

= 1.7.2 =
* Initial stable release with admin menu and dashboard.

== Upgrade Notice ==

= 5.0.9 =
Recommended update. Fixes GSC OAuth issues and improves AI performance.

== Privacy Policy ==

ContentGem does not collect, store, or transmit any personal data on its own behalf. All connections to external APIs (Claude, OpenAI, Google) are made using credentials you supply and data you choose to send. Please review the privacy policies of each external service listed in the Description tab.

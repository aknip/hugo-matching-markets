# hugo102
first hugo test for netlify

check on https://hugo102.netlify.com/



Start Hugo Dev-Server (intern/extern)
- **Intern** (localhost, Server and Browser on the same system):
    - hugo server -D
    - in webbrowser: http://localhost:1313/
- **Extern** (IP or Domainname, server externally and browser local)
    - hugo server -D --bind=100.68.48.184 --baseURL=http://100.68.48.184:1313
    - Im Webbrowser: http://100.68.48.184:1313


Create Post
- hugo server -D
- In second terminal: hugo new posts/my-first-post.md
- Im browser: http://localhost:1313/



## Configuration and Theme settings

Multilanguage:
- deleted folder 'zh'
- deactivated language switch in config.toml: [menu] [[menu.main]] identifier = "zh" (line 60)
- added themes/LoveIt/i18n/de.toml
- set default language to 'de' in config.toml

config.toml
- [params] dateFormatToUse = "02.01.2006"
- [params] avatar => deleted, no avatar pic on homepage

themes/LoveIt/i18n/de.toml
- deleted text "published on" in post list (line 60)

Theme modifications:
- added custom styles in "fakplus.scss" in themes/LoveIt/assets/css/style.scss
- Dark Theme als default: <body class="dark-theme"> (themes/LoveIt/layouts/_default/baseof.html, line 12)
- Post list (themes/LoveIt/layouts/_default/summary.html)
-- Removed author from list (line 21)
- Footer (themes/LoveIt/layouts/partials/footer.html)
-- Changed copyright line (line 3 ff.)
- Pinned posts (themes/LoveIt/layouts/partials/home/profile.html) line 32 ff.

# hugo102
first hugo test for netlify

check on https://hugo102.netlify.com/


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
- Dark Theme als default: <body class="dark-theme"> (themes/LoveIt/layouts/_default/baseof.html, line 12)
- Post list (themes/LoveIt/layouts/_default/summary.html)
-- Removed author from list (line 21)
- Footer (themes/LoveIt/layouts/partials/footer.html)
-- Changed copyright line (line 3 ff.)
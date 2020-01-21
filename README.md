# hugo102
first hugo test for netlify

check on https://hugo102.netlify.com/


Multilanguage:
- deleted folder 'zh'
- deactivated language switch in config.toml: [menu] [[menu.main]] identifier = "zh" (line 60)

config.toml
- [params] dateFormatToUse = "02.01.2006"

themes/LoveIt/i18n/en.toml
- deleted text "published on" in post list (line 60)

Theme modifications:
- Post list (themes/LoveIt/layouts/_default/summary.html)
-- Removed author from list (line 21)
- Footer (themes/LoveIt/layouts/partials/footer.html)
-- Changed copyright line (line 3 ff.)
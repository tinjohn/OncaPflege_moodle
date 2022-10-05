# OncaPflege_moodle
A collection of files and a documentation for [Onlinecampus Pflege](https://www.onlinecampus-pflege.de).

## Moodle
[Version 4.0.4]
[github](https://github.com/moodle/moodle/tree/MOODLE_400_STABLE)
[moodle.org]()

## Appearance
- Logo : [Onlinecampus Pflege Logo](./appearance/Logos/OncaPflegeLogo_653x200hres.png)
- Compact logo : [Onlinecampus Pflege Pfeil](./appearance/Logos/OCP_Pfeil_d72733_72dpi_200x200px.png)

## Theme
learnR
- [github](https://github.com/dbnschools/moodle-theme_learnr.git)
- [moodle.org](https://moodle.org/plugins/theme_learnr)

### preset
learnR default with some adjustments for [OCP](./presets/OCP%20LearnR.scss)

### layout
- coursetilestyle : Tile Style Four w/course summary
- sectionstyle : LearnR Default Style
- fullwidthpage: No
- showcourseindexnav: No
- showblockdrawer: Yes
- showlatestcourses: Yes
- showprogressbar: Yes
- activitynavdisplay: Turn top location on
- showpageimage: Yes

### Icon Navigation / Navigationssymbol
- createbuttontext : Kurs anlegen  

### Custom image settings
- loginimage : [Onlinecampus Pflege backgroundgraphic](./custom_image_settings/OncaPflegeMoodle_Loginbg72.png)
- headerdefaultimage : [Onlinecampus Pflege backgroundgraphic](./custom_image_settings/headerbg_OncaPflege_kurslogos72.png)


## Plugins
- mod_MotBot
  - [github](https://github.com/ild-thl/motbot)
- moodle-block_lpprogressx
  - [github](https://github.com/tinjohn/moodle-block_lpprogressx)
- moodle-local_lpautocomplete
  - [gitlab bugfix version until fixed in official version](https://gitlab.com/tinjohn/moodle-local_lpautocompletedeb)
  - [gitlab](https://gitlab.com/adapta/moodle-local_lpautocomplete)
  - [moodle.org](https://moodle.org/plugins/local_lpautocomplete)
- moodle-format_buttonsx (in course/format)
  - [github](https://github.com/tinjohn/moodle-format_buttonsx)

## Plugins for further developements
- moodle-local_metadata (will be used for alternate content)
- moodle-atto_snippets (will be used for alternate content) (in lib/editor/atto/plugins)
- moodle-block_game (option for gamification)
- moodle-block_xp (option for gamification)

## Plugins for former developements
- moodle-format_collapsibletopics (might not be used further)
- moodle-format_multitopic (might not be used further)
- moodle-atto_templates4u (might not be used further)
- moodle-atto_wordcount (might not be used further)
- moodle-mod_hvp (might not be used further)

## Configuration
  e-mail base authentification
  SMTP

## Course Configuration
  self enrolement

## Upgrade notes
* 3.11 -> 4.0.3
- plugin qformat_examview missing [discussion](https://moodle.org/mod/forum/discuss.php?d=435784)
-

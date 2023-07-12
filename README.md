# OncaPflege_moodle
A collection of files and a documentation for [Onlinecampus Pflege](https://www.onlinecampus-pflege.de).

## Moodle
[Version 4.1+]
- [github](https://github.com/moodle/moodle.git) use branch MOODLE_STABLE_401
- [moodle.org](https://moodle.org)

## Appearance
- Logo : [Onlinecampus Pflege Logo](./appearance/Logos/OncaPflegeLogo_653x200hres.png)
- Compact logo : [Onlinecampus Pflege Pfeil](./appearance/Logos/OCP_Pfeil_d72733_72dpi_200x200px.png)

## Theme
learnR (version v4.2.r7)
- [github](https://github.com/dbnschools/moodle-theme_learnr.git)
- [moodle.org](https://moodle.org/plugins/theme_learnr)

### preset
- learnR default with some adjustments for [OCP](./presets)
- add icons to pix directory of the theme, necessary for some highlighting layouts  


### configuration
- Feel -> Navigation -> hidenodesprimarynavigation (Home, Dashboard) 
  - removes multiple ways for navigation  
- Feel -> Blocks -> blockregionsforfrontpage -> Content (lower)
  - add ISymetaselect block at frontpage 
  - change capability to Allow for theme/learnr:viewregioncontentlower for guests (Administration -> Define roles -> 'Guest' -> Edit)
- Look -> Page
  - coursecontentmaxwidth 82%
  - mediumcontentmaxwidth 95%
- Look -> Generell Settings
  - coursetilestyle : Tile Style Four w/course summary
  - sectionstyle : LearnR Default Style
  - add the preset file from presets (OCP_learnR_YYYYMMDD.scss)
- Look -> SCSS
  - raw intial SCSS: copy from presets
  - raw SCSS: copy from presets
- Look -> Branding
  - logo: siehe [logos](./appearance/Logos/)
  - logocompact: [logos](./appearance/Logos/)
  - favicon: [logos](./appearance/Logos/)
  - brandcolor: #7A000C
  - bodybg: #d9d9d9
  - bgdark: #7A000C
  - navbarcolor: Primary color navbar with light font color
- Look -> Login Page
    - loginbackgroundimage: [custom_image_settings](./appearance/Logos/custom_image_settings)
    - loginformtransparency: yes
- Look -> Course
    - showprogressbar: yes

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

## for front pagelayout
- add [fpimgs folder](./front_page/) to pix directory of moodles root dir, necessary for front page images
- edit front page and add [html code](./front_page/html.html)

## for Dashboard Menu
- set custommenuitems (Website administration -> Appearance -> Theme Settings)
  - Alle Nuggets|/my/index.php#ildmetaselect_form_anchor_freetxtsearch||de
  - All Nuggets|/my/index.php#ildmetaselect_form_anchor_freetxtsearch||en

## Custom language settings
- set via administration (Language / Language customisation)
- upload customlang package
  - Course -> Nugget : [customlangpack](./custom_lang/customlang22111002_de.zip)


## Plugins
- mod_MotBot
  - [github](https://github.com/ild-thl/motbot)
   ```
   git clone https://github.com/ild-thl/motbot motbot
   ```
  - needs additional plugins installed in moodle (not installed yet)
    - Telegram plugin
    ```
      git clone https://github.com/pascalhuerten/moodle_telegram.git
    ```
    - Signal plugin
    ```
       git clone https://github.com/pascalhuerten/moodle_signal.git
    ```

- moodle-block_lpprogressx
  - [github](https://github.com/tinjohn/moodle-block_lpprogressx)
- moodle-local_lpautocomplete
  - [gitlab bugfix version until fixed in official version](https://gitlab.com/tinjohn/moodle-local_lpautocompletedeb)
  - [gitlab](https://gitlab.com/adapta/moodle-local_lpautocomplete)
  - [moodle.org](https://moodle.org/plugins/local_lpautocomplete)
- moodle-format_buttonsx (in course/format)
  - [github](https://github.com/tinjohn/moodle-format_buttonsx)
- moodle-block_game
  - [github](https://github.com/JotaDF/moodle-block_game.git)
  - [moodle.org](https://moodle.org/plugins/block_game)
- block_isymetaselect
  - [github](https://github.com/ild-thl/moodle-block_isymetaselect.git)
    ```
      git clone -b master https://github.com/ild-thl/moodle-block_isymetaselect.git ildmetaselect
    ```
  - [github dev OCP](https://github.com/tinjohn/moodle-block_isymetaselect.git)
    ```
      git clone -b master https://github.com/tinjohn/moodle-block_isymetaselect.git ildmetaselect
    ```
- block_isyselect
  - [github](https://github.com/ild-thl/moodle-local_isymeta.git)
    ```
      git clone -b master https://github.com/ild-thl/moodle-local_isymeta.git ildmeta
    ```
  - [github dev OCP](https://github.com/tinjohn/moodle-local_isymeta.git)
     ```
       git clone -b master https://github.com/tinjohn/moodle-local_isymeta.git ildmeta
     ```

## Planned plugins 
- moodle_mod_ilddigitalcert
- [github](https://github.com/oncampus/moodle_mod_ilddigitalcert.git)
  ```
    git clone https://github.com/oncampus/moodle_mod_ilddigitalcert.git ilddigitalcert
  ```
- needs more than the moodle plugin, see readme in repository  


## Plugins for further developements
- moodle-local_metadata (will be used for alternate content)
- moodle-atto_snippets (will be used for alternate content) (in lib/editor/atto/plugins)

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

## Navigationsbuttons
- Appearance -> Theme settings
  - Alle Nuggets|/my/index.php#ildmetaselect_form_anchor_freetxtsearch||de
  - All Nuggets|/my/index.php#ildmetaselect_form_anchor_freetxtsearch||en
- hide on frontpage in RAW SCSS
     ``` 
        .pagelayout-frontpage .primary-navigation {
            visibility: hidden;
         }  
     ```

##  Hide participants – in course and score board
[thanks to](https://www.xelium.co.uk/2018/06/moodle-hide-participants-view-from-students/)
- Go to Site administration > Users > Permissions > Define roles.
- Click the Edit settings icon (the gear button) for the Student role.
- Filter the list by typing ‘Participants‘ in the filter field.
- Make sure you uncheck the two capabilities called View participants. By default the Course: View participants check box is ticked to Allow. Uncheck this.
- Click Save changes to commit the change in Permission

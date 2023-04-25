# Hide participants in course
- Users:Manage Roles:Student
  - moodle/course:viewparticipants false

# Hide Home in top navigation
- advanced SCSS (Appearance:THEME:advanced)
    ```
    div.primary-navigation nav.navigation ul.nav li:first-child {
         display: none;
    }
   ```
# Css for Mobile App - work in progress 20221111
- most plugins are not App ready
- see https://docs.moodle.org/400/en/Moodle_app_guide_for_admins
    - Administration > Site administration > Mobile app > Mobile appearance and enter in the mobilecssurl
    - e.g. copy ocp_mobileapp.css to the theme/style directory and use the according url
    - (write a simple local plugin)

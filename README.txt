PBSE307 - WEB DEVELOPMENT FUNDAMENTALS
WEB GALLERY ASSIGNMENT (Image Gallery and Video Gallery)
STYLED VERSION (HTML + CSS)
=========================================================

IMPORTANT: this is the STYLED version. It uses CSS (styles.css) for a modern
corporate look. The assignment brief asks for plain HTML with NO CSS, so the
plain version in AbelAsiedu_WebgalleryAssignment.zip is the one that follows
the brief. Ask your lecturer before submitting this styled version.

Student name : Abel Asiedu
University   : Pentecost University
Course code  : PBSE307
Course title : Web Development Fundamentals


1. THEMES
---------
Image gallery : NBA Stars and Arenas
                (9 pictures of players in NBA team jerseys + 2 pictures of
                 famous arenas)
Video gallery : NBA Highlights - Dunks, Shooting and Defence
                (6 short clips)


2. FOLDER STRUCTURE
-------------------
AbelAsiedu_WebGallery_Assignment/
  image_gallery.html   Task 1 - the picture gallery page
  video_gallery.html   Task 2 - the video gallery page
  styles.css           the shared stylesheet used by both pages
  README.txt           this file
  fonts/               the font files used by styles.css, with their licence note
  Images/              image_01.jpg ... image_11.jpg  (11 pictures)
  Videos/              video_01.mp4 ... video_06.mp4  (6 videos)

All paths in the HTML files are relative (for example Images/image_01.jpg),
so the project works on any computer after the ZIP file is extracted.
Extract the whole ZIP first. Do not open the pages from inside the ZIP.


3. HOW TO OPEN AND TEST
-----------------------
1. Extract AbelAsiedu_WebgalleryAssignment.zip (right-click > Extract All).
2. Open the extracted folder.
3. Double-click image_gallery.html. It opens in the web browser.
   Check that all 11 pictures show, the five marquee lines move, and the
   information table, the bulleted list and the lettered list are visible.
   Resize the window (or open it on a phone) to see the layout adapt.
4. Double-click video_gallery.html.
   Check that the videos start by themselves (muted) as they scroll into
   view, that every video can be played with its controls, and that the
   table and lists are visible.
5. Use a modern browser such as Chrome, Edge, Firefox or Safari.
   Note: the <marquee> tag is old HTML. Current browsers still run it,
   but it is no longer part of the official HTML standard.


4. IMPORTANT HTML TAGS, ATTRIBUTES AND CSS USED
-----------------------------------------------
Structure     : <html lang>, <head>, <title>, <body>, <meta charset>,
                <meta name="viewport">, <link rel="stylesheet">,
                <header>, <nav>, <main>, <section>, <footer>
Headings      : <h1> (one main heading per page), <h2>, <h3>
Text          : <p>, <dl> with <dt> and <dd> for facts
Moving text   : <marquee> with direction (left, right, up),
                behavior (scroll, alternate, slide) and scrollamount
Images        : <figure> and <figcaption>; <img> with src, width, height
                and alt
Videos        : <video> with width, height, controls, muted, autoplay,
                loop and playsinline; <source> with src and type="video/mp4"
Tables        : <table>, <caption>, <thead>, <tbody>, <tr>, <th scope="col">,
                <td>
Lists         : <ul type="square"> and <ul type="circle">,
                <ol type="A"> and <ol type="1">, with <li>
Links         : <a href> between the pages and to sections (#lakers, ...)

CSS (styles.css, one file shared by both pages)
  Custom properties (--ink, --ball ...) hold the colours, fonts and sizes.
  @font-face loads the local fonts in the fonts/ folder.
  CSS Grid lays out the hero, the picture rows and the video rows; subgrid
  keeps photos and captions aligned across a row.
  Flexbox is used for the header and buttons.
  @media rules adapt the layout for tablets and phones.
  prefers-reduced-motion switches off the line-drawing animation.
  :focus-visible gives keyboard users a clear outline.
  The half-court drawing in the hero is an inline SVG, drawn with CSS.
No JavaScript, no Bootstrap, no CSS frameworks and no remote files are used.
Everything works offline.

Video attributes: every video uses controls, muted, autoplay and loop, so
all six start by themselves and repeat. muted is required because browsers
only allow autoplay when the sound is off; viewers can unmute with the
controls. Browsers may pause an autoplaying video that is scrolled out of
view and start it again when it comes back into view.

5. MEDIA SOURCES AND ATTRIBUTION  (PLEASE READ)
-----------------------------------------------
IMAGES (Images/image_01.jpg to image_11.jpg)
  Supplied by the student. They were saved from the internet and the
  original photographers, agencies and licences are not known to the
  author of this project. Copyright stays with the original owners.
  The pictures are used only as part of this class assignment.
  STUDENT TO COMPLETE: add the source website and photographer for each
  picture here if your lecturer asks for it.
    image_01 - Kawhi Leonard, Clippers No. 2
    image_02 - Jayson Tatum, Celtics No. 0
    image_03 - Philadelphia 76ers No. 7 (player name not confirmed)
    image_04 - LeBron James, Lakers No. 23
    image_05 - Magic Johnson, Lakers No. 32
    image_06 - Michael Jordan, Bulls No. 23
    image_07 - Kobe Bryant, Lakers No. 24
    image_08 - Larry Bird, Celtics No. 33
    image_09 - Stephen Curry, Warriors No. 30
    image_10 - Madison Square Garden, New York (aerial view)
    image_11 - Chase Center, San Francisco (aerial view)
  Player names, positions and achievements were added from general
  basketball knowledge. Michael Jordan and Stephen Curry were named by the
  student. The other names were matched from each picture's team and jersey
  number and should be double-checked by the student; the 76ers No. 7
  player could not be matched, so no name is given. Image 10 has a photographer credit printed in its bottom-left
  corner, which is left unchanged.
  Image 10 was identified from its setting (round arena beside the
  Empire State Building). Image 11 shows the name "Chase Center".

VIDEOS (Videos/video_01.mp4 to video_06.mp4)
  The six clips come from phone screen recordings (dated 27 October 2026)
  of NBA highlight videos posted on social media, supplied by the student.
  They were then trimmed, cropped to remove the phone's buttons and
  menus, and converted to H.264 MP4 so that they play in all browsers.
    video_01 : "Top 10 Poster dunks in NBA history" post (Anthony Edwards'
               dunk; named in the clip's own commentary)
    video_02 : "Some Of The Best NBA Dunks Of All Time" post
    video_03, video_04 : two parts of one recording from the "Top 10 Poster
               dunks in NBA history" post (Clippers plays)
    video_05 : NBA post titled "Steph was PERFECT from the field"
               (Warriors v Nuggets)
    video_06 : "The best basketball blocks in NBA history" post
  The original footage belongs to the NBA, its teams and broadcasters and
  to the people who posted it. It is NOT public domain and NOT freely
  licensed. It is included only for this class assignment. Do not publish
  this project on the internet or share it further without permission.
  Some clips show the original commentary captions.

The lengths in the video table (7.8, 4.7, 3.0, 3.8, 5.7 and 9.6 seconds)
were measured from the final files.

FONTS (fonts/ folder)
  Inter and Inter Display (Copyright 2016 The Inter Project Authors) and
  Lora (Copyright 2011 The Lora Project Authors, Reserved Font Name "Lora")
  are used under the SIL Open Font License 1.1. Details are in
  fonts/FONTS-LICENSE.txt.

---
title: Einführung
date: 2023-07-22T20:49:19+02:00
draft: false

subtitle: 

weight: 10

tags: [hugo]
---

## Hugo

**Hugo** [[w]][w1] [[d]][d1] ist eine freie Software zur schnellen Erzeugung statischer Websites <_static website generator_>.

* Hugo hat einen **HTTP-Server** [[w]][w2] zur lokalen Ansicht der erzeugten HTML-Dateien eingebaut.
* Hugo ist in der Programmiersprache **Go** [[w]][w3] geschrieben.
* Hugo erzeugt die Webseiten aus **HTML**- [[w]][w4] oder **Markdown**-Dateien [[w]][w5].

<!-- Reference Links - Start -->
[w1]: https://de.wikipedia.org/wiki/Freie_Software "wikipedia"
[w2]: https://en.wikipedia.org/wiki/HTTP_server "wikipedia"
[w3]: https://de.wikipedia.org/wiki/Go_(Programmiersprache) "wikipedia"
[w4]: https://de.wikipedia.org/wiki/Hypertext_Markup_Language "wikipedia"
[w5]: https://de.wikipedia.org/wiki/Markdown "wikipedia"
[w4]:  "wikipedia"


[d1]: https://gohugo.io/documentation/ "hugo documentation"
<!-- Reference Links - End -->

[Hugo learn theme](https://learn.netlify.app/en/) Netlify <br>

---

### Hugo und git CLI-Befehle

Auf den Ordner mit dem Projekt gehen.  <br>
> cd documents/programmierung/github/quickstart

Einen neuen Post anlegen. <br>
> hugo new posts/my-first-post.md <br>

Neue Seite auf den lokalen Server bringen. <br>
> hugo server <br>

> hugo server -D <br>

Seiten im public Ordner aktualisieren. <br>
> hugo <br>

Neue Dateien zu git hinzufügen. <br>
> git add . <br>

Die Änderungen lokal commiten. <br>
> git commit -m 'Added files' <br>

Die Änderungen auf das remote GitHub schieben. <br>
> it push -u origin main <br>

Auf GitHub "Action" aktivieren und Seite veröffentlichen.

---

### Neue leere WebSite mit Hugo erstellen

[Getting started with Bootstrap 5 and HUGO static site generator](https://www.youtube.com/watch?v=Vj5zy2q7O9U&list=PLE92IfveVXuXTOjdPM_nleN6Cga_d3uJ-&index=2) Future Web Design <br>

Ordner Einführung-in-swift-und-swiftui erstellt

Ordner in VSCode geöffnet

VSCode Terminal gestartet

```console
hugo new site ./
Congratulations! Your new Hugo site is created in /Users/test/Documents/Programmierung/Github/einfuehrung-in-swift-und-swiftui.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/ or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
```

Leeres theme einrichten

```console
hugo new theme temp
Creating theme at /Users/test/Documents/Programmierung/Github/einfuehrung-in-swift-und-swiftui/themes/temp
```

Inhalt themes/temp layout nach layout verschieben.
Inhalt themes/temp static nach static verschieben.
Rest von themes/temp aus löschen.
temp löschen.

In den leeren Ordnern themes und data .gitkeep Datei eingefügt.

Archetypes default.md angepasst draft: false

```console
hugo new _index.md
Content "/Users/test/Documents/Programmierung/Github/einfuehrung-in-swift-und-swiftui/content/_index.md" created
```

Bootstrap 5 Copy Starter Template in layout/baseof.html

https://getbootstrap.com/docs/5.0/getting-started/introduction/

---

### Links

[Getting Started With Hugo](https://www.youtube.com/watch?v=hjD9jTi_DQ4) Adi Purdila, 2022, 48 min <br>
[Creating your own Hugo Theme!](https://www.youtube.com/watch?v=wcMqrb3v2SM) Eric Murphy, 2021 <br>
[Introduction to Hugo | Hugo - Static Site Generator | Tutorial 1](https://www.youtube.com/watch?v=qtIqKaDlqXo) Mike, 2018, 8 min <br>
[Was ist ein Static-Site-Generator?](https://www.ionos.de/digitalguide/websites/webseiten-erstellen/was-ist-ein-static-site-generator/) IONOS, 2023 <br>
[How to Set Up a Hugo Site on Github Pages - with Git Submodules!](https://dev.to/aormsby/how-to-set-up-a-hugo-site-on-github-pages-with-git-submodules-106p) DEV, 2020 <br>
[Deploy Hugo website using Github pages](https://dev.to/importhuman/deploy-hugo-website-using-github-pages-1mc5) Ujjwal Goyal, 2021 <br>
[Einfach erklärt: Webseiten mit Hugo erstellen](https://trendschau.net/blog/webseiten-mit-hugo) trendschau.net <br>
[Wie man mit Hugo eine rasend schnelle statische Seite erstellt ](https://kinsta.com/de/blog/hugo-statische-seite/) Brian Le, 2013 <br>

Hugo und GitHub-Pages <br>
[Quick start](https://gohugo.io/getting-started/quick-start/) Hugo <br>
[Host on GitHub Pages](https://gohugo.io/hosting-and-deployment/hosting-on-github/) Hugo <br>

---

### Videos

[Hugo on Github pages](https://www.youtube.com/watch?v=vgz-6IDDWOc) Mathieu Besançon, 2019, 112 min

[Creating a Free Blog or Static Content Website with Hugo and GitHub Pages with Custom Domain and Ads](https://www.youtube.com/watch?v=LSJ5S8VG5aU) MissCoding, 2022, 27 min

by Luke Smith <br>
[Hugo Actually Explained (Websites, Themes, Layouts, and Intro to Scripting)](https://www.youtube.com/watch?v=ZFL09qhKi5I) Luke Smith, 2022, 40 min
[Simple Hugo Shortcodes absolutely MOG pathetic obese Wordpress!](https://www.youtube.com/watch?v=QTolhoxMyXg) Luke Smith, 2022, 25 min

CLI-Apps <br>
[Ranger the Terminal File Manager (Going deeper into configuration)](https://www.youtube.com/watch?v=nlolvAVqn10&list=PL-p5XmQHB_JSjgaGQdMPNm3jKVjaMkxSp&index=1) Luke Smith, 2017, 9 min

[Terminal vs. Bash vs. Command line vs. Prompt](https://www.youtube.com/watch?v=hMSByvFHOro) Luke Smith, 2019, 11 min

by Markco Michely <br>
[01 Website erstellen: Wordpress-, Drupal-CMS oder Static Site Generator?](https://www.youtube.com/watch?v=eSIzPFtMteM) Marco Michely, 2017, 22 min <br>
[02 Website erstellen: Den richtigen Static Site Generator finden]( https://www.youtube.com/watch?v=GxjCmXXaHes) Marco Michely, 2017, 8 min <br>
[03 Statische Website mit HUGO erstellen
](https://www.youtube.com/watch?v=ChaNUan-SK0) Marco Michely, 2017, 39 min <br>
[04 Baue mit HUGO statische Websites wie ein Profi](https://www.youtube.com/watch?v=BUQzuIq_PNQ) Marco Michely, 2017, 47 min <br>
[05 Statische Websites mit HUGO](https://www.youtube.com/watch?v=PlqrXZjCoQc) Marco Michely, 2017, 11 min <br>
[06 Responsive Images und HUGO - Grundlagen]( https://www.youtube.com/watch?v=jfhf6kMCUZk) Marco Michely, 2017, 28 min <br>

Hugo and Bootstrap 5 by Future Web Design <br>
[01 Installing Hugo Static Site Generator and software for Development environment on Windows](https://www.youtube.com/watch?v=l7PHRA8t4Bw) Future Web Design, 2020, 10 min <br>
[02 Getting started with Bootstrap 5 and HUGO - Introduction](https://www.youtube.com/watch?v=Vj5zy2q7O9U) Future Web Design, 2022, 53 min <br>
[03 Dynamic JavaScript year/date in copyright footer](https://www.youtube.com/watch?v=HcyBdgJhDZI) Future Web Design, 2022, 18 min <br>
[04 Integrating HUGO with NPM node.js package manager](https://www.youtube.com/watch?v=9ODyMFnGma8) Future Web Design, 2022, 24 min <br>
[05 SCSS & SASS Compiling with Hugo](https://www.youtube.com/watch?v=wgB7kMEVOg0) Future Web Design, 2022, 41 min <br>
[06 HUGO with SCSS and SASS + PostCSS, Autoprefixer](https://www.youtube.com/watch?v=kHuRp7W8StE) Future Web Design, 2022, 43 min <br>
[07 HUGO and Bootstrap 5 Navbar Introduction](https://www.youtube.com/watch?v=Di11hJUFd-E) Future Web Design, 2022, 21 min <br>
[08 Hugo + HTML 5 Semantic Elements & Templates](https://www.youtube.com/watch?v=bt6be18-cxg) Future Web Design, 2022, 30 min <br>
[09 Bootstrap 5 Cards with Hugo - Loop over front matter data with range.](https://www.youtube.com/watch?v=gjd8fKSSuB0) Future Web Design, 2022, 19 min <br>
[10 Save time with NPM scripts](https://www.youtube.com/watch?v=d7L8ydAdu7U) Future Web Design, 2022, 13 min <br>
[11 Enable render of HTML in Markdown](https://www.youtube.com/watch?v=igIXqfSxm4k) Future Web Design, 2022, 5 min <br>
[12 Minifying with HUGO - the right way!](https://www.youtube.com/watch?v=5QfVNP-UC6g) Future Web Design, 2022, 11 min <br>
[13 Changing the Site Language](https://www.youtube.com/watch?v=TaMicUc9GSM) Future Web Design, 2022, 5 min <br>
[14 Starting a new GitHub Project with HUGO](https://www.youtube.com/watch?v=NPnMZJXJx5g) Future Web Design, 2022, 7 min <br>
[15 Test Netlify CMS Config Locally](https://www.youtube.com/watch?v=byFBKrM9MNY) Future Web Design, 2022, 5 min <br>
[16 Creating Masonry/Pinterest style image gallery](https://www.youtube.com/watch?v=2b6gTq1zFt0) Future Web Design, 2022, 9 min <br>
[17 Creating Instagram Square style image gallery](https://www.youtube.com/watch?v=s61ZwPC4Q7g) Future Web Design, 2022, 12 min <br>
[18 Social Media Sharing with Twitter, Facebook, Linkedin & Pinterest](https://www.youtube.com/watch?v=jn5SwgN_B9s) Future Web Design, 2022, 9 min <br>
[19 Save time with NPM scripts](https://www.youtube.com/watch?v=V4nFtwu7cpM) Future Web Design, 2022, 14 min <br>
[20 Use Prettier for HUGO & Go Templates in Visual Studio Code](https://www.youtube.com/watch?v=1L7b3dm0j9o) Future Web Design, 2022, 13 min <br>
[21 Social Media Sharing with Twitter, Facebook, Linkedin & Pinterest](https://www.youtube.com/watch?v=MaaMdWyek6Y) Future Web Design, 2022, 9 min <br>
[22 Bootstrap 5 Menu Navbar with Dropdowns](https://www.youtube.com/watch?v=Ecm1OcljA2o) Future Web Design, 2022, 27 min <br>
[23 Bootstrap 5 Breadcrumbs](https://www.youtube.com/watch?v=70rb6nE0SPI) Future Web Design, 2022, 7 min <br>
[24 How to import Hugo modules](https://www.youtube.com/watch?v=kd-9T-k1wes) Future Web Design, 2022, 7 min <br>

[Starting a new GitHub Project with HUGO](https://www.youtube.com/watch?v=NPnMZJXJx5g) Future Web Design, 2020, 7 min <br>
[Test Netlify CMS Config Locally](https://www.youtube.com/watch?v=byFBKrM9MNY) Future Web Design, 2022, 5 min <br>
[How to import Hugo modules into your Hugo Website](https://www.youtube.com/watch?v=kd-9T-k1wes) Future Web Design, 2023, 7 min <br>
[Use Prettier for HUGO & Go Templates in Visual Studio Code](https://www.youtube.com/watch?v=1L7b3dm0j9o) Future Web Design, 2022, 13 min <br>
[Use Prettier and ESLint in Visual Studio Code | Lint and Format your Code](https://www.youtube.com/watch?v=kWIlrSorqFE) Future Web Design, 2022, 16 min <br>
[Test Netlify CMS Config Locally](https://www.youtube.com/watch?v=byFBKrM9MNY) Future Web Design, 2022, 3 min <br>

by Chris Stayte <br>
[01 Buy, Build, Host a Website for $12](https://www.youtube.com/watch?v=5aajv-2YZYM) Chris Stayte, 2018, 8 min <br>
[02 Why Use A Static Site Generator](https://www.youtube.com/watch?v=mDKQGANttyE) Chris Stayte, 2018, 10 min <br>
[03 Building A Website Using Hugo](https://www.youtube.com/watch?v=c7vpcqA6SEQ) Chris Stayte, 2018, 35 min <br>
[04 Hosting Your Website With Github and Netlify](https://www.youtube.com/watch?v=hBQlCtfRmqs) Chris Stayte, 2018, 18 min <br>
[05 Purchasing A Domain (Google Domains)](https://www.youtube.com/watch?v=S7DVyHfv4zM) Chris Stayte, 2018, 8 min <br>
[Xxx06 Setup Custom Domain On Netlify](https://www.youtube.com/watch?v=Q9giWrfIJK&list=PL-Kz5P-mYdMgAJDmRJquyMHfdaIOD-3oj&index=6) Chris Stayte, 2018, 11 min <br>
[07 Netlify CMS](https://www.youtube.com/watch?v=_CNZJLYvINc) Chris Stayte, 2018, 19 min <br>
[08 Updating Hugo on Netlify](https://www.youtube.com/watch?v=c1_-Xq296Dk) Chris Stayte, 2018, 5 min <br>
[Xxx09 Add A Form To Your Netlify Powered Website](https://www.youtube.com&list=PL-Kz5P-mYdMgAJDmRJquyMHfdaIOD-3oj&index=9) Chris Stayte, 2018, 25 min <br>
 
---

### Hugo

  completion  Generate the autocompletion script for the specified shell
  config      Print the site configuration
  convert     Convert your content to different formats
  deploy      Deploy your site to a Cloud provider.
  env         Print Hugo version and environment info
  gen         A collection of several useful generators.
  help        Help about any command
  import      Import your site from others.
  list        Listing out various types of content
  mod         Various Hugo Modules helpers.
  new         Create new content for your site
  server      A high performance webserver
  version 


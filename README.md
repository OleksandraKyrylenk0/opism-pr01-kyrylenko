# Практична робота № 1

**Дисципліна:** Основи побудови інформаційних систем та мереж

**Тема:** Спостереження за процесом звернення до вебресурсу. Побудова власної моделі рівнів взаємодії

| | |
|---|---|
| **Прізвище, ім'я** |Кириленко Олександра |
| **Група** |Іпз 2.1 |
| **Номер варіанта** | 9|
| **Домен варіанта** |fortran-lang.org |
| **Середовище виконання** |  macOS |
| **Версія curl** | curl 8.7.1 (x86_64-apple-darwin25.0) libcurl/8.7.1 (SecureTransport) LibreSSL/3.3.6 zlib/1.2.12 nghttp2/1.68.1 |
| **Дата виконання** | 09.09.2026 |

---

## Частина A. Збір експериментальних даних

### A.1. Запит із діагностичним виводом

**Команда:**

```
curl -v https://fortran-lang.org
```

**Вивід:**

```
* Host fortran-lang.org:443 was resolved.
* IPv6: (none)
* IPv4: 185.199.111.153, 185.199.110.153, 185.199.109.153, 185.199.108.153
*   Trying 185.199.111.153:443...
* Connected to fortran-lang.org (185.199.111.153) port 443
* ALPN: curl offers h2,http/1.1
* (304) (OUT), TLS handshake, Client hello (1):
*  CAfile: /etc/ssl/cert.pem
*  CApath: none
* (304) (IN), TLS handshake, Server hello (2):
* (304) (IN), TLS handshake, Unknown (8):
* (304) (IN), TLS handshake, Certificate (11):
* (304) (IN), TLS handshake, CERT verify (15):
* (304) (IN), TLS handshake, Finished (20):
* (304) (OUT), TLS handshake, Finished (20):
* SSL connection using TLSv1.3 / AEAD-CHACHA20-POLY1305-SHA256 / [blank] / UNDEF
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=fortran-lang.org
*  start date: Jul 21 08:58:21 2026 GMT
*  expire date: Oct 19 08:58:20 2026 GMT
*  subjectAltName: host "fortran-lang.org" matched cert's "fortran-lang.org"
*  issuer: C=US; O=Let's Encrypt; CN=YR2
*  SSL certificate verify ok.
* using HTTP/2
* [HTTP/2] [1] OPENED stream for https://fortran-lang.org/
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: fortran-lang.org]
* [HTTP/2] [1] [:path: /]
* [HTTP/2] [1] [user-agent: curl/8.7.1]
* [HTTP/2] [1] [accept: */*]
> GET / HTTP/2
> Host: fortran-lang.org
> User-Agent: curl/8.7.1
> Accept: */*
> 
* Request completely sent off
< HTTP/2 200 
< server: GitHub.com
< content-type: text/html; charset=utf-8
< last-modified: Wed, 09 Sep 2026 08:08:05 GMT
< access-control-allow-origin: *
< etag: "6aa113e5-7309"
< expires: Wed, 09 Sep 2026 08:42:22 GMT
< cache-control: max-age=600
< x-proxy-cache: MISS
< x-github-request-id: 69C6:149E32:8DF4B2:8F8D95:6AA11996
< x-github-edge-region: fra
< accept-ranges: bytes
< age: 0
< date: Wed, 09 Sep 2026 08:32:22 GMT
< via: 1.1 varnish
< x-served-by: cache-vie6346-VIE
< x-cache: MISS
< x-cache-hits: 0
< x-timer: S1788942742.405481,VS0,VE126
< vary: Accept-Encoding
< x-fastly-request-id: 7cd180770a78deadacfed0198ea9ccae00f61cbc
< content-length: 29449
< 

<!DOCTYPE html>


<html lang="en" data-content_root="./" >

  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="icon" sizes="256x256" href="_static/images/favicon.ico" type="image/x-icon">
    <title>The Fortran Programming Language &#8212; Fortran Programming Language</title>
  
  
  
  <script data-cfasync="false">
    document.documentElement.dataset.mode = localStorage.getItem("mode") || "";
    document.documentElement.dataset.theme = localStorage.getItem("theme") || "";
  </script>
  <!--
    this give us a css class that will be invisible only if js is disabled
  -->
  <noscript>
    <style>
      .pst-js-only { display: none !important; }

    </style>
  </noscript>
  
  <!-- Loaded before other Sphinx assets -->
  <link href="_static/styles/theme.css?digest=90905a2f556bf617f1a9" rel="stylesheet" />
<link href="_static/styles/pydata-sphinx-theme.css?digest=90905a2f556bf617f1a9" rel="stylesheet" />

    <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=8f2a1f02" />
    <link rel="stylesheet" type="text/css" href="_static/copybutton.css?v=76b2166b" />
    <link rel="stylesheet" type="text/css" href="_static/sphinx-design.min.css?v=95c83b7e" />
    <link rel="stylesheet" type="text/css" href="_static/custom.css?v=0a3c677e" />
  
  <!-- So that users can add custom icons -->
  <script defer src="_static/scripts/fontawesome.js?digest=90905a2f556bf617f1a9"></script>
  <!-- Pre-loaded scripts that we'll load fully later -->
  <link rel="preload" as="script" href="_static/scripts/bootstrap.js?digest=90905a2f556bf617f1a9" />
<link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=90905a2f556bf617f1a9" />

    <script src="_static/documentation_options.js?v=51fd25b1"></script>
    <script src="_static/doctools.js?v=fd6eb6e6"></script>
    <script src="_static/sphinx_highlight.js?v=6ffebe34"></script>
    <script src="_static/clipboard.min.js?v=a7894cd8"></script>
    <script src="_static/copybutton.js?v=6dbb43f8"></script>
    <script src="_static/design-tabs.js?v=f930bc37"></script>
    <script>DOCUMENTATION_OPTIONS.pagename = 'index';</script>
    <script>
        DOCUMENTATION_OPTIONS.theme_version = '0.20.0';
        DOCUMENTATION_OPTIONS.theme_switcher_json_url = 'https://fortran-lang.org/_static/data.json';
        DOCUMENTATION_OPTIONS.theme_switcher_version_match = 'en';
        DOCUMENTATION_OPTIONS.show_version_warning_banner =
            false;
        </script>
    <script>DOCUMENTATION_OPTIONS.search_as_you_type = false;</script>
    <link rel="canonical" href="https://fortran-lang.org/" />
    <link rel="index" title="Index" href="genindex/" />
    <link rel="search" title="Search" href="search/" />
    <link rel="next" title="Learn" href="learn/" /> 
<meta
  name="description"
  content="Fortran : High-performance parallel programming language"
/>
<meta
  name="keywords"
  content="High-performance, parallel, programming language"
/>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script type="text/javascript">
  var pr_number = -1;
  $(document).ready(function () {
    if (window.location.href.indexOf("/pr/") > -1) {
      pr_number = window.location.href.split("/").indexOf("pr") + 1;
      document.getElementById("pr").innerHTML =
        "pull request " + window.location.href.split("/")[pr_number];
      document.getElementById("pr").href =
        "https://github.com/fortran-lang/webpage/pull/" +
        window.location.href.split("/")[pr_number];
      var banner = document.getElementById("banner");
      banner.style.display = "block";
    }
  });
</script>
<div id="banner" style="display: none" class="container">
  <h3>
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="24"
      height="24"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="feather feather-git-pull-request"
    >
      <circle cx="18" cy="18" r="3"></circle>
      <circle cx="6" cy="6" r="3"></circle>
      <path d="M13 6h3a2 2 0 0 1 2 2v7"></path>
      <line x1="6" y1="9" x2="6" y2="21"></line>
    </svg>
    <b>Site preview: </b>you are previewing unpublished changes for
    <a id="pr"></a>
  </h3>
</div> 
<link
  rel="alternate"
  type="application/atom+xml"
  href="news/atom.xml"
  title="Blog"
/>
 
<link href="True" rel="stylesheet" />
 
  </head>
  <body data-default-mode="">
  
  
  <div id="pst-skip-link" class="skip-link d-print-none"><a href="#main-content">Skip to main content</a></div>

  
  <div id="pst-scroll-pixel-helper"></div>
  
  <button type="button" class="btn rounded-pill" id="pst-back-to-top">
    <i class="fa-solid fa-arrow-up"></i>Back to top</button>
  
  
  
  
  <dialog id="pst-search-dialog">
    
<form class="bd-search d-flex align-items-center"
      action="search/"
      method="get">
  <i class="fa-solid fa-magnifying-glass"></i>
  <input type="search"
         class="form-control"
         name="q"
         placeholder="Search"
         aria-label="Search"
         autocomplete="off"
         autocorrect="off"
         autocapitalize="off"
         spellcheck="false"/>
  <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd>K</kbd></span>
</form>
  </dialog>

  <div class="pst-async-banner-revealer d-none">
  <aside id="bd-header-version-warning" class="d-none d-print-none" aria-label="Version warning"></aside>
</div>

  
    <header id="pst-header" class="bd-header navbar navbar-expand-lg bd-navbar d-print-none">
<div class="bd-header__inner bd-page-width">
  <button class="pst-navbar-icon sidebar-toggle primary-toggle" aria-label="Site navigation">
    <span class="fa-solid fa-bars"></span>
  </button>
  
  
  <div class=" navbar-header-items__start">
    
      <div class="navbar-item">

  
    
  

<a class="navbar-brand logo" href="#">
  
  
  
  
  
    
    
      
    
    
    <img src="_static/fortran-logo-256x256.png" class="logo__image only-light" alt="Fortran Programming Language - Home"/>
    <img src="_static/fortran-logo-256x256.png" class="logo__image only-dark pst-js-only" alt="Fortran Programming Language - Home"/>
  
  
</a></div>
    
      <div class="navbar-item">

<div class="theme-switch-container dropdown pst-js-only" data-bs-toggle="tooltip" data-bs-placement="bottom" title="Color mode">
  <button class="btn btn-sm nav-link pst-navbar-icon theme-switch-button dropdown-toggle" aria-label="Color mode" data-bs-toggle="dropdown">
    <i class="theme-switch fa-solid fa-sun fa-lg fa-fw" data-mode="light" title="Light"></i>
    <i class="theme-switch fa-solid fa-moon fa-lg fa-fw" data-mode="dark" title="Dark"></i>
    <i class="theme-switch fa-solid fa-circle-half-stroke fa-lg fa-fw" data-mode="auto" title="System Settings"></i>
  </button>
  <ul class="dropdown-menu dropdown-menu-end">
    <li><button class="dropdown-item d-flex align-items-center theme-change-button" data-mode="auto"><i class="fa-solid fa-circle-half-stroke fa-lg fa-fw me-1"></i>System Settings</button></li>
    <li><button class="dropdown-item d-flex align-items-center theme-change-button" data-mode="light"><i class="fa-solid fa-sun fa-lg fa-fw me-1"></i>Light</button></li>
    <li><button class="dropdown-item d-flex align-items-center theme-change-button" data-mode="dark"><i class="fa-solid fa-moon fa-lg fa-fw me-1"></i>Dark</button></li>
  </ul>
</div></div>
    
  </div>
  
  <div class=" navbar-header-items">
    
    <div class="ms-auto navbar-header-items__center">
      
        <div class="navbar-item">
<nav>
  <ul class="bd-navbar-elements navbar-nav">
    
<li class="nav-item ">
  <a class="nav-link nav-external" href="https://dev.lfortran.org/">
    Play
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="learn/">
    Learn
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="compilers/">
    Compilers
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="packages/">
    Packages
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="community/">
    Community
  </a>
</li>

            <li class="nav-item dropdown">
                <button class="btn dropdown-toggle nav-item" type="button"
                data-bs-toggle="dropdown" aria-expanded="false"
                aria-controls="pst-nav-more-links">
                    More
                </button>
                <ul id="pst-nav-more-links" class="dropdown-menu">
                    
<li class=" ">
  <a class="nav-link dropdown-item nav-internal" href="roadmap/">
    Roadmap <!-- omit in toc -->
  </a>
</li>


<li class=" ">
  <a class="nav-link dropdown-item nav-internal" href="news/">
    News
  </a>
</li>

                </ul>
            </li>
            
  </ul>
</nav></div>
      
    </div>
    
    
    <div class="navbar-header-items__end">
      
        <div class="navbar-item navbar-persistent--container">
          

<button class="btn search-button-field search-button__button pst-js-only" title="Search" aria-label="Search" data-bs-placement="bottom" data-bs-toggle="tooltip">
 <i class="fa-solid fa-magnifying-glass"></i>
 <span class="search-button__default-text">Search</span>
 <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd class="kbd-shortcut__modifier">K</kbd></span>
</button>
        </div>
      
      
        <div class="navbar-item"><ul class="navbar-icon-links"
    aria-label="Icon Links">
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://fortran-lang.discourse.group/" title="Discourse" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fab fa-discourse fa-lg" aria-hidden="true"></i><span class="visually-hidden">Discourse</span></a>
        </li>
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://twitter.com/fortranlang" title="Twitter" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fab fa-twitter fa-lg" aria-hidden="true"></i><span class="visually-hidden">Twitter</span></a>
        </li>
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://github.com/fortran-lang" title="GitHub" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fab fa-github fa-lg" aria-hidden="true"></i><span class="visually-hidden">GitHub</span></a>
        </li>
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://fortran-lang.org/news/atom.xml" title="RSS" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fas fa-rss fa-lg" aria-hidden="true"></i><span class="visually-hidden">RSS</span></a>
        </li>
</ul></div>
      
        <div class="navbar-item">
<div class="version-switcher__container dropdown pst-js-only">
  <button id="pst-version-switcher-button-2"
    type="button"
    class="version-switcher__button btn btn-sm dropdown-toggle"
    data-bs-toggle="dropdown"
    aria-haspopup="listbox"
    aria-controls="pst-version-switcher-list-2"
    aria-label="Version switcher list"
  >
    Choose version  <!-- this text may get changed later by javascript -->
    <span class="caret"></span>
  </button>
  <div id="pst-version-switcher-list-2"
    class="version-switcher__menu dropdown-menu list-group-flush py-0"
    role="listbox" aria-labelledby="pst-version-switcher-button-2">
    <!-- dropdown will be populated by javascript on page load -->
  </div>
</div></div>
      
    </div>
    
  </div>
  
  
    <div class="navbar-persistent--mobile">

<button class="btn search-button-field search-button__button pst-js-only" title="Search" aria-label="Search" data-bs-placement="bottom" data-bs-toggle="tooltip">
 <i class="fa-solid fa-magnifying-glass"></i>
 <span class="search-button__default-text">Search</span>
 <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd class="kbd-shortcut__modifier">K</kbd></span>
</button>
    </div>
  

  
    <button class="pst-navbar-icon sidebar-toggle secondary-toggle" aria-label="On this page">
      <span class="fa-solid fa-outdent"></span>
    </button>
  
</div>

    </header>
  

  <div class="bd-container">
    <div class="bd-container__inner bd-page-width">
      
      
      
        
      
      <dialog id="pst-primary-sidebar-modal"></dialog>
      <div id="pst-primary-sidebar" class="bd-sidebar-primary bd-sidebar">
        

  
  <div class="sidebar-header-items sidebar-primary__section">
    
    
      <div class="sidebar-header-items__center">
        
          
          
            <div class="navbar-item">
<nav>
  <ul class="bd-navbar-elements navbar-nav">
    
<li class="nav-item ">
  <a class="nav-link nav-external" href="https://dev.lfortran.org/">
    Play
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="learn/">
    Learn
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="compilers/">
    Compilers
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="packages/">
    Packages
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="community/">
    Community
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="roadmap/">
    Roadmap <!-- omit in toc -->
  </a>
</li>


<li class="nav-item ">
  <a class="nav-link nav-internal" href="news/">
    News
  </a>
</li>

  </ul>
</nav></div>
          
        
      </div>
    
    
    
      <div class="sidebar-header-items__end">
        
          <div class="navbar-item"><ul class="navbar-icon-links"
    aria-label="Icon Links">
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://fortran-lang.discourse.group/" title="Discourse" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fab fa-discourse fa-lg" aria-hidden="true"></i><span class="visually-hidden">Discourse</span></a>
        </li>
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://twitter.com/fortranlang" title="Twitter" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fab fa-twitter fa-lg" aria-hidden="true"></i><span class="visually-hidden">Twitter</span></a>
        </li>
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://github.com/fortran-lang" title="GitHub" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fab fa-github fa-lg" aria-hidden="true"></i><span class="visually-hidden">GitHub</span></a>
        </li>
        <li class="nav-item">
          
          
          
          
          
          
          
          
          <a href="https://fortran-lang.org/news/atom.xml" title="RSS" class="nav-link pst-navbar-icon" rel="noopener" target="_blank" data-bs-toggle="tooltip" data-bs-placement="bottom"><i class="fas fa-rss fa-lg" aria-hidden="true"></i><span class="visually-hidden">RSS</span></a>
        </li>
</ul></div>
        
          <div class="navbar-item">
<div class="version-switcher__container dropdown pst-js-only">
  <button id="pst-version-switcher-button-3"
    type="button"
    class="version-switcher__button btn btn-sm dropdown-toggle"
    data-bs-toggle="dropdown"
    aria-haspopup="listbox"
    aria-controls="pst-version-switcher-list-3"
    aria-label="Version switcher list"
  >
    Choose version  <!-- this text may get changed later by javascript -->
    <span class="caret"></span>
  </button>
  <div id="pst-version-switcher-list-3"
    class="version-switcher__menu dropdown-menu list-group-flush py-0"
    role="listbox" aria-labelledby="pst-version-switcher-button-3">
    <!-- dropdown will be populated by javascript on page load -->
  </div>
</div></div>
        
      </div>
    
  </div>
  
    <div class="sidebar-primary-items__start sidebar-primary__section">
        <div class="sidebar-primary-item">
<div class="index_joinus">
  <h3 id="chat">
    <p style="color: #734f96">Join us!</p>
  </h3>
  <h4><i class="fas fa-envelope-open-text"></i> Mailing list</h4>
  <p>
    Subscribe to our
    <a href="https://groups.io/g/fortran-lang" target="_blank">mailing list</a>
    to discuss anything Fortran related, announce Fortran projects, discuss
    development of core fortran-lang.org projects (stdlib, fpm), and get the
    latest news.
  </p>
  <h4><i class="fab fa-discourse"></i> Discourse</h4>
  <p>
    Join the discussion about all things Fortran on the
    <a href="https://fortran-lang.discourse.group" target="_blank"
      >fortran-lang discourse.</a
    >
  </p>
  <h4><i class="fab fa-twitter"></i> Twitter</h4>
  <a
    href="https://twitter.com/fortranlang"
    class="twitter-follow-button"
    data-show-count="true"
    data-size="large"
    >@fortranlang</a
  >
  <script
    async
    src="https://platform.twitter.com/widgets.js"
    charset="utf-8"
  ></script>
  <h4><i class="fas fa-rss"></i> RSS feed</h4>
  <p>
    RSS clients can follow the
    <a href="news/atom.xml" target="_blank">RSS feed</a>.
  </p>
  <h4><i class="fab fa-github"></i> Open source</h4>
  <p>
    Contribute code, report bugs and request features at
    <a href="https://github.com/fortran-lang" target="_blank">GitHub</a>.
  </p>
</div>
</div>
    </div>
  
  
  <div class="sidebar-primary-items__end sidebar-primary__section">
  </div>


      </div>
      
      <main id="main-content" class="bd-main" role="main">
        
        
          <div class="bd-content">
            <div class="bd-article-container">
              
              <div class="bd-header-article d-print-none"></div>
              
              
              
                
<div id="searchbox"></div>
                <article class="bd-article">
                   <section class="tex2jax_ignore mathjax_ignore" id="the-fortran-programming-language">
<h1 class="sd-d-none">The Fortran Programming Language<a class="headerlink" href="#the-fortran-programming-language" title="Link to this heading">#</a></h1>
<div class="sd-text-center sd-fs-3 sd-font-weight-bold sd-text-primary docutils">
<p>Fortran <br> High-performance parallel programming language</p>
</div>
<div class="sd-text-center sd-fs-4 docutils">
<p><a class="sd-sphinx-override sd-badge sd-bg-primary sd-bg-text-primary reference external" href="learn/"><span>Get started</span></a></p>
</div>
<div class="sd-fs-3 sd-font-weight-bold sd-text-primary docutils">
<p>Features</p>
</div>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>High performance</p>
</div>
<p>Fortran has been designed from the ground up for computationally intensive applications in science and engineering. Mature and battle-tested compilers and libraries allow you to write code that runs close to the metal, fast.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>Statically and strongly typed</p>
</div>
<p>Fortran is statically and strongly typed, which allows the compiler to catch many programming errors early on for you. This also allows the compiler to generate efficient binary code.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>Easy to learn and use</p>
</div>
<p>Fortran is a relatively small language that is surprisingly easy to learn and use. Expressing most mathematical and arithmetic operations over large arrays is as simple as writing them as equations on a whiteboard.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>Versatile</p>
</div>
<p>Fortran allows you to write code in a style that best fits your problem: imperative, procedural, array-oriented, object-oriented, or functional.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>Built-in parallelism</p>
</div>
<p>Fortran directly supports parallel programming with its intuitive array-like syntax to communicate data between CPUs. You can run almost the same code on a single CPU, on a shared-memory multicore system, or on a distributed-memory HPC or cloud-based system. Coarrays, teams, events, and collective subroutines allow you to express different parallel programming patterns that best fit your problem at hand.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>Interoperable</p>
</div>
<p>Fortran’s standardized C interoperability enables seamless integration into multi-language projects, enabling the optimization of performance-critical components.</p>
<div class="sd-fs-3 sd-font-weight-bold sd-text-primary docutils">
<p>FAQ</p>
</div>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>What is the status of Fortran?</p>
</div>
<p>Fortran is mature and under active development.
The latest revision of the language is
<a class="reference external" href="https://wg5-fortran.org/N2201-N2250/N2212.pdf">Fortran 2023</a>.
For the latest published interpretations, see the
<a class="reference external" href="https://go.lbl.gov/fortran-2023">Fortran 2023 Interpretation Document</a>.
There are over a dozen open source and proprietary
<a class="reference internal" href="compilers/"><span class="doc std std-doc">Fortran compilers</span></a>.
Further, open source projects like the
<a class="reference external" href="https://github.com/fortran-lang/stdlib">Standard Library</a>
and the <a class="reference external" href="https://fpm.fortran-lang.org">Fortran Package Manager</a> are
under active development.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>What is Fortran used for?</p>
</div>
<p>Fortran is mostly used in domains that adopted computation early–science and engineering. These include numerical weather and ocean prediction, computational fluid dynamics, applied math, statistics, and finance. Fortran is the dominant language of High Performance Computing and is used to <a class="reference external" href="https://top500.org/">benchmark the fastest supercomputers in the world</a>.</p>
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p>Should I use Fortran for my new project?</p>
</div>
<p>If you’re writing a program or a library to perform fast arithmetic computation over large numeric arrays, Fortran is the optimal tool for the job.</p>
<div class="index_joinus_mobile">
<h3><p style="color:#734f96;">Join us!</p> </h3>
<h4> <i class="fas fa-envelope-open-text"></i> Mailing list</h4>
<p>Subscribe to our <a href="https://groups.io/g/fortran-lang" target="_blank">mailing list</a>
to discuss anything Fortran related, announce Fortran projects, discuss development
of core fortran-lang.org projects (stdlib, fpm), and get
the latest news.
</p>
<h4><i class="fab fa-discourse"></i> Discourse</h4>
<p>
Join the discussion about all things Fortran on the
<a href="https://fortran-lang.discourse.group" target="_blank">fortran-lang discourse.</a>
</p>
<h4><i class="fab fa-twitter"></i> Twitter</h4>
<a href="https://twitter.com/fortranlang" class="twitter-follow-button" data-show-count="true"
data-size="large">@fortranlang</a>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
<h4><i class="fas fa-rss"></i> RSS feed</h4>
<p>RSS clients can follow the <a href="news/atom.xml" target="_blank">RSS feed</a>.</p>
<h4><i class="fab fa-github"></i> Open source</h4>
<p>
Contribute code, report bugs and request features at
<a href="https://github.com/fortran-lang" target="_blank">GitHub</a>.
</p>
</div>
<div class="sd-fs-3 sd-font-weight-bold sd-text-primary docutils">
<p>Make Fortran better</p>
</div>
<div class="sd-container-fluid sd-sphinx-override sd-mb-4 docutils">
<div class="sd-row sd-row-cols-2 sd-row-cols-xs-2 sd-row-cols-sm-2 sd-row-cols-md-2 sd-row-cols-lg-2 docutils">
<div class="sd-col sd-d-flex-row sd-col-6 sd-col-xs-6 sd-col-sm-6 sd-col-md-6 sd-col-lg-6 docutils">
<div class="sd-card sd-sphinx-override sd-w-100 sd-shadow-sm docutils">
<div class="sd-card-body docutils">
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p class="sd-card-text">Write proposals</p>
</div>
<p class="sd-card-text">Have an idea about how to improve the language? You can write new proposals or contribute to existing proposals to the Fortran Standard Committee on
<a class="reference external" href="https://github.com/j3-fortran/fortran_proposals">GitHub</a>.</p>
</div>
</div>
</div>
<div class="sd-col sd-d-flex-row sd-col-6 sd-col-xs-6 sd-col-sm-6 sd-col-md-6 sd-col-lg-6 docutils">
<div class="sd-card sd-sphinx-override sd-w-100 sd-shadow-sm docutils">
<div class="sd-card-body docutils">
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p class="sd-card-text">Develop tools</p>
</div>
<p class="sd-card-text">You can also help make Fortran better by contributing to its suite of tools, such as <a class="reference external" href="https://github.com/fortran-lang/stdlib">Standard Library</a>, <a class="reference external" href="https://github.com/fortran-lang/fpm">Package Manager</a>, <a class="reference external" href="https://github.com/fortran-lang/webpage">this website</a>.</p>
</div>
</div>
</div>
</div>
</div>
<div class="sd-container-fluid sd-sphinx-override sd-mb-4 docutils">
<div class="sd-row sd-row-cols-2 sd-row-cols-xs-2 sd-row-cols-sm-2 sd-row-cols-md-2 sd-row-cols-lg-2 docutils">
<div class="sd-col sd-d-flex-row sd-col-12 sd-col-xs-12 sd-col-sm-12 sd-col-md-12 sd-col-lg-12 docutils">
<div class="sd-card sd-sphinx-override sd-w-100 sd-shadow-sm docutils">
<div class="sd-card-body docutils">
<div class="sd-fs-5 sd-font-weight-bold docutils">
<p class="sd-card-text">Write Fortran software</p>
</div>
<p class="sd-card-text">Or just write Fortran software for your research, business, or schoolwork. You can learn how to <a class="reference internal" href="learn/"><span class="doc std std-doc">get started here</span></a>.</p>
</div>
</div>
</div>
</div>
</div>
<div class="toctree-wrapper compound">
</div>
</section>

<div class="section ablog__blog_comments">
   
</div>

                </article>
              
              
              
              
              
            </div>
            
            
              
                <dialog id="pst-secondary-sidebar-modal"></dialog>
                <div id="pst-secondary-sidebar" class="bd-sidebar-secondary bd-toc"><div class="sidebar-secondary-items sidebar-secondary__inner">


  <div class="sidebar-secondary-item"> 

<h2>
  <p style="color: #734f96">News</p>
</h2>
<ul>
   
  <li>
    <a href="news/2026/05-05-Back-to-the-Fortran-Future-3/"
      >Back to the Fortran Future 3</a
    >
  </li>
  
  <li>
    <a href="news/2026/01-02-Fortran-Newsletter-February-2026/"
      >Fortran newsletter: February 2026</a
    >
  </li>
  
  <li>
    <a href="news/2026/01-23-Fortran-index-blogpost/"
      >Fortran index CAKE fellowship</a
    >
  </li>
  
  <li>
    <a href="news/2022/06-09-Fortran-Newsletter-June-2022/"
      >Fortran newsletter: June 2022</a
    >
  </li>
  
  <li>
    <a href="news/2022/05-05-Fortran-Newsletter-May-2022/"
      >Fortran newsletter: May 2022</a
    >
  </li>
  
</ul>
<a
  class="twitter-timeline"
  data-height="500"
  href="https://twitter.com/fortranlang?ref_src=twsrc%5Etfw"
></a>
<script
  async
  src="https://platform.twitter.com/widgets.js"
  charset="utf-8"
></script>

  </div>

</div></div>
              
            
          </div>
          <footer class="bd-footer-content">
            
          </footer>
        
      </main>
    </div>
  </div>
  
  <!-- Scripts loaded after <body> so the DOM is not blocked -->
  <script defer src="_static/scripts/bootstrap.js?digest=90905a2f556bf617f1a9"></script>
<script defer src="_static/scripts/pydata-sphinx-theme.js?digest=90905a2f556bf617f1a9"></script>

  <footer class="bd-footer">
<div class="bd-footer__inner bd-page-width">
  
    <div class="footer-items__start">
      
        <div class="footer-item">

  <p class="copyright">
    
      © Copyright 2020-2026, Fortran Community.
      <br/>
    
  </p>
</div>
      
        <div class="footer-item">

  <p class="sphinx-version">
    Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 9.1.0.
    <br/>
  </p>
</div>
      
    </div>
  
  
  
    <div class="footer-items__end">
      
        <div class="footer-item">
<p class="theme-version">
  <!-- # L10n: Setting the PST URL as an argument as this does not need to be localized -->
  Built with the <a href="https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html">PyData Sphinx Theme</a> 0.20.0.
</p></div>
      
    </div>
  
</div>

  </footer>
  </body>
* Connection #0 to host fortran-lang.org left intact
</html>%                                                                                                                macbook@MacBook-Air-MacBook ~ % 
```

---

### A.2. Запит без захисту з'єднання

**Команда:**

```
curl -v http://neverssl.com
```

**Вивід:**

```
* Host neverssl.com:80 was resolved.
* IPv6: (none)
* IPv4: 34.223.124.45
*   Trying 34.223.124.45:80...
* Connected to neverssl.com (34.223.124.45) port 80
> GET / HTTP/1.1
> Host: neverssl.com
> User-Agent: curl/8.7.1
> Accept: */*
> 
* Request completely sent off
< HTTP/1.1 200 OK
< Date: Wed, 09 Sep 2026 08:47:34 GMT
< Server: Apache/2.4.66 ()
< Upgrade: h2,h2c
< Connection: Upgrade
< Last-Modified: Wed, 29 Jun 2022 00:23:33 GMT
< ETag: "f79-5e28b29d38e93"
< Accept-Ranges: bytes
< Content-Length: 3961
< Vary: Accept-Encoding
< Content-Type: text/html; charset=UTF-8
< 
<html>
	<head>
		<title>NeverSSL - Connecting ... </title>
		<style>
		body {
			font-family: Montserrat, helvetica, arial, sans-serif;
			font-size: 16x;
			color: #444444;
			margin: 0;
		}
		h2 {
			font-weight: 700;
			font-size: 1.6em;
			margin-top: 30px;
		}
		p {
			line-height: 1.6em;
		}
		.container {
			max-width: 650px;
			margin: 20px auto 20px auto;
			padding-left: 15px;
			padding-right: 15px
		}
		.header {
			background-color: #42C0FD;
			color: #FFFFFF;
			padding: 10px 0 10px 0;
			font-size: 2.2em;
		}
		.notice {
			background-color: red;
			color: white;
			padding: 10px 0 10px 0;
			font-size: 1.25em;
			animation: flash 4s infinite;
		}
		@keyframes flash {
		0% {
			background-color: red;
		}
		50% {
			background-color: #AA0000;
		}
		0% {
			background-color: red;
		}
		}
		<!-- CSS from Mark Webster https://gist.github.com/markcwebster/9bdf30655cdd5279bad13993ac87c85d -->
		</style>

		<script>
			var adjectives = [ 'cool' , 'calm' , 'relaxed', 'soothing', 'serene', 'slow',
							'beautiful', 'wonderful', 'wonderous', 'fun', 'good',
							'glowing', 'inner', 'grand', 'majestic', 'astounding',
							'fine', 'splendid', 'transcendent', 'sublime', 'whole',
							'unique', 'old', 'young', 'fresh', 'clear', 'shiny',
							'shining', 'lush', 'quiet', 'bright', 'silver' ];

			var nouns =	  [ 'day', 'dawn', 'peace', 'smile', 'love', 'zen', 'laugh',
							'yawn', 'poem', 'song', 'joke', 'verse', 'kiss', 'sunrise',
							'sunset', 'eclipse', 'moon', 'rainbow', 'rain', 'plan',
							'play', 'chart', 'birds', 'stars', 'pathway', 'secret',
							'treasure', 'melody', 'magic', 'spell', 'light', 'morning'];

			var prefix =
					// Choose 3 zen adjectives
					adjectives.sort(function(){return 0.5-Math.random()}).slice(-3).join('')
					+
					// Coupled with a zen noun
					nouns.sort(function(){return 0.5-Math.random()}).slice(-1).join('');
			window.location.href = 'http://' + prefix + '.neverssl.com/online';
		</script>
	</head>
	<body>
	<noscript>
		<div class="notice">
			<div class="container">
				⚠️ JavaScript appears to be disabled. NeverSSL's cache-busting works better if you enable JavaScript for <code>neverssl.com</code>.
			</div>
		</div>
	</noscript>
	<div class="header">
		<div class="container">
		<h1>NeverSSL</h1>
		</div>
	</div>
	<div class="content">
	<div class="container">

	<h1 id="status"></h1>
	<script>document.querySelector("#status").textContent = "Connecting ...";</script>
	<noscript>

		<h2>What?</h2>
		<p>This website is for when you try to open Facebook, Google, Amazon, etc
		on a wifi network, and nothing happens. Type "http://neverssl.com"
		into your browser's url bar, and you'll be able to log on.</p>

		<h2>How?</h2>
		<p>neverssl.com will never use SSL (also known as TLS). No
		encryption, no strong authentication, no <a
		href="https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security">HSTS</a>,
		no HTTP/2.0, just plain old unencrypted HTTP and forever stuck in the dark
		ages of internet security.</p>

		<h2>Why?</h2>
		<p>Normally, that's a bad idea. You should always use SSL and secure
		encryption when possible. In fact, it's such a bad idea that most websites
		are now using https by default.</p>

		<p>And that's great, but it also means that if you're relying on
		poorly-behaved wifi networks, it can be hard to get online.  Secure
		browsers and websites using https make it impossible for those wifi
		networks to send you to a login or payment page. Basically, those networks
		can't tap into your connection just like attackers can't. Modern browsers
		are so good that they can remember when a website supports encryption and
		even if you type in the website name, they'll use https.</p>

		<p>And if the network never redirects you to this page, well as you can
		see, you're not missing much.</p>

        <a href="https://twitter.com/neverssl">Follow @neverssl</a>

	</noscript>

	</div>
	</div>

	</body>
</html>
* Connection #0 to host neverssl.com left intact
macbook@MacBook-Air-MacBook ~ % 
```

---

### A.3. Запит до служби доменних імен


**Команда (перше виконання):**

```
dig fortran-lang.org
```

**Вивід:**

```
; <<>> DiG 9.10.6 <<>> fortran-lang.org
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 33757
;; flags: qr rd ra ad; QUERY: 1, ANSWER: 4, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;fortran-lang.org.		IN	A

;; ANSWER SECTION:
fortran-lang.org.	12704	IN	A	185.199.108.153
fortran-lang.org.	12704	IN	A	185.199.111.153
fortran-lang.org.	12704	IN	A	185.199.109.153
fortran-lang.org.	12704	IN	A	185.199.110.153

;; Query time: 60 msec
;; SERVER: 192.168.0.1#53(192.168.0.1)
;; WHEN: Wed Sep 09 11:51:07 EEST 2026
;; MSG SIZE  rcvd: 109

macbook@MacBook-Air-MacBook ~ % 
```

**Команда (повторне виконання через 5–7 хвилин):**

```
dig fortran-lang.org
```

**Вивід:**

```
; <<>> DiG 9.10.6 <<>> fortran-lang.org
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 42636
;; flags: qr rd ra ad; QUERY: 1, ANSWER: 4, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;fortran-lang.org.		IN	A

;; ANSWER SECTION:
fortran-lang.org.	12145	IN	A	185.199.108.153
fortran-lang.org.	12145	IN	A	185.199.111.153
fortran-lang.org.	12145	IN	A	185.199.109.153
fortran-lang.org.	12145	IN	A	185.199.110.153

;; Query time: 25 msec
;; SERVER: 192.168.0.1#53(192.168.0.1)
;; WHEN: Wed Sep 09 12:00:26 EEST 2026
;; MSG SIZE  rcvd: 109

macbook@MacBook-Air-MacBook ~ %
```

**Зафіксовані значення:**

| Параметр | Перше виконання | Повторне виконання |
|---|---|---|
| Час виконання (год:хв) | 11:51:07| 12:00:26|
| IP-адреса | 185.199.108.153| 185.199.108.153|
| Значення TTL | 12704| 12145|

> Якщо друге значення TTL виявилося більшим за перше — це нормально: кеш резолвера встиг оновитися. Зафіксуйте як є.

---

### A.4. Контрольний ресурс

**Команда:**

```
curl -v https://google.com
```

**Вивід:**

```
* Host google.com:443 was resolved.
* IPv6: (none)
* IPv4: 142.250.120.100, 142.250.120.113, 142.250.120.139, 142.250.120.138, 142.250.120.101, 142.250.120.102
*   Trying 142.250.120.100:443...
* Connected to google.com (142.250.120.100) port 443
* ALPN: curl offers h2,http/1.1
* (304) (OUT), TLS handshake, Client hello (1):
*  CAfile: /etc/ssl/cert.pem
*  CApath: none
* (304) (IN), TLS handshake, Server hello (2):
* (304) (IN), TLS handshake, Unknown (8):
* (304) (IN), TLS handshake, Certificate (11):
* (304) (IN), TLS handshake, CERT verify (15):
* (304) (IN), TLS handshake, Finished (20):
* (304) (OUT), TLS handshake, Finished (20):
* SSL connection using TLSv1.3 / AEAD-CHACHA20-POLY1305-SHA256 / [blank] / UNDEF
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=*.google.com
*  start date: Aug 10 08:37:42 2026 GMT
*  expire date: Nov  2 08:37:41 2026 GMT
*  subjectAltName: host "google.com" matched cert's "google.com"
*  issuer: C=US; O=Google Trust Services; CN=WE2
*  SSL certificate verify ok.
* using HTTP/2
* [HTTP/2] [1] OPENED stream for https://google.com/
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: google.com]
* [HTTP/2] [1] [:path: /]
* [HTTP/2] [1] [user-agent: curl/8.7.1]
* [HTTP/2] [1] [accept: */*]
> GET / HTTP/2
> Host: google.com
> User-Agent: curl/8.7.1
> Accept: */*
> 
* Request completely sent off
< HTTP/2 301 
< location: https://www.google.com/
< content-type: text/html; charset=UTF-8
< content-security-policy-report-only: object-src 'none';base-uri 'self';script-src 'nonce-rQBtZmKG-jTvczICNqPSKw' 'strict-dynamic' 'report-sample' 'unsafe-eval' 'unsafe-inline' https: http:;report-uri https://csp.withgoogle.com/csp/gws/other-hp
< date: Wed, 09 Sep 2026 08:54:56 GMT
< expires: Fri, 09 Oct 2026 08:54:56 GMT
< cache-control: public, max-age=2592000
< server: gws
< content-length: 220
< x-xss-protection: 0
< x-frame-options: SAMEORIGIN
< alt-svc: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000
< 
<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">
<TITLE>301 Moved</TITLE></HEAD><BODY>
<H1>301 Moved</H1>
The document has moved
<A HREF="https://www.google.com/">here</A>.
</BODY></HTML>
* Connection #0 to host google.com left intact
macbook@MacBook-Air-MacBook ~ % 
```

---

### A.5. Ресурси з некоректною конфігурацією сертифіката

**Випадок 1**

```
curl -v https://expired.badssl.com
```

```
* Host expired.badssl.com:443 was resolved.
* IPv6: (none)
* IPv4: 104.154.89.105
*   Trying 104.154.89.105:443...
* Connected to expired.badssl.com (104.154.89.105) port 443
* ALPN: curl offers h2,http/1.1
* (304) (OUT), TLS handshake, Client hello (1):
*  CAfile: /etc/ssl/cert.pem
*  CApath: none
* (304) (IN), TLS handshake, Server hello (2):
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (OUT), TLS alert, certificate expired (557):
* SSL certificate problem: certificate has expired
* Closing connection
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (OUT), TLS alert, certificate expired (557):
curl: (60) SSL certificate problem: certificate has expired
More details here: https://curl.se/docs/sslcerts.html

curl failed to verify the legitimacy of the server and therefore could not
establish a secure connection to it. To learn more about this situation and
how to fix it, please visit the web page mentioned above.
macbook@MacBook-Air-MacBook ~ % 
```

**Випадок 2**

```
curl -v https://wrong.host.badssl.com
```

```
* Host wrong.host.badssl.com:443 was resolved.
* IPv6: (none)
* IPv4: 104.154.89.105
*   Trying 104.154.89.105:443...
* Connected to wrong.host.badssl.com (104.154.89.105) port 443
* ALPN: curl offers h2,http/1.1
* (304) (OUT), TLS handshake, Client hello (1):
*  CAfile: /etc/ssl/cert.pem
*  CApath: none
* (304) (IN), TLS handshake, Server hello (2):
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (IN), TLS handshake, Server key exchange (12):
* TLSv1.2 (IN), TLS handshake, Server finished (14):
* TLSv1.2 (OUT), TLS handshake, Client key exchange (16):
* TLSv1.2 (OUT), TLS change cipher, Change cipher spec (1):
* TLSv1.2 (OUT), TLS handshake, Finished (20):
* TLSv1.2 (IN), TLS change cipher, Change cipher spec (1):
* TLSv1.2 (IN), TLS handshake, Finished (20):
* SSL connection using TLSv1.2 / ECDHE-RSA-AES128-GCM-SHA256 / [blank] / UNDEF
* ALPN: server accepted http/1.1
* Server certificate:
*  subject: CN=*.badssl.com
*  start date: Jul 28 20:03:02 2026 GMT
*  expire date: Oct 26 20:03:01 2026 GMT
*  subjectAltName does not match host name wrong.host.badssl.com
* SSL: no alternative certificate subject name matches target host name 'wrong.host.badssl.com'
* Closing connection
* TLSv1.2 (OUT), TLS alert, close notify (256):
curl: (60) SSL: no alternative certificate subject name matches target host name 'wrong.host.badssl.com'
More details here: https://curl.se/docs/sslcerts.html

curl failed to verify the legitimacy of the server and therefore could not
establish a secure connection to it. To learn more about this situation and
how to fix it, please visit the web page mentioned above.
macbook@MacBook-Air-MacBook ~ % 
```

**Випадок 3**

```
curl -v https://self-signed.badssl.com
```

```
* Host self-signed.badssl.com:443 was resolved.
* IPv6: (none)
* IPv4: 104.154.89.105
*   Trying 104.154.89.105:443...
* Connected to self-signed.badssl.com (104.154.89.105) port 443
* ALPN: curl offers h2,http/1.1
* (304) (OUT), TLS handshake, Client hello (1):
*  CAfile: /etc/ssl/cert.pem
*  CApath: none
* (304) (IN), TLS handshake, Server hello (2):
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (OUT), TLS alert, unknown CA (560):
* SSL certificate problem: self signed certificate
* Closing connection
* TLSv1.2 (IN), TLS handshake, Certificate (11):
* TLSv1.2 (OUT), TLS alert, unknown CA (560):
curl: (60) SSL certificate problem: self signed certificate
More details here: https://curl.se/docs/sslcerts.html

curl failed to verify the legitimacy of the server and therefore could not
establish a secure connection to it. To learn more about this situation and
how to fix it, please visit the web page mentioned above.
macbook@MacBook-Air-MacBook ~ %
```

> Якщо використано альтернативний спосіб із параметром `--resolve` — зазначити це та навести фактичну команду.

---

## Частина B. Власна модель рівнів

**Кількість виділених груп:** ___

| № | Назва групи (власне формулювання) | Рядки виводу, віднесені до групи | Обґрунтування |
|---|---|---|---|
| 1 | Результат | <code>&lt;HTML&gt;&lt;HEAD&gt;&lt;meta http-equiv="content-type" content="text/html;charset=utf-8"&gt;<br>&lt;TITLE&gt;301 Moved&lt;/TITLE&gt;&lt;/HEAD&gt;&lt;BODY&gt;<br>&lt;/BODY&gt;&lt;/HTML&gt;<br>&lt;!DOCTYPE html&gt;</code> | Готовий код і текст сторінки, який бачить користувач |
| 2 | HTTP/HTTPS (Запит і відповідь) | <code>&gt; GET / HTTP/2<br>&gt; Host: google.com<br>&lt; HTTP/2 301<br>&lt; location: https://www.google.com/</code> | Обмін команд для завантаження сторінки |
| 3 | TLS/SSL (Перевірка сертифікатів та шифрування) | <code>* TLSv1.2 (IN), TLS handshake, Certificate (11):<br>* (304) (OUT), TLS handshake, Client hello (1):<br>*   CAfile: /etc/ssl/cert.pem<br>*   CApath: none</code> | Перевірка сертифікату сайту та захист даних |
| 4 | DNS (Перекладання в IP-адресу) | <code>* Host google.com:443 was resolved.<br>* IPv6: (none)<br>* IPv4: 142.250.120.100, 142.250.120.113, 142.250.120.139, 142.250.120.138, 142.250.120.101, 142.250.120.102<br>fortran-lang.org. 12145 IN A 185.199.108.153</code> | Перекладає зрозуміле доменне ім'я в числову IP-адресу |
| 5 | Порти (Підключення до сервера) | <code>*   Trying 104.154.89.105:443...<br>* Connected to google.com (142.250.120.100) port 443</code> | Встановлення зв'язку з потрібним портом сервера (Найближчий до апаратного забезпечення) |
*Групи впорядковано від найближчої до користувача (№ 1) до найближчої до апаратного забезпечення. Зайві рядки вилучити, за потреби — додати.*

**Рядки, які не вдалося віднести до жодної групи:**

| Рядок виводу | Причина утруднення |
|---|---|
| ;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 42636|Містить службову інформацію |
| ;; WHEN: Wed Sep 09 12:00:26 EEST 2026|Не є одним із етапів,а просто описує час виконання запиту |


---

## Контрольні питання

**1. Скільки рядків діагностичного виводу передує отриманню даних сторінки (завдання A.1)?**

> 92 рядків діагностичного виводу передує отриманню даних сторінки

**2. Які рядки наявні у виводі A.1 і відсутні у виводі A.2? Чим це зумовлено?**

> У виводі A.1 наявні такі рядки:"* SSL certificate verify ok". Вони є відсутніми у A.2 тому що запит виконується за незахищеним протоколом 

**3. Звідки у виводі з'явилося значення `443`, якщо його не було вказано в адресі?**

> 443 це порт за замовчуванням для безпечного з'єднання HTTPS 

**4. Як змінилося значення TTL між двома запитами (A.3)? Що означає це число?**

>  Значення TTL між двома запитами (A.3) зменшилося на 559 секунд.Показує скільки часу IP-адреса ще зберігатиметься в пам'яті DNS

**5. Чим відрізняються між собою три причини помилок із завдання A.5? Сформулювати кожну однією фразою.**

| Випадок | Причина недовіри |
|---|---|
| `expired` | Протермінований |
| `wrong.host` | Невідповідність|
| `self-signed` |Самопідписаний |

**6. Три рядки з власних виводів, про які не йшлося на лекції 1:**

| № | Рядок виводу | Джерело (номер завдання) |
|---|---|---|
| 1 | < ETag: "f79-5e28b29d38e93"|A.2 |
| 2 | < Vary: Accept-Encoding|A.1 |
| 3 | * ALPN: server accepted h2|A.4 |

*Пояснення до цих рядків не потрібне.*

---

## Висновки

*150–300 слів. Спиратися на власні спостереження, а не на матеріал лекції.*

**D.1. Що виявилося неочевидним або несподіваним**

*Назвати конкретно, з посиланням на рядок виводу.*

> Несподіваним виявилося те, що при виконанні команди curl -v http://neverssl.com вивід у терміналі з'явився не одразу. Після рядка *   Trying 34.223.124.45:80... сталася затримка приблизно на 10 секунд, і текст завис. Через це я спочатку навіть не скопіювала вивід повністю. 

**D.2. Чому саме така кількість груп у частині B**

*На якій підставі ухвалено рішення. Що змусило б його змінити.*

> На таку кількість груп мене наштовхнув слайд 6 з лекції №1, як і на типи груп

**D.3. Питання, яке залишилося без відповіді**

> На слайді 16 лекції №1 було показано, що дані передаються за MAC-адресою роутера. Чому тоді у виводі curl ми бачимо тільки IP-адресу сервера і зовсім не бачимо MAC-адреси? 

---

## Використання штучного інтелекту

*Розділ обов'язковий. Заповнюється незалежно від того, чи використовувався ШІ. Детальні вимоги — у документі «Політика використання технологій штучного інтелекту».*

**Факт використання:** використано 
**Установлений рівень для цієї роботи:** Р3 — ШІ як співвиконавець

**Фактичний рівень використання:** Р2

### Використані системи

| Система | Версія або модель | Період використання |
|---|---|---|
| Gemini|Gemini 3.6 Flash | 09.09.2026|

### Промпти

*Наводити дослівно, у тому вигляді, у якому запит було надано системі. Переказ не приймається.*

| № | Розділ роботи | Текст промпта |
|---|---|---|
| 1 | Частина B(Рядки, які не вдалося віднести до жодної групи а точніше причини утруднення)| Цей рядок ж  ;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 42636 містить службову інформацію?|
| 2 |Контрольні питання№1 | Поясни це питання більш зрозуміліше
Скільки рядків діагностичного виводу передує отриманню даних сторінки (завдання A.1)|
| 3 |Таблиці з відповідями | У мене тут з'їхала таблиця,як її виправити?|

### Дії з отриманим результатом

| № промпта | Що перевірено | Що змінено | Що відхилено і чому |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

### Підтвердження

Підтверджую, що всі наведені в цьому звіті виводи команд отримано мною особисто внаслідок фактичного виконання відповідних дій, а відомості цього розділу є повними та достовірними.

> Виводи `curl`, `dig` та інші артефакти не можуть бути згенеровані. Це стосується будь-якого рівня використання ШІ.

---

## Примітки виконавця

*(необов'язковий розділ: що не спрацювало, які команди довелося змінити, які виникли труднощі)*

> 

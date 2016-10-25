<!DOCTYPE html>
<html><head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
<title>React Native | A framework for building native apps using React</title>
<meta name="viewport" content="width=device-width">
<meta property="og:title" content="React Native | A framework for building native apps using React">
<meta property="og:type" content="website">
<meta property="og:url" content="http://facebook.github.io/react-native/index.html">
<meta property="og:image" content="http://facebook.github.io/react-native/img/opengraph.png?2">
<meta property="og:description" content="A framework for building native apps using React"><base href="/react-native/">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/docsearch.js/1/docsearch.min.css">
<link rel="shortcut icon" href="img/favicon.png?2">
<link rel="stylesheet" href="css/react-native.css">
<script type="text/javascript" src="//use.typekit.net/vqa1hcx.js"></script>
<script type="text/javascript">try{Typekit.load();}catch(e){}</script>
</head>
<body>
<div class="container">
<div class="nav-main"><div class="wrap"><a class="nav-home" href=""><img src="img/header_logo.png">React Native</a><a class="nav-version" href="/react-native/versions.html">0.33</a><div class="nav-site-wrapper"><ul class="nav-site nav-site-internal"><li><a href="docs/getting-started.html" class="" data-target=".nav-docs">Docs</a></li><li><a href="support.html" class="">Support</a></li><li><a href="showcase.html" class="">Showcase</a></li><li><a href="blog/" class="">Blog</a></li></ul><div class="algolia-search-wrapper"><input id="algolia-doc-search" tabindex="0" type="text" placeholder="Search docs..."></div><ul class="nav-site nav-site-external"><li><a href="https://github.com/facebook/react-native" class="">GitHub</a></li><li><a href="http://facebook.github.io/react" class="">React</a></li></ul></div></div></div><div class="hero"><div class="wrap"><div class="text"><strong>React Native</strong></div><div class="minitext">Learn once, write anywhere: Build mobile apps with React</div></div><div class="buttons-unit"><a href="docs/getting-started.html#content" class="button">Get started with React Native</a></div></div><section class="content wrap"><div style="margin:40px auto;max-width:800px;"><h2>Build Native Mobile Apps using JavaScript and React</h2><p>React Native lets you build mobile apps using only JavaScript. It uses the same design as React, letting you compose a rich mobile UI from declarative components.</p><div class="prism language-javascript">import React<span class="token punctuation">,</span> <span class="token punctuation">{</span> Component <span class="token punctuation">}</span> from <span class="token string">&#x27;react&#x27;</span><span class="token punctuation">;</span>
import <span class="token punctuation">{</span> Text<span class="token punctuation">,</span> View <span class="token punctuation">}</span> from <span class="token string">&#x27;react-native&#x27;</span><span class="token punctuation">;</span>

class <span class="token class-name">WhyReactNativeIsSoGreat</span> extends <span class="token class-name">Component</span> <span class="token punctuation">{</span>
  <span class="token function">render<span class="token punctuation">(</span></span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token keyword">return</span> <span class="token punctuation">(</span>
      &lt;View<span class="token operator">&gt;</span>
        &lt;Text<span class="token operator">&gt;</span>
          If you like React on the web<span class="token punctuation">,</span> you&#x27;ll like React Native<span class="token punctuation">.</span>
        &lt;<span class="token operator">/</span>Text<span class="token operator">&gt;</span>
        &lt;Text<span class="token operator">&gt;</span>
          You just use native components like <span class="token string">&#x27;View&#x27;</span> and <span class="token string">&#x27;Text&#x27;</span><span class="token punctuation">,</span>
          instead of web components like <span class="token string">&#x27;div&#x27;</span> and <span class="token string">&#x27;span&#x27;</span><span class="token punctuation">.</span>
        &lt;<span class="token operator">/</span>Text<span class="token operator">&gt;</span>
      &lt;<span class="token operator">/</span>View<span class="token operator">&gt;</span>
    <span class="token punctuation">)</span><span class="token punctuation">;</span>
  <span class="token punctuation">}</span>
<span class="token punctuation">}</span></div><h2>A React Native App is a Real Mobile App</h2><p>With React Native, you don&#x27;t build a “mobile web app”, an “HTML5 app”, or a “hybrid app”. You build a real mobile app that&#x27;s indistinguishable from an app built using Objective-C or Java. React Native uses the same fundamental UI building blocks as regular iOS and Android apps. You just put those building blocks together using JavaScript and React.</p><div class="prism language-javascript">import React<span class="token punctuation">,</span> <span class="token punctuation">{</span> Component <span class="token punctuation">}</span> from <span class="token string">&#x27;react&#x27;</span><span class="token punctuation">;</span>
import <span class="token punctuation">{</span> Image<span class="token punctuation">,</span> ScrollView<span class="token punctuation">,</span> Text <span class="token punctuation">}</span> from <span class="token string">&#x27;react-native&#x27;</span><span class="token punctuation">;</span>

class <span class="token class-name">AwkwardScrollingImageWithText</span> extends <span class="token class-name">Component</span> <span class="token punctuation">{</span>
  <span class="token function">render<span class="token punctuation">(</span></span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token keyword">return</span> <span class="token punctuation">(</span>
      &lt;ScrollView<span class="token operator">&gt;</span>
        &lt;Image source<span class="token operator">=</span><span class="token punctuation">{</span><span class="token punctuation">{</span>uri<span class="token punctuation">:</span> <span class="token string">&#x27;https://i.chzbgr.com/full/7345954048/h7E2C65F9/&#x27;</span><span class="token punctuation">}</span><span class="token punctuation">}</span> <span class="token operator">/</span><span class="token operator">&gt;</span>
        &lt;Text<span class="token operator">&gt;</span>
          On iOS<span class="token punctuation">,</span> a React Native ScrollView uses a native UIScrollView<span class="token punctuation">.</span>
          On Android<span class="token punctuation">,</span> it uses a native ScrollView<span class="token punctuation">.</span>

          On iOS<span class="token punctuation">,</span> a React Native Image uses a native UIImageView<span class="token punctuation">.</span>
          On Android<span class="token punctuation">,</span> it uses a native ImageView<span class="token punctuation">.</span>

          React Native wraps the fundamental native components<span class="token punctuation">,</span> giving you
          the performance of a native app<span class="token punctuation">,</span> plus the clean design of React<span class="token punctuation">.</span>
        &lt;<span class="token operator">/</span>Text<span class="token operator">&gt;</span>
      &lt;<span class="token operator">/</span>ScrollView<span class="token operator">&gt;</span>
    <span class="token punctuation">)</span><span class="token punctuation">;</span>
  <span class="token punctuation">}</span>
<span class="token punctuation">}</span></div><h2>Don&#x27;t Waste Time Recompiling</h2><p>React Native lets you build your app faster. Instead of recompiling, you can reload your app instantly. With hot reloading, you can even run new code while retaining your application state. Give it a try - it&#x27;s a magical experience.</p><br><img src="https://media.giphy.com/media/13WZniThXy0hSE/giphy.gif"><h2>Use Native Code When You Need To</h2><p>React Native combines smoothly with components written in Objective-C, Java, or Swift. It&#x27;s simple to drop down to native code if you need to optimize a few aspects of your application. It&#x27;s also easy to build part of your app in React Native, and part of your app using native code directly - that&#x27;s how the Facebook app works.</p><div class="prism language-javascript">import React<span class="token punctuation">,</span> <span class="token punctuation">{</span> Component <span class="token punctuation">}</span> from <span class="token string">&#x27;react&#x27;</span><span class="token punctuation">;</span>
import <span class="token punctuation">{</span> Text<span class="token punctuation">,</span> View <span class="token punctuation">}</span> from <span class="token string">&#x27;react-native&#x27;</span><span class="token punctuation">;</span>
import <span class="token punctuation">{</span> TheGreatestComponentInTheWorld <span class="token punctuation">}</span> from <span class="token string">&#x27;./your-native-code&#x27;</span><span class="token punctuation">;</span>

class <span class="token class-name">SomethingFast</span> extends <span class="token class-name">Component</span> <span class="token punctuation">{</span>
  <span class="token function">render<span class="token punctuation">(</span></span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token keyword">return</span> <span class="token punctuation">(</span>
      &lt;View<span class="token operator">&gt;</span>
        &lt;TheGreatestComponentInTheWorld <span class="token operator">/</span><span class="token operator">&gt;</span>
        &lt;Text<span class="token operator">&gt;</span>
          TheGreatestComponentInTheWorld could use native Objective<span class="token operator">-</span>C<span class="token punctuation">,</span>
          Java<span class="token punctuation">,</span> or Swift <span class="token operator">-</span> the product development process is the same<span class="token punctuation">.</span>
        &lt;<span class="token operator">/</span>Text<span class="token operator">&gt;</span>
      &lt;<span class="token operator">/</span>View<span class="token operator">&gt;</span>
    <span class="token punctuation">)</span><span class="token punctuation">;</span>
  <span class="token punctuation">}</span>
<span class="token punctuation">}</span></div></div><section class="home-bottom-section"><div class="buttons-unit"><a href="docs/getting-started.html#content" class="button">Get started with React Native</a></div></section></section>

<footer class="wrap">
<div class="center">© 2016 Facebook Inc.</div>
</footer>
</div>
<div id="fb-root"></div>
<script type="text/javascript" src="https://cdn.jsdelivr.net/docsearch.js/1/docsearch.min.js"></script>
<script>
            
        (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
        (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
        m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
        })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

        ga('create', 'UA-86267577-1', 'react-native.webgeeker.xyz');
        ga('send', 'pageview');

            !function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)
            ){js=d.createElement(s);js.id=id;js.src="https://platform.twitter.com/widgets.js";
            fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");

            docsearch({
              apiKey: '2c98749b4a1e588efec53b2acec13025',
              indexName: 'react-native-versions',
              inputSelector: '#algolia-doc-search',
              algoliaOptions: { facetFilters: [ "tags:0.33" ], hitsPerPage: 5 }
            });
          </script>
          <script src="js/scripts.js"></script>
</body>
</html>

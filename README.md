<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="google-site-verification" content="xBT4GhYoi5qRD5tr338pgPM5OWHHIDR6mNg1a3euekI" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="二轮车上写游记的厚厚同学">
    <meta name="keywords"  content="游记">
    <meta name="theme-color" content="#000000">
    
    <title>人生一场旅行</title>

    <!-- Web App Manifest -->
    <link rel="manifest" href="/pwa/manifest.json">

    <!-- Favicon -->
    <link rel="shortcut icon" href="/img/favicon.ico">
    
    <!-- Canonical URL -->
    <link rel="canonical" href="/">

    <!-- Bootstrap Core CSS -->
    <link rel="stylesheet" href="/css/bootstrap.min.css">

    <!-- Custom CSS -->
    <link rel="stylesheet" href="/css/hux-blog.min.css">

    <!-- Pygments Github CSS -->
    <link rel="stylesheet" href="/css/syntax.css">

    <!-- Custom Fonts -->
    <!-- <link href="http://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css" rel="stylesheet" type="text/css"> -->
    <!-- Hux change font-awesome CDN to qiniu -->
    <link href="//cdnjs.cloudflare.com/ajax/libs/font-awesome/4.6.3/css/font-awesome.min.css" rel="stylesheet" type="text/css">


    <!-- Hux Delete, sad but pending in China
    <link href='http://fonts.googleapis.com/css?family=Lora:400,700,400italic,700italic' rel='stylesheet' type='text/css'>
    <link href='http://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800' rel='stylesheet' type='text/
    css'>
    -->


    <!-- HTML5 Shim and Respond.js IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
        <script src="https://oss.maxcdn.com/libs/html5shiv/3.7.0/html5shiv.js"></script>
        <script src="https://oss.maxcdn.com/libs/respond.js/1.4.2/respond.min.js"></script>
    <![endif]-->

    <!-- ga & ba script hoook -->
    <script></script>
</head>


<!-- hack iOS CSS :active style -->
<body ontouchstart="">

    <!-- Navigation -->
<nav class="navbar navbar-default navbar-custom navbar-fixed-top">
    <div class="container-fluid">
        <!-- Brand and toggle get grouped for better mobile display -->
        <div class="navbar-header page-scroll">
            <button type="button" class="navbar-toggle">
                <span class="sr-only">Toggle navigation</span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
            </button>
            <a class="navbar-brand" href="/">人生一场旅行</a>
        </div>

        <!-- Collect the nav links, forms, and other content for toggling -->
        <div id="huxblog_navbar">
            <div class="navbar-collapse">
                <ul class="nav navbar-nav navbar-right">
                    <li>
                        <a href="/">Home</a>
                    </li>
                    
                    <li>
                        <a href="/about/">About</a>
                    </li>
                    
                    <li>
                        <a href="/portfolio/">Portfolio</a>
                    </li>
                    
                    <li>
                        <a href="/tags/">Tags</a>
                    </li>
                    
                </ul>
            </div>
        </div>
        <!-- /.navbar-collapse -->
    </div>
    <!-- /.container -->
</nav>
<script>
    // Drop Bootstarp low-performance Navbar
    // Use customize navbar with high-quality material design animation
    // in high-perf jank-free CSS3 implementation
    var $body   = document.body;
    var $toggle = document.querySelector('.navbar-toggle');
    var $navbar = document.querySelector('#huxblog_navbar');
    var $collapse = document.querySelector('.navbar-collapse');

    var __HuxNav__ = {
        close: function(){
            $navbar.className = " ";
            // wait until animation end.
            setTimeout(function(){
                // prevent frequently toggle
                if($navbar.className.indexOf('in') < 0) {
                    $collapse.style.height = "0px"
                }
            },400)
        },
        open: function(){
            $collapse.style.height = "auto"
            $navbar.className += " in";
        }
    }

    // Bind Event
    $toggle.addEventListener('click', function(e){
        if ($navbar.className.indexOf('in') > 0) {
            __HuxNav__.close()
        }else{
            __HuxNav__.open()
        }
    })

    /**
     * Since Fastclick is used to delegate 'touchstart' globally
     * to hack 300ms delay in iOS by performing a fake 'click',
     * Using 'e.stopPropagation' to stop 'touchstart' event from 
     * $toggle/$collapse will break global delegation.
     * 
     * Instead, we use a 'e.target' filter to prevent handler
     * added to document close HuxNav.  
     *
     * Also, we use 'click' instead of 'touchstart' as compromise
     */
    document.addEventListener('click', function(e){
        if(e.target == $toggle) return;
        if(e.target.className == 'icon-bar') return;
        __HuxNav__.close();
    })
</script>


    <!-- Page Header -->
<header class="intro-header" style="background-image: url('/img/home-bg.jpg')">
    <div class="container">
        <div class="row">
            <div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1 ">
                <div class="site-heading">
                    <h1>人生一场旅行</h1>
                    <!--<hr class="small">-->
                    <span class="subheading">总有属于你的远方值得追寻</span>
                </div>
            </div>
        </div>
    </div>
</header>

<!-- Main Content -->
<div class="container">
	<div class="row">
        

<!-- USE SIDEBAR -->
    <!-- PostList Container -->
    		<div class="
                col-lg-8 col-lg-offset-1
                col-md-8 col-md-offset-1
                col-sm-12
                col-xs-12
                postlist-container
            ">
    			
<div class="post-preview">
    <a href="/ios/2018/03/23/iosfeedback/">
        <h2 class="post-title">
            【iOS程序员面试笔试宝典答疑帖】
        </h2>
        
        <div class="post-content-preview">
            关于书中的问题欢迎批评指正，关于iOS技术问题也可以通过邮箱和我们交流探讨。祝iOS爱好者和学习者们都能不断进步，更上一层楼吧！一起加油！

联系反馈邮箱：【919575700艾特扣扣dotCOM】


===================纠错补充分割线=====================

3.6.2	Swift和Objective-C如何互调？

解释和纠错点：



其中的Sw...
        </div>
    </a>
    <p class="post-meta">
        Posted by 人生一场旅行 on March 23, 2018
    </p>
</div>
<hr>


<!-- Pager -->


    		</div>
    <!-- Sidebar Container -->
            <div class="
                col-lg-3 col-lg-offset-0
                col-md-3 col-md-offset-0
                col-sm-12
                col-xs-12
                sidebar-container
            ">
                <!-- Featured Tags -->
                
                <section>
                    <hr class="hidden-sm hidden-xs">
                    <h5><a href="/tags/">FEATURED TAGS</a></h5>
                    <div class="tags">
                        
                            
                        
                    </div>
                </section>
                

                <!-- Short About -->
                <section class="visible-md visible-lg">
                    <hr><h5><a href="/about/">ABOUT ME</a></h5>
                    <div class="short-about">
                        
                            <img src="/img/avatar-jxh.jpg" />
                        
                        
                            <p>人生一场旅行<br>甜苦皆在途中</p>
                        
                        <!-- SNS Link -->
                        <ul class="list-inline">
                            
                            
                            
                            <li>
                                <a target="_blank" href="https://www.zhihu.com/people/Jiangxh1992@HKU">
                                    <span class="fa-stack fa-lg">
                                        <i class="fa fa-circle fa-stack-2x"></i>
                                        <i class="fa  fa-stack-1x fa-inverse">知</i>
                                    </span>
                                </a>
                            </li>
                            
                            
                            
                            <li>
                                <a target="_blank" href="https://www.facebook.com/JiangXinhou">
                                    <span class="fa-stack fa-lg">
                                        <i class="fa fa-circle fa-stack-2x"></i>
                                        <i class="fa fa-facebook fa-stack-1x fa-inverse"></i>
                                    </span>
                                </a>
                            </li>
                            
                            
                            <li>
                                <a target="_blank" href="https://github.com/jiangxh1992">
                                    <span class="fa-stack fa-lg">
                                        <i class="fa fa-circle fa-stack-2x"></i>
                                        <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                                    </span>
                                </a>
                            </li>
                            
                            
                            <li>
                                <a target="_blank" href="https://www.linkedin.com/in/信厚-蒋-13745212a?trk=nav_responsive_tab_profile_pic">
                                    <span class="fa-stack fa-lg">
                                        <i class="fa fa-circle fa-stack-2x"></i>
                                        <i class="fa fa-linkedin fa-stack-1x fa-inverse"></i>
                                    </span>
                                </a>
                            </li>
                            
                        </ul>
                    </div>
                </section>
                <!-- Friends Blog -->
                
                <hr>
                <h5>FRIENDS</h5>
                <ul class="list-inline">
                    
                        <li><a href="http://blog.csdn.net/cordova">蒋信厚CSDN</a></li>
                    
                        <li><a href="http://fz0512.com">最好金龟换酒</a></li>
                    
                </ul>
                
    		</div>
        
	</div>
</div>


    <!-- Footer -->
<footer>
    <div class="container">
        <div class="row">
            <div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1">
                <ul class="list-inline text-center">
                    
                    

                    <!-- add Weibo, Zhihu by Hux, add target = "_blank" to <a> by Hux -->
                    
                    <li>
                        <a target="_blank" href="https://www.zhihu.com/people/Jiangxh1992@HKU">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa  fa-stack-1x fa-inverse">知</i>
                            </span>
                        </a>
                    </li>
                    
                    


                    
                    <li>
                        <a target="_blank" href="https://www.facebook.com/JiangXinhou">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa fa-facebook fa-stack-1x fa-inverse"></i>
                            </span>
                        </a>
                    </li>
                    
                    
                    <li>
                        <a target="_blank" href="https://github.com/jiangxh1992">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                            </span>
                        </a>
                    </li>
                    
                    
                    <li>
                        <a target="_blank" href="https://www.linkedin.com/in/信厚-蒋-13745212a?trk=nav_responsive_tab_profile_pic">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa fa-linkedin fa-stack-1x fa-inverse"></i>
                            </span>
                        </a>
                    </li>
                    
                </ul>
                <p class="copyright text-muted">
                    Copyright &copy; 人生一场旅行 2019
                </p>
            </div>
        </div>
    </div>
</footer>

<!-- jQuery -->
<script src="/js/jquery.min.js "></script>

<!-- Bootstrap Core JavaScript -->
<!-- Currently, only navbar scroll-down effect at desktop still depends on this -->
<script src="/js/bootstrap.min.js "></script>

<!-- Custom Theme JavaScript -->
<script src="/js/hux-blog.min.js "></script>

<!-- Service Worker -->

<script src="/js/snackbar.js "></script>
<script src="/js/sw-registration.js "></script>


<!-- async load function -->
<script>
    function async(u, c) {
      var d = document, t = 'script',
          o = d.createElement(t),
          s = d.getElementsByTagName(t)[0];
      o.src = u;
      if (c) { o.addEventListener('load', function (e) { c(null, e); }, false); }
      s.parentNode.insertBefore(o, s);
    }
</script>

<!--
     Because of the native support for backtick-style fenced code blocks
     right within the Markdown is landed in Github Pages,
     From V1.6, There is no need for Highlight.js,
     so Huxblog drops it officially.

     - https://github.com/blog/2100-github-pages-now-faster-and-simpler-with-jekyll-3-0
     - https://help.github.com/articles/creating-and-highlighting-code-blocks/
     - https://github.com/jneen/rouge/wiki/list-of-supported-languages-and-lexers
-->
<!--
    <script>
        async("http://cdn.bootcss.com/highlight.js/8.6/highlight.min.js", function(){
            hljs.initHighlightingOnLoad();
        })
    </script>
    <link href="http://cdn.bootcss.com/highlight.js/8.6/styles/github.min.css" rel="stylesheet">
-->


<!-- jquery.tagcloud.js -->
<script>
    // only load tagcloud.js in tag.html
    if($('#tag_cloud').length !== 0){
        async('/js/jquery.tagcloud.js',function(){
            $.fn.tagcloud.defaults = {
                //size: {start: 1, end: 1, unit: 'em'},
                color: {start: '#bbbbee', end: '#0085a1'},
            };
            $('#tag_cloud a').tagcloud();
        })
    }
</script>

<!--fastClick.js -->
<script>
    async("//cdnjs.cloudflare.com/ajax/libs/fastclick/1.0.6/fastclick.min.js", function(){
        var $nav = document.querySelector("nav");
        if($nav) FastClick.attach($nav);
    })
</script>


<!-- Google Analytics -->

<script>
    // dynamic User by Hux
    var _gaId = 'UA-49627206-1';
    var _gaDomain = 'huangxuan.me';

    // Originial
    (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
    (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
    m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
    })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

    ga('create', _gaId, _gaDomain);
    ga('send', 'pageview');
</script>



<!-- Baidu Tongji -->



<!-- Side Catalog -->



<!-- Multi-Lingual -->




<!-- Image to hack wechat -->
<img src="/img/icon_wechat.png" width="0" height="0" />
<!-- Migrate from head to bottom, no longer block render and still work -->

</body>

</html>

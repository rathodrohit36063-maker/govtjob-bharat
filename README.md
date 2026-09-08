<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>GovtJob India | Government Jobs Portal</title>

<style>
/* =========================
   RESET
========================= */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Inter,Arial,Helvetica,sans-serif;
    background:#f6f8fc;
    color:#182230;
    overflow-x:hidden;
}

a{
    text-decoration:none;
}

button,
input{
    font:inherit;
}


/* =========================
   VARIABLES
========================= */
:root{
    --navy:#102a43;
    --blue:#075985;
    --blue2:#0ea5e9;
    --saffron:#ff9933;
    --green:#138808;
    --white:#ffffff;
    --light:#f6f8fc;
    --text:#182230;
    --muted:#64748b;
    --border:#e2e8f0;
    --shadow:0 15px 40px rgba(15,23,42,.08);
}


/* =========================
   TOP GOVERNMENT STRIP
========================= */
.top-strip{
    background:var(--navy);
    color:white;
    padding:8px 20px;
    font-size:13px;
}

.top-inner{
    max-width:1200px;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.top-right{
    opacity:.85;
}


/* =========================
   NAVBAR
========================= */
.navbar{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(255,255,255,.96);
    backdrop-filter:blur(12px);
    border-bottom:1px solid var(--border);
}

.nav-inner{
    max-width:1200px;
    margin:auto;
    padding:15px 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:20px;
}

.brand{
    display:flex;
    align-items:center;
    gap:12px;
}

.emblem{
    width:46px;
    height:46px;
    border-radius:50%;
    background:linear-gradient(145deg,#ff9933 0 33%,white 33% 66%,#138808 66%);
    display:grid;
    place-items:center;
    border:2px solid #e2e8f0;
    font-size:21px;
}

.brand-text h2{
    font-size:20px;
    color:var(--navy);
}

.brand-text span{
    font-size:11px;
    color:var(--muted);
    letter-spacing:.7px;
}

.nav-links{
    display:flex;
    gap:26px;
    align-items:center;
}

.nav-links a{
    color:#334155;
    font-size:14px;
    font-weight:700;
    transition:.2s;
}

.nav-links a:hover{
    color:var(--blue2);
}

.nav-btn{
    background:var(--navy);
    color:white!important;
    padding:10px 17px;
    border-radius:9px;
}


/* =========================
   HERO
========================= */
.hero{
    position:relative;
    padding:90px 20px 100px;
    background:
        radial-gradient(circle at 10% 20%,rgba(14,165,233,.10),transparent 30%),
        radial-gradient(circle at 90% 30%,rgba(255,153,51,.10),transparent 30%),
        linear-gradient(135deg,#ffffff,#eef6fb);
    overflow:hidden;
}

.hero:before{
    content:"";
    position:absolute;
    width:350px;
    height:350px;
    border:1px solid rgba(7,89,133,.10);
    border-radius:50%;
    right:-100px;
    top:-100px;
}

.hero-content{
    max-width:1000px;
    margin:auto;
    text-align:center;
    position:relative;
    z-index:2;
}

.gov-badge{
    display:inline-flex;
    align-items:center;
    gap:8px;
    padding:9px 16px;
    background:white;
    border:1px solid var(--border);
    border-radius:50px;
    box-shadow:0 5px 20px rgba(0,0,0,.05);
    color:var(--blue);
    font-size:13px;
    font-weight:800;
    margin-bottom:22px;
}

.hero h1{
    font-size:clamp(42px,7vw,72px);
    line-height:1.03;
    letter-spacing:-2px;
    color:var(--navy);
}

.hero h1 span{
    color:var(--blue2);
}

.hero-description{
    max-width:700px;
    margin:22px auto 0;
    color:var(--muted);
    font-size:18px;
    line-height:1.7;
}


/* =========================
   SEARCH
========================= */
.search-wrapper{
    max-width:780px;
    margin:35px auto 0;
}

.search-box{
    display:flex;
    align-items:center;
    background:white;
    padding:7px;
    border:1px solid #dce5ee;
    border-radius:16px;
    box-shadow:var(--shadow);
}

.search-icon{
    padding:0 12px;
    font-size:22px;
}

.search-box input{
    flex:1;
    border:0;
    outline:0;
    padding:17px 8px;
    font-size:16px;
    color:var(--text);
}

.search-box button{
    border:0;
    background:var(--blue);
    color:white;
    padding:15px 27px;
    border-radius:11px;
    cursor:pointer;
    font-weight:800;
    transition:.2s;
}

.search-box button:hover{
    background:#064e72;
    transform:translateY(-1px);
}

.search-hints{
    margin-top:13px;
    color:#64748b;
    font-size:12px;
}


/* =========================
   STATS
========================= */
.stats{
    max-width:1100px;
    margin:-35px auto 0;
    position:relative;
    z-index:5;
    padding:0 20px;
}

.stats-box{
    background:white;
    border:1px solid var(--border);
    border-radius:18px;
    box-shadow:var(--shadow);
    display:grid;
    grid-template-columns:repeat(4,1fr);
    overflow:hidden;
}

.stat{
    padding:25px 15px;
    text-align:center;
    border-right:1px solid var(--border);
}

.stat:last-child{
    border-right:0;
}

.stat-number{
    font-size:29px;
    font-weight:900;
    color:var(--navy);
}

.stat-label{
    margin-top:6px;
    color:var(--muted);
    font-size:13px;
}


/* =========================
   COMMON SECTION
========================= */
.section{
    max-width:1200px;
    margin:auto;
    padding:85px 20px;
}

.section-heading{
    display:flex;
    justify-content:space-between;
    align-items:end;
    gap:20px;
    margin-bottom:35px;
}

.section-heading h2{
    color:var(--navy);
    font-size:34px;
}

.section-heading p{
    color:var(--muted);
    margin-top:8px;
}

.view-all{
    color:var(--blue);
    font-weight:800;
    font-size:14px;
}


/* =========================
   CATEGORY CARDS
========================= */
.category-grid{
    display:grid;
    grid-template-columns:repeat(6,1fr);
    gap:15px;
}

.category-card{
    border:1px solid var(--border);
    background:white;
    border-radius:15px;
    padding:23px 12px;
    text-align:center;
    cursor:pointer;
    transition:.25s;
}

.category-card:hover{
    transform:translateY(-6px);
    box-shadow:var(--shadow);
    border-color:#bae6fd;
}

.category-icon{
    width:52px;
    height:52px;
    margin:auto;
    display:grid;
    place-items:center;
    background:#f0f9ff;
    border-radius:14px;
    font-size:25px;
}

.category-card h3{
    margin-top:13px;
    font-size:15px;
    color:var(--navy);
}

.category-card p{
    color:var(--muted);
    font-size:11px;
    margin-top:5px;
}


/* =========================
   LATEST JOBS
========================= */
.jobs-section{
    background:white;
    border-top:1px solid var(--border);
    border-bottom:1px solid var(--border);
}

.job-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.job-card{
    background:white;
    border:1px solid var(--border);
    border-radius:17px;
    padding:24px;
    transition:.25s;
    position:relative;
    overflow:hidden;
}

.job-card:hover{
    transform:translateY(-5px);
    box-shadow:var(--shadow);
}

.job-card:before{
    content:"";
    position:absolute;
    left:0;
    top:0;
    width:4px;
    height:100%;
    background:var(--saffron);
}

.job-top{
    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:10px;
}

.job-icon{
    width:48px;
    height:48px;
    display:grid;
    place-items:center;
    border-radius:12px;
    background:#eff6ff;
    font-size:23px;
}

.job-status{
    color:#15803d;
    background:#f0fdf4;
    padding:5px 9px;
    border-radius:30px;
    font-size:10px;
    font-weight:900;
}

.job-card h3{
    color:var(--navy);
    margin-top:18px;
    font-size:19px;
}

.job-card p{
    color:var(--muted);
    line-height:1.55;
    margin-top:8px;
    font-size:13px;
}

.job-meta{
    display:flex;
    flex-wrap:wrap;
    gap:7px;
    margin-top:15px;
}

.job-meta span{
    background:#f8fafc;
    border:1px solid #edf2f7;
    padding:5px 8px;
    border-radius:6px;
    color:#64748b;
    font-size:10px;
}

.job-button{
    display:block;
    text-align:center;
    background:var(--navy);
    color:white;
    padding:11px;
    margin-top:19px;
    border-radius:9px;
    font-size:13px;
    font-weight:800;
    transition:.2s;
}

.job-button:hover{
    background:var(--blue);
}


/* =========================
   OFFICIAL PORTALS
========================= */
.portal-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.portal{
    background:#fff;
    border:1px solid var(--border);
    border-radius:15px;
    padding:22px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:15px;
    transition:.2s;
}

.portal:hover{
    box-shadow:var(--shadow);
    transform:translateY(-3px);
}

.portal-left{
    display:flex;
    align-items:center;
    gap:13px;
}

.portal-logo{
    width:45px;
    height:45px;
    border-radius:11px;
    display:grid;
    place-items:center;
    background:#f1f5f9;
    font-size:22px;
}

.portal h3{
    font-size:15px;
    color:var(--navy);
}

.portal p{
    font-size:11px;
    color:var(--muted);
    margin-top:4px;
}

.portal-arrow{
    color:var(--blue);
    font-size:20px;
}


/* =========================
   INFORMATION BANNER
========================= */
.notice{
    max-width:1160px;
    margin:0 auto 80px;
    padding:0 20px;
}

.notice-box{
    background:linear-gradient(120deg,var(--navy),#075985);
    color:white;
    border-radius:20px;
    padding:35px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:30px;
    overflow:hidden;
    position:relative;
}

.notice-box:after{
    content:"🇮🇳";
    position:absolute;
    right:35px;
    font-size:100px;
    opacity:.08;
}

.notice h2{
    font-size:25px;
}

.notice p{
    color:#cbd5e1;
    margin-top:8px;
    line-height:1.6;
    max-width:700px;
    font-size:14px;
}


/* =========================
   FOOTER
========================= */
footer{
    background:#0b1728;
    color:white;
}

.footer-main{
    max-width:1200px;
    margin:auto;
    padding:60px 20px;
    display:grid;
    grid-template-columns:2fr 1fr 1fr 1fr;
    gap:40px;
}

.footer-brand h2{
    font-size:23px;
}

.footer-brand p{
    color:#94a3b8;
    line-height:1.7;
    margin-top:13px;
    max-width:380px;
    font-size:13px;
}

.footer-col h4{
    margin-bottom:16px;
}

.footer-col a{
    display:block;
    color:#94a3b8;
    margin-bottom:11px;
    font-size:13px;
    transition:.2s;
}

.footer-col a:hover{
    color:white;
}

.footer-bottom{
    border-top:1px solid rgba(255,255,255,.08);
    padding:20px;
    text-align:center;
    color:#64748b;
    font-size:11px;
}


/* =========================
   NO RESULT
========================= */
.no-result{
    display:none;
    text-align:center;
    padding:35px;
    color:var(--muted);
}


/* =========================
   ANIMATION
========================= */
@keyframes fadeUp{
    from{
        opacity:0;
        transform:translateY(18px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

.hero-content,
.category-card,
.job-card,
.portal{
    animation:fadeUp .7s ease both;
}


/* =========================
   MOBILE
========================= */
@media(max-width:950px){

    .category-grid{
        grid-template-columns:repeat(3,1fr);
    }

    .job-grid,
    .portal-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .footer-main{
        grid-template-columns:2fr 1fr 1fr;
    }
}

@media(max-width:650px){

    .top-right{
        display:none;
    }

    .top-inner{
        justify-content:center;
    }

    .nav-links{
        display:none;
    }

    .hero{
        padding:65px 15px 80px;
    }

    .hero h1{
        font-size:43px;
        letter-spacing:-1px;
    }

    .hero-description{
        font-size:15px;
    }

    .search-box{
        flex-direction:column;
        padding:8px;
    }

    .search-icon{
        display:none;
    }

    .search-box input{
        width:100%;
        padding:15px;
    }

    .search-box button{
        width:100%;
    }

    .stats{
        margin-top:-25px;
    }

    .stats-box{
        grid-template-columns:repeat(2,1fr);
    }

    .stat:nth-child(2){
        border-right:0;
    }

    .stat:nth-child(-n+2){
        border-bottom:1px solid var(--border);
    }

    .section{
        padding:60px 15px;
    }

    .section-heading{
        display:block;
    }

    .section-heading h2{
        font-size:27px;
    }

    .view-all{
        display:inline-block;
        margin-top:12px;
    }

    .category-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .job-grid,
    .portal-grid{
        grid-template-columns:1fr;
    }

    .notice{
        padding:0 15px;
        margin-bottom:60px;
    }

    .notice-box{
        padding:27px 22px;
    }

    .footer-main{
        grid-template-columns:1fr 1fr;
        gap:30px;
    }

    .footer-brand{
        grid-column:1/-1;
    }
}

@media(max-width:400px){

    .category-grid{
        grid-template-columns:1fr 1fr;
    }

    .brand-text h2{
        font-size:17px;
    }

    .brand-text span{
        font-size:9px;
    }
}
</style>
</head>


<body>

<!-- TOP STRIP -->
<div class="top-strip">
    <div class="top-inner">
        <div>🇮🇳 Government Jobs Information Portal</div>
        <div class="top-right">Verify every notification on the official website</div>
    </div>
</div>


<!-- NAVBAR -->
<header class="navbar">
    <div class="nav-inner">

        <a href="#home" class="brand">
            <div class="emblem">☸</div>

            <div class="brand-text">
                <h2>GovtJob India</h2>
                <span>GOVERNMENT JOBS PORTAL</span>
            </div>
        </a>

        <nav class="nav-links">
            <a href="#home">Home</a>
            <a href="#categories">Categories</a>
            <a href="#latest">Latest Jobs</a>
            <a href="#portals">Official Portals</a>
            <a href="#important" class="nav-btn">Important Links</a>
        </nav>

    </div>
</header>


<!-- HERO -->
<section class="hero" id="home">

    <div class="hero-content">

        <div class="gov-badge">
            🇮🇳 Trusted Government Job Information
        </div>

        <h1>
            Find Your <span>Government Job</span>
        </h1>

        <p class="hero-description">
            Search government job categories and quickly access
            official recruitment, examination, admit card and
            result portals.
        </p>

        <div class="search-wrapper">

            <div class="search-box">

                <div class="search-icon">🔎</div>

                <input
                    type="text"
                    id="searchInput"
                    placeholder="Search SSC, UPSC, Railway, Banking..."
                    autocomplete="off"
                >

                <button onclick="searchJobs()">
                    Search Jobs
                </button>

            </div>

            <div class="search-hints">
                Popular: SSC • UPSC • Railway • Banking • Police • Defence
            </div>

        </div>

    </div>

</section>


<!-- STATS -->
<section class="stats">

    <div class="stats-box">

        <div class="stat">
            <div class="stat-number">06+</div>
            <div class="stat-label">Major Categories</div>
        </div>

        <div class="stat">
            <div class="stat-number">10+</div>
            <div class="stat-label">Official Portals</div>
        </div>

        <div class="stat">
            <div class="stat-number">24×7</div>
            <div class="stat-label">Portal Access</div>
        </div>

        <div class="stat">
            <div class="stat-number">100%</div>
            <div class="stat-label">Official Links</div>
        </div>

    </div>

</section>


<!-- CATEGORIES -->
<section class="section" id="categories">

    <div class="section-heading">

        <div>
            <h2>Explore Categories</h2>
            <p>Choose the government sector you're interested in.</p>
        </div>

    </div>

    <div class="category-grid">

        <div class="category-card" onclick="filterCategory('SSC')">
            <div class="category-icon">📝</div>
            <h3>SSC</h3>
            <p>Staff Selection</p>
        </div>

        <div class="category-card" onclick="filterCategory('UPSC')">
            <div class="category-icon">🏛️</div>
            <h3>UPSC</h3>
            <p>Civil Services</p>
        </div>

        <div class="category-card" onclick="filterCategory('Railway')">
            <div class="category-icon">🚆</div>
            <h3>Railway</h3>
            <p>Railway Jobs</p>
        </div>

        <div class="category-card" onclick="filterCategory('Banking')">
            <div class="category-icon">🏦</div>
            <h3>Banking</h3>
            <p>Bank Jobs</p>
        </div>

        <div class="category-card" onclick="filterCategory('Police')">
            <div class="category-icon">👮</div>
            <h3>Police</h3>
            <p>Police Jobs</p>
        </div>

        <div class="category-card" onclick="filterCategory('Defence')">
            <div class="category-icon">🪖</div>
            <h3>Defence</h3>
            <p>Defence Jobs</p>
        </div>

    </div>

</section>


<!-- LATEST JOBS -->
<section class="jobs-section" id="latest">

    <div class="section">

        <div class="section-heading">

            <div>
                <h2>🔥 Latest Job Portals</h2>
                <p>Quick access to major official recruitment websites.</p>
            </div>

            <a href="#portals" class="view-all">
                View Official Portals →
            </a>

        </div>


        <div class="job-grid" id="jobGrid">


            <!-- SSC -->
            <article class="job-card" data-category="SSC">

                <div class="job-top">
                    <div class="job-icon">📝</div>
                    <div class="job-status">OFFICIAL</div>
                </div>

                <h3>SSC Recruitment</h3>

                <p>
                    Staff Selection Commission examinations,
                    recruitment notices and candidate services.
                </p>

                <div class="job-meta">
                    <span>SSC</span>
                    <span>Central Govt.</span>
                </div>

                <a
                    href="https://ssc.gov.in/"
                    target="_blank"
                    rel="noopener noreferrer"
                    class="job-button">
                    Official Website ↗
                </a>

            </article>


            <!-- UPSC -->
            <article class="job-card" data-category="UPSC">

                <div class="job-top">
                    <div class="job-icon">🏛️</div>
                    <div class="job-status">OFFICIAL</div>
                </div>

                <h3>UPSC Recruitment</h3>

                <p>
                    Civil services, examinations, recruitment,
                    results and e-admit card information.
                </p>

                <div class="job-meta">
                    <span>UPSC</span>
                    <span>Central Govt.</span>
                </div>

                <a
                    href="https://www.upsc.gov.in/"
                    target="_blank"
                    rel="noopener noreferrer"
                    class="job-button">
                    Official Website ↗
                </a>

            </article>


            <!-- RAILWAY -->
            <article class="job-card" data-category="Railway">

                <div class="job-top">
                    <div class="job-icon">🚆</div>
                    <div class="job-status">OFFICIAL</div>
                </div>

                <h3>Indian Railways</h3>

      

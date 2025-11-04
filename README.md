<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PR Report - October 2025 | Intelligent Lending</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.9.1/chart.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: #08051C;
            background: #170F57;
            background-image: 
                radial-gradient(circle at 20% 50%, rgba(146, 140, 200, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(38, 26, 145, 0.2) 0%, transparent 50%),
                radial-gradient(circle at 40% 20%, rgba(146, 140, 200, 0.1) 0%, transparent 40%);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        .summary-card {
            background: white;
            border-radius: 12px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }
        
        .summary-card h2 {
            font-size: 2.5rem;
            font-weight: 700;
            color: #170F57;
            text-align: center;
            margin-bottom: 1.5rem;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .stat-box {
            background: linear-gradient(135deg, #261A91 0%, #170F57 100%);
            color: white;
            padding: 1.5rem;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease;
            cursor: pointer;
        }
        
        .stat-box:hover {
            transform: scale(1.05);
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            display: block;
        }
        
        .stat-label {
            font-size: 0.9rem;
            opacity: 0.9;
            margin-top: 0.5rem;
        }
        
        .brand-row {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
            flex-wrap: nowrap;
            overflow-x: auto;
        }
        
        .brand-row .stat-box {
            flex: 1;
            min-width: 150px;
        }
        
        .brand-section {
            background: white;
            border-radius: 12px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            border-left: 4px solid #261A91;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .brand-section:hover {
            transform: scale(1.02);
            box-shadow: 0 4px 16px rgba(0,0,0,0.15);
        }
        
        .brand-header {
            margin-bottom: 2rem;
            padding-bottom: 1rem;
            border-bottom: 3px solid #928CC8;
        }
        
        .brand-name {
            font-size: 2.5rem;
            font-weight: 700;
            color: #170F57;
            text-align: center;
        }
        
        .section-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: #170F57;
            margin: 1.5rem 0 1rem 0;
        }
        
        .content-block {
            margin-bottom: 1.5rem;
            color: #08051C;
        }
        
        .content-block ul {
            list-style: none;
            padding-left: 0;
        }
        
        .content-block li {
            padding: 0.5rem 0;
            padding-left: 2rem;
            position: relative;
        }
        
        .content-block li:before {
            content: "→";
            position: absolute;
            left: 0.5rem;
            color: #261A91;
            font-weight: 700;
        }
        
        .coverage-link {
            display: block;
            padding: 1rem;
            margin: 0.5rem 0;
            background: #FFECF1;
            border-radius: 8px;
            text-decoration: none;
            color: #08051C;
            transition: all 0.3s ease;
            border-left: 3px solid #261A91;
        }
        
        .coverage-link:hover {
            background: #928CC8;
            transform: translateX(5px);
        }
        
        .coverage-source {
            font-weight: 600;
            color: #261A91;
            display: block;
            margin-bottom: 0.3rem;
        }
        
        nav {
            background: white;
            border-radius: 12px;
            padding: 1rem 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            position: sticky;
            top: 20px;
            z-index: 100;
        }
        
        nav a {
            color: #261A91;
            text-decoration: none;
            font-weight: 600;
            padding: 0.5rem 1rem;
            border-radius: 6px;
            transition: all 0.3s ease;
        }
        
        nav a:hover {
            background: #FFE27C;
            transform: translateY(-2px);
        }
        
        html {
            scroll-padding-top: 120px;
        }
        
        @media (max-width: 768px) {
            .stats-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div style="text-align: center; margin-bottom: 2rem;">
            <h1 style="font-size: 3rem; font-weight: 700; color: white; margin: 0;">Intelligent Lending</h1>
        </div>
        
        <nav>
            <div style="display: flex; justify-content: center; gap: 2rem; flex-wrap: wrap;">
                <a href="#summary">📊 Summary</a>
                <a href="#binq">🤖 Binq</a>
                <a href="#credability">💳 CredAbility</a>
                <a href="#luv">💙 Luv</a>
                <a href="#ocean">🌊 Ocean</a>
                <a href="#totallymoney">™️ TotallyMoney</a>
            </div>
        </nav>
        
        <div class="summary-card" id="summary">
            <h2>⭐ October PR Update ⭐</h2>
            
            <div style="text-align: left; margin-bottom: 2rem; padding: 1.5rem; background: #f8f9fa; border-radius: 8px; border-left: 4px solid #261A91;">
                <h3 style="font-size: 1.5rem; font-weight: 700; color: #170F57; margin-bottom: 1rem;">A Record-Breaking Month for Intelligent Lending PR</h3>
                
                <p style="margin-bottom: 1rem;">October delivered exceptional results across the Intelligent Lending portfolio, with nearly 1,340 pieces of coverage spanning 262 different outlets and 404 journalists - marking our strongest performance to date. The coverage breakdown demonstrates impressive reach: 138 mentions in the national press, 362 in regional outlets, and 740 in local publications.</p>
                
                <p style="margin-bottom: 1rem;">TotallyMoney dominated with an impressive 976 mentions, driven by strategic commentary on the surge of seven CASS offers hitting the market simultaneously, alongside our down-selling warning and balance transfer analysis that caught widespread media attention.</p>
                
                <p style="margin-bottom: 1rem;">The month saw significant recognition across our brands. CredAbility earned a nomination for Innovation in Consumer Finance at the MoneyAge awards, while Ocean was shortlisted for Credit Builder Card Provider of the Year. Both brands leveraged cross-team collaboration with User Research and Social teams to develop compelling case studies that resonated with journalists.</p>
                
                <p style="margin-bottom: 1rem;">Meanwhile, Binq made substantial progress on brand development, completing comprehensive tone of voice guidelines and brand language work that will shape how the business communicates across all channels.</p>
                
                <p style="margin-bottom: 1rem;">Key coverage highlights included The FCA referencing TotallyMoney's research in their car finance scandal analysis - a significant validation of our data-driven approach. Major placements spanned Daily Mail, The Independent, The Guardian, Daily Mirror, and The Express, with topics ranging from credit card interest-free periods and energy bill management to mobile phone bill reductions.</p>
                
                <p>Behind the scenes, progress continued on strategic initiatives. Luv's brand refresh and website rebuild moved forward with six key content pages completed, while TotallyMoney completed its comprehensive SEO overhaul of all credit card product pages. Looking ahead to November, the focus shifts to Autumn Budget analysis, Talk Money Week campaigns, and scam awareness pieces tied to Black Friday and Christmas shopping.</p>
            </div>
            
            <div class="stats-grid">
                <div class="stat-box">
                    <span class="stat-number">1,338</span>
                    <span class="stat-label">Total Mentions</span>
                </div>
                <div class="stat-box">
                    <span class="stat-number">1,298</span>
                    <span class="stat-label">Separate Articles</span>
                </div>
                <div class="stat-box">
                    <span class="stat-number">4</span>
                    <span class="stat-label">Active Brands</span>
                </div>
            </div>
            
            <div class="brand-row">
                <div class="stat-box" style="background: linear-gradient(135deg, #170F57 0%, #261A91 100%);">
                    <span class="stat-number">64</span>
                    <span class="stat-label">CredAbility</span>
                </div>
                <div class="stat-box" style="background: linear-gradient(135deg, #261A91 0%, #928CC8 100%);">
                    <span class="stat-number">298</span>
                    <span class="stat-label">Ocean</span>
                </div>
                <div class="stat-box" style="background: linear-gradient(135deg, #170F57 0%, #3A384B 100%);">
                    <span class="stat-number">976</span>
                    <span class="stat-label">TotallyMoney</span>
                </div>
                <div class="stat-box" style="background: linear-gradient(135deg, #928CC8 0%, #73738C 100%);">
                    <span class="stat-number">4</span>
                    <span class="stat-label">Binq</span>
                </div>
            </div>
            
            <h3 style="font-size: 1.8rem; font-weight: 700; color: #170F57; text-align: center; margin: 2rem 0 1.5rem 0;">2025 Coverage</h3>
            
            <div style="margin: 2rem 0;">
                <canvas id="prChart" style="max-height: 400px;"></canvas>
            </div>
            
            <div style="text-align: center; margin: 2rem 0; padding: 1.5rem; background: white; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
                <p style="font-size: 1.2rem; font-weight: 600; color: #170F57;">During 2025, the four active Intelligent Lending brands have received a total of <strong style="font-size: 1.4rem; color: #261A91;">5,667</strong> pieces of coverage.</p>
            </div>
        </div>

        <div class="brand-section" id="binq">
            <div class="brand-header">
                <h2 class="brand-name">🤖 Binq 🤖</h2>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📝 Top Level</h3>
                <ul>
                    <li>Brand language – spelling out the Binq principles, identifying and naming our brand purpose, creating straplines, writing boilerplate copy and nailing down the essentials of how we talk and write about our brand. As part of this, we did some competitor analysis.</li>
                    <li>Binq Tone of Voice – identifying the correct tone for the brand and then creating a clear set of principles and guidelines for everyone to follow (including the AI) when they write as Binq. This will soon be shared with the wider Binq team.</li>
                    <li>Suite of welcome letters - that will be sent out automatically to the customers at various stages in their journey through getting funding with Binq, including nudges to complete certain tasks, reminders of what Binq offers, hooks if they drop out and longer term value once the initial interaction has completed.</li>
                    <li>PDF brochure - It will make it really clear to all potential customers what Binq can do for them and why we're a great choice.</li>
                    <li>3 press comments on relevant business topics, and a CEO pitch to The Metro</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">✏️ Press Comments</h3>
                <ul>
                    <li>Energy switching / no price cap for businesses comment</li>
                    <li>Self-assessment registration deadline</li>
                    <li>Autum Budget startup parent</li>
                    <li>Tanyel Mustafa, The Metro/ looking to speak with SME owners</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📰 Coverage Highlights</h3>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Birmingham Mail</span>
                    HMRC imposes strict deadline 'you can't afford to miss'
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Manchester Evening News</span>
                    HMRC sets strict Sunday deadline
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Devon Live</span>
                    HMRC sets strict Sunday deadline for UK households
                </a>
            </div>
            
            <div style="margin: 2rem 0;">
                <div style="position: relative; max-width: 900px; margin: 0 auto;">
                    <div id="binqCarouselContainer" style="overflow: hidden; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); background: white; position: relative; padding-bottom: 75%;">
                        <div id="binqCarousel" style="display: flex; transition: transform 0.5s ease-in-out; position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/yxKpr2Xb/binq-1.png" alt="Binq Coverage 1" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/yxTpqnvG/binq2.png" alt="Binq Coverage 2" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/prBcNkq6/binq3.png" alt="Binq Coverage 3" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                        </div>
                    </div>
                    
                    <button id="binqPrevBtn" style="position: absolute; left: -50px; top: 50%; transform: translateY(-50%); background: white; border: 2px solid #261A91; border-radius: 50%; width: 45px; height: 45px; cursor: pointer; font-size: 24px; color: #261A91; font-weight: bold; box-shadow: 0 2px 8px rgba(0,0,0,0.2); z-index: 10;">‹</button>
                    <button id="binqNextBtn" style="position: absolute; right: -50px; top: 50%; transform: translateY(-50%); background: white; border: 2px solid #261A91; border-radius: 50%; width: 45px; height: 45px; cursor: pointer; font-size: 24px; color: #261A91; font-weight: bold; box-shadow: 0 2px 8px rgba(0,0,0,0.2); z-index: 10;">›</button>
                    
                    <div id="binqDotsContainer" style="text-align: center; margin-top: 1.5rem; display: flex; gap: 10px; justify-content: center;"></div>
                </div>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📅 November Plans</h3>
                <ul>
                    <li>Create a suite of marketing emails to keep customers engaged and eventually a regular newsletter with more broader general interest items to add value for SMEs and boost our brand visibility.</li>
                    <li>After an audit of the website, we've identified the next pages that we need in order to build the business. These are an 'About us' page, increased functionality for the guides, customer testimonials and a blog. We're busy creating content for these pages and will look forward to being able to launch them when we can. The blog content will be regularly updated and will feed into the monthly newsletter.</li>
                </ul>
            </div>
        </div>

        <div class="brand-section" id="credability">
            <div class="brand-header">
                <h2 class="brand-name">💳 CredAbility 💳</h2>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📝 Top Level</h3>
                <ul>
                    <li>Attended MoneyAge awards – nominated for Innovation in Consumer Finance</li>
                    <li>Cross-collaboration with User Research & Social teams – planning case studies and reviews to be used in PR</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">✏️ Press Releases</h3>
                <ul>
                    <li>Why your mortgage might be rejected and how to fix it</li>
                    <li>One month until the Autumn Statement: 5 things every saver should check now</li>
                    <li>New research reveals top five money myths costing Brits £100s every year</li>
                    <li>Inflation pushes Brits back to 2008-style saving frenzy</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📰 Coverage Highlights</h3>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Daily Mirror</span>
                    UK households warned make payment before November or 'there may be more tax'
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">MSN</span>
                    Major inheritance tax change could be announced in November say experts
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">The Express</span>
                    Warning for Lloyds, Halifax, Santander customers over £500 payments
                </a>
            </div>
            
            <div style="margin: 2rem 0;">
                <div style="position: relative; max-width: 900px; margin: 0 auto;">
                    <div id="credCarouselContainer" style="overflow: hidden; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); background: white; position: relative; padding-bottom: 75%;">
                        <div id="credCarousel" style="display: flex; transition: transform 0.5s ease-in-out; position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/BZYN98g2/cred1.png" alt="CredAbility Coverage 1" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/L4CvKqTV/cred2.png" alt="CredAbility Coverage 2" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/J76KVyq5/cred3.png" alt="CredAbility Coverage 3" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/RCsG53RQ/cred4.png" alt="CredAbility Coverage 4" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                        </div>
                    </div>
                    
                    <button id="credPrevBtn" style="position: absolute; left: -50px; top: 50%; transform: translateY(-50%); background: white; border: 2px solid #261A91; border-radius: 50%; width: 45px; height: 45px; cursor: pointer; font-size: 24px; color: #261A91; font-weight: bold; box-shadow: 0 2px 8px rgba(0,0,0,0.2); z-index: 10;">‹</button>
                    <button id="credNextBtn" style="position: absolute; right: -50px; top: 50%; transform: translateY(-50%); background: white; border: 2px solid #261A91; border-radius: 50%; width: 45px; height: 45px; cursor: pointer; font-size: 24px; color: #261A91; font-weight: bold; box-shadow: 0 2px 8px rgba(0,0,0,0.2); z-index: 10;">›</button>
                    
                    <div id="credDotsContainer" style="text-align: center; margin-top: 1.5rem; display: flex; gap: 10px; justify-content: center;"></div>
                </div>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📅 November Plans</h3>
                <ul>
                    <li>Autumn Budget - what Brits can expect, plus any early 2026 financial updates people should be aware of.</li>
                    <li>"5 ways you're sabotaging your finances" - consumer-friendly piece.</li>
                    <li>Borrowing in retirement - expert insights following the latest state pension news.</li>
                    <li>Using our summer survey data revealing that one in three people who checked their credit report found a mistake.</li>
                    <li>Ongoing journalist requests and reactive opportunities</li>
                </ul>
            </div>
        </div>

        <div class="brand-section" id="luv">
            <div class="brand-header">
                <h2 class="brand-name">💙 Luv 💙</h2>
            </div>
            
            <div class="content-block">
                <p>Brand refresh and website rebuild taking place. Working with the team to create all onsite content, including six of the following pages:</p>
                <ul>
                    <li>Homepage</li>
                    <li>How car finance works ✅</li>
                    <li>HP car finance ✅</li>
                    <li>PCP car finance ✅</li>
                    <li>Value my car</li>
                    <li>Bad credit card finance ✅</li>
                    <li>No deposit car finance ✅</li>
                    <li>Refinance my car</li>
                    <li>Car finance explained</li>
                    <li>Business car finance ✅</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📅 November Plans</h3>
                <ul>
                    <li>Create content for remaining pages</li>
                </ul>
            </div>
        </div>

        <div class="brand-section" id="ocean">
            <div class="brand-header">
                <h2 class="brand-name">🌊 Ocean 🌊</h2>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📝 Top Level</h3>
                <ul>
                    <li>Shortlisted for <strong>Credit Builder Card Provider of the Year</strong></li>
                    <li>Cross-collaboration with User Research & Social teams – planning case studies and reviews to be used in PR</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">✏️ Press Releases</h3>
                <ul>
                    <li>Energy bill rise pushes 1m UK households into arrears</li>
                    <li>Experts warn unlimited contactless could fuel debt and fraud</li>
                    <li>Brits can cut energy bills by changing the day they do the washing</li>
                    <li>6 ways to afford Christmas on a budget</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📰 Coverage Highlights</h3>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Birmingham Live</span>
                    Christmas 2025 shopping hacks with six smart ways to save money
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">The Guardian</span>
                    Scam watch - Cut your energy bills by a third? No, these 'energy-saving plugs' will cause nothing but hassle
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Daily Mail</span>
                    The 5 money questions you MUST ask your partner before having children, according to experts
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">MSN</span>
                    UK households told day of the week they should be using washing machines to cut bills
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Daily Mirror</span>
                    Expert says 250,000 Brits turning to illegal energy hacks
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Best Magazine</span>
                    Full-page spread
                </a>
            </div>
            
            <div style="margin: 2rem 0;">
                <div style="position: relative; max-width: 900px; margin: 0 auto;">
                    <div id="oceanCarouselContainer" style="overflow: hidden; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.15); background: white; position: relative; padding-bottom: 75%;">
                        <div id="oceanCarousel" style="display: flex; transition: transform 0.5s ease-in-out; position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/CL0M01LQ/o1.png" alt="Ocean Coverage 1" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/PrHfHx5s/o2.png" alt="Ocean Coverage 2" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                            <div style="min-width: 100%; box-sizing: border-box; height: 100%;">
                                <img src="https://i.postimg.cc/MKwZwTpW/o3.png" alt="Ocean Coverage 3" style="width: 100%; height: 100%; display: block; object-fit: cover; object-position: center;">
                            </div>
                        </div>
                    </div>
                    
                    <button id="oceanPrevBtn" style="position: absolute; left: -50px; top: 50%; transform: translateY(-50%); background: white; border: 2px solid #261A91; border-radius: 50%; width: 45px; height: 45px; cursor: pointer; font-size: 24px; color: #261A91; font-weight: bold; box-shadow: 0 2px 8px rgba(0,0,0,0.2); z-index: 10;">‹</button>
                    <button id="oceanNextBtn" style="position: absolute; right: -50px; top: 50%; transform: translateY(-50%); background: white; border: 2px solid #261A91; border-radius: 50%; width: 45px; height: 45px; cursor: pointer; font-size: 24px; color: #261A91; font-weight: bold; box-shadow: 0 2px 8px rgba(0,0,0,0.2); z-index: 10;">›</button>
                    
                    <div id="oceanDotsContainer" style="text-align: center; margin-top: 1.5rem; display: flex; gap: 10px; justify-content: center;"></div>
                </div>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📅 November Plans</h3>
                <ul>
                    <li>Talk Money Week – how to talk about money and why it's so important.</li>
                    <li>Scam awareness pieces including Black Friday & Christmas shopping scams, and the top celebrities used by scammers in 2025.</li>
                    <li>Top 5 debt mistakes to avoid this winter – featuring advice and links to Debt Consolidation Loans page.</li>
                    <li>Improve rather than move – the true cost of home renovations and how to budget, supported by our insider data showing a rise in home improvement loans.</li>
                    <li>Ongoing journalist requests and reactive opportunities</li>
                </ul>
            </div>
        </div>

        <div class="brand-section" id="totallymoney">
            <div class="brand-header">
                <h2 class="brand-name">™️ TotallyMoney ™️</h2>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📝 Top Level</h3>
                <ul>
                    <li>Record month with almost 1,000 pieces of coverage (better try harder next time), largely down to numerous current account switch offers coming to market, and capitalizing on the medias love for them</li>
                    <li>All credit card product pages completely rewritten and rebuilt with the aim of improving UX, UI, SEO on the SERPs, CTRs, CPAs, and overall ROMI</li>
                    <li>Highlight for me was The FCA referencing our research in their car finance scandal report, good to be on the regulators radar for the right reasons</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">✏️ Press Releases and Comments</h3>
                <ul>
                    <li>SEVEN CASS offers press release</li>
                    <li>Down-selling warning press release</li>
                    <li>Five tips for getting the best personal loan deal press release</li>
                    <li>Energy price cap/ savings comment</li>
                    <li>Self-assessment registration deadline comment</li>
                    <li>Tesco Mobile agreement ending comment</li>
                    <li>Barclays CASS offer comment</li>
                    <li>Lloyds credit builder card comment</li>
                    <li>Zopa savings account comment</li>
                    <li>Cold snap, switch providers (drafted not sent) comment</li>
                    <li>No cold snap, but still switch comment</li>
                    <li>Inflation comment</li>
                    <li>Santander current account offer comment</li>
                    <li>Current Account Switch Service – analysis of figures press release</li>
                    <li>Ofgem urging people to claim £240m comment</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📞 Requests</h3>
                <ul>
                    <li>Energy saving myths: Harriet Cooke/ The Sun</li>
                    <li>Credit scores: Tanyel Mustafa/ The Metro</li>
                    <li>BNPL holidays: Harriet Cooke/ The Guardian</li>
                    <li>Barclays CASS: Nicholas Dawson/ The Express</li>
                    <li>Credit scores: Adele Cooke/ The Sun</li>
                    <li>Balance transfers: Michael Brown/ The Sun</li>
                </ul>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📰 Coverage Highlights</h3>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Daily Mail</span>
                    Credit cards now offer bumper interest-free periods of almost 3 years
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">The Independent</span>
                    High street banks found to offer worse interest rates
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">Express</span>
                    Millions of mobile phone users urged to text 5-digit number to reduce bill
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">The Mirror</span>
                    Change one credit card habit to improve your financial worthiness
                </a>
                <a href="#" target="_blank" class="coverage-link">
                    <span class="coverage-source">The FCA</span>
                    In its analysis of the impact of the car finance scandal, the regulator referenced a TotallyMoney press release which put a price on the impact of a poor credit score on the cost of a personal loan.
                </a>
            </div>
            
            <div class="content-block">
                <h3 class="section-title">📅 November Plans</h3>
                <p>On holiday for a chunk of November, leaving tomorrow, the 5th, and I'll return on 24th.</p>
            </div>
        </div>

        <div class="summary-card" style="margin-top: 3rem; text-align: left;">
            <h3 style="font-size: 1.5rem; font-weight: 700; color: #170F57; margin-bottom: 1rem;">Looking Ahead</h3>
            <p style="margin-bottom: 1rem;">Beyond November, and moving into December and January, we will be finalising the positioning for each brand, and wrapping it into the Intelligent Lending story. That way, we'll have a clear outline of who we are, and why we do it. And we'll be in a better position when it comes to launching/ making Numero 'real'.</p>
            <p style="margin-bottom: 1rem;">We will also roll out Binq's new tone of voice across the website, app, AI, CRM, and other marketing channels, while creating a content calendar which will cover the above and PR.</p>
            <p style="margin-bottom: 1rem;">At the same time, we'll review what's gone well this year, what can be improved, what we'll repeat in 2026, and new things we'll be trying and be adding to the calendar.</p>
            <p>This year has been about getting everything in order, and next year we'll focus on growing awareness for the group and the brands that sit within it.</p>
        </div>
        
        <div class="summary-card" style="text-align: center; margin-top: 2rem;">
            <p style="color: #3A384B; margin-bottom: 1rem;">Questions or feedback? Please get in touch with the PR and Content team.</p>
            <div style="display: flex; flex-direction: column; gap: 0.5rem; align-items: center;">
                <a href="mailto:jmccaffrey@totallymoney.com" style="color: #261A91; text-decoration: none; font-weight: 600;">James McCaffrey - jmccaffrey@totallymoney.com</a>
                <a href="mailto:alicia.boukersi@ocean.co.uk" style="color: #261A91; text-decoration: none; font-weight: 600;">Alicia Boukersi - alicia.boukersi@ocean.co.uk</a>
                <a href="mailto:eleanor.debruin@binq.co.uk" style="color: #261A91; text-decoration: none; font-weight: 600;">Eleanor de Bruin - eleanor.debruin@binq.co.uk</a>
            </div>
        </div>
    </div>

    <script>
        const ctx = document.getElementById('prChart').getContext('2d');
        
        const data = {
            labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October'],
            datasets: [
                {
                    label: 'TotallyMoney',
                    data: [104, 154, 575, 71, 34, 45, 48, 212, 230, 976],
                    backgroundColor: '#1e3a8a',
                    borderColor: '#1e3a8a',
                    borderWidth: 0
                },
                {
                    label: 'Ocean',
                    data: [103, 26, 344, 511, 26, 203, 121, 565, 236, 298],
                    backgroundColor: '#0ea5e9',
                    borderColor: '#0ea5e9',
                    borderWidth: 0
                },
                {
                    label: 'CredAbility',
                    data: [41, 26, 384, 70, 21, 33, 64, 32, 34, 64],
                    backgroundColor: '#7c3aed',
                    borderColor: '#7c3aed',
                    borderWidth: 0
                },
                {
                    label: 'Binq',
                    data: [0, 0, 0, 0, 0, 0, 0, 14, 2, 4],
                    backgroundColor: '#10b981',
                    borderColor: '#10b981',
                    borderWidth: 0
                },
                {
                    label: 'Total',
                    data: [248, 206, 1303, 652, 81, 281, 233, 823, 764, 1342],
                    type: 'line',
                    backgroundColor: 'transparent',
                    borderColor: '#f97316',
                    borderWidth: 3,
                    pointRadius: 0,
                    pointHoverRadius: 6,
                    tension: 0.4,
                    yAxisID: 'y1'
                }
            ]
        };

        const config = {
            type: 'bar',
            data: data,
            options: {
                responsive: true,
                maintainAspectRatio: true,
                interaction: {
                    mode: 'index',
                    intersect: false,
                },
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            usePointStyle: true,
                            padding: 15,
                            font: {
                                size: 12
                            }
                        }
                    },
                    tooltip: {
                        backgroundColor: 'rgba(0, 0, 0, 0.8)',
                        padding: 12,
                        titleFont: {
                            size: 13
                        },
                        bodyFont: {
                            size: 12
                        }
                    }
                },
                scales: {
                    x: {
                        grid: {
                            display: false
                        },
                        ticks: {
                            font: {
                                size: 11
                            }
                        }
                    },
                    y: {
                        type: 'linear',
                        display: true,
                        position: 'left',
                        beginAtZero: true,
                        max: 1000,
                        ticks: {
                            stepSize: 100,
                            font: {
                                size: 11
                            }
                        },
                        grid: {
                            color: '#e5e5e5'
                        }
                    },
                    y1: {
                        type: 'linear',
                        display: true,
                        position: 'right',
                        beginAtZero: true,
                        max: 1600,
                        ticks: {
                            stepSize: 200,
                            font: {
                                size: 11
                            }
                        },
                        grid: {
                            drawOnChartArea: false
                        }
                    }
                },
                barPercentage: 0.9,
                categoryPercentage: 0.8
            }
        };

        new Chart(ctx, config);

        // Binq Carousel
        (function() {
            let binqSlideIndex = 0;
            const binqTotalSlides = 3;
            const binqCarousel = document.getElementById('binqCarousel');
            const binqDotsContainer = document.getElementById('binqDotsContainer');
            
            for (let i = 0; i < binqTotalSlides; i++) {
                const dot = document.createElement('span');
                dot.style.cssText = 'width: 12px; height: 12px; border-radius: 50%; background: #928CC8; cursor: pointer; display: inline-block; transition: all 0.3s;';
                dot.onclick = () => binqGoToSlide(i);
                binqDotsContainer.appendChild(dot);
            }
            
            const binqDots = binqDotsContainer.children;
            
            function binqUpdateSlide() {
                binqCarousel.style.transform = `translateX(-${binqSlideIndex * 100}%)`;
                for (let i = 0; i < binqDots.length; i++) {
                    binqDots[i].style.background = i === binqSlideIndex ? '#261A91' : '#928CC8';
                    binqDots[i].style.transform = i === binqSlideIndex ? 'scale(1.2)' : 'scale(1)';
                }
            }
            
            function binqNextSlide() {
                binqSlideIndex = (binqSlideIndex + 1) % binqTotalSlides;
                binqUpdateSlide();
            }
            
            function binqPrevSlide() {
                binqSlideIndex = (binqSlideIndex - 1 + binqTotalSlides) % binqTotalSlides;
                binqUpdateSlide();
            }
            
            function binqGoToSlide(index) {
                binqSlideIndex = index;
                binqUpdateSlide();
            }
            
            document.getElementById('binqNextBtn').onclick = binqNextSlide;
            document.getElementById('binqPrevBtn').onclick = binqPrevSlide;
            
            setInterval(binqNextSlide, 5000);
            
            binqUpdateSlide();
        })();

        // CredAbility Carousel
        (function() {
            let credSlideIndex = 0;
            const credTotalSlides = 4;
            const credCarousel = document.getElementById('credCarousel');
            const credDotsContainer = document.getElementById('credDotsContainer');
            
            for (let i = 0; i < credTotalSlides; i++) {
                const dot = document.createElement('span');
                dot.style.cssText = 'width: 12px; height: 12px; border-radius: 50%; background: #928CC8; cursor: pointer; display: inline-block; transition: all 0.3s;';
                dot.onclick = () => credGoToSlide(i);
                credDotsContainer.appendChild(dot);
            }
            
            const credDots = credDotsContainer.children;
            
            function credUpdateSlide() {
                credCarousel.style.transform = `translateX(-${credSlideIndex * 100}%)`;
                for (let i = 0; i < credDots.length; i++) {
                    credDots[i].style.background = i === credSlideIndex ? '#261A91' : '#928CC8';
                    credDots[i].style.transform = i === credSlideIndex ? 'scale(1.2)' : 'scale(1)';
                }
            }
            
            function credNextSlide() {
                credSlideIndex = (credSlideIndex + 1) % credTotalSlides;
                credUpdateSlide();
            }
            
            function credPrevSlide() {
                credSlideIndex = (credSlideIndex - 1 + credTotalSlides) % credTotalSlides;
                credUpdateSlide();
            }
            
            function credGoToSlide(index) {
                credSlideIndex = index;
                credUpdateSlide();
            }
            
            document.getElementById('credNextBtn').onclick = credNextSlide;
            document.getElementById('credPrevBtn').onclick = credPrevSlide;
            
            setInterval(credNextSlide, 5000);
            
            credUpdateSlide();
        })();

        // Ocean Carousel
        (function() {
            let oceanSlideIndex = 0;
            const oceanTotalSlides = 3;
            const oceanCarousel = document.getElementById('oceanCarousel');
            const oceanDotsContainer = document.getElementById('oceanDotsContainer');
            
            for (let i = 0; i < oceanTotalSlides; i++) {
                const dot = document.createElement('span');
                dot.style.cssText = 'width: 12px; height: 12px; border-radius: 50%; background: #928CC8; cursor: pointer; display: inline-block; transition: all 0.3s;';
                dot.onclick = () => oceanGoToSlide(i);
                oceanDotsContainer.appendChild(dot);
            }
            
            const oceanDots = oceanDotsContainer.children;
            
            function oceanUpdateSlide() {
                oceanCarousel.style.transform = `translateX(-${oceanSlideIndex * 100}%)`;
                for (let i = 0; i < oceanDots.length; i++) {
                    oceanDots[i].style.background = i === oceanSlideIndex ? '#261A91' : '#928CC8';
                    oceanDots[i].style.transform = i === oceanSlideIndex ? 'scale(1.2)' : 'scale(1)';
                }
            }
            
            function oceanNextSlide() {
                oceanSlideIndex = (oceanSlideIndex + 1) % oceanTotalSlides;
                oceanUpdateSlide();
            }
            
            function oceanPrevSlide() {
                oceanSlideIndex = (oceanSlideIndex - 1 + oceanTotalSlides) % oceanTotalSlides;
                oceanUpdateSlide();
            }
            
            function oceanGoToSlide(index) {
                oceanSlideIndex = index;
                oceanUpdateSlide();
            }
            
            document.getElementById('oceanNextBtn').onclick = oceanNextSlide;
            document.getElementById('oceanPrevBtn').onclick = oceanPrevSlide;
            
            setInterval(oceanNextSlide, 5000);
            
            oceanUpdateSlide();
        })();
    </script>
</body>
</html>

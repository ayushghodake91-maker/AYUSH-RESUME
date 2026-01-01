<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ayush Ghodake - Digital Marketing Specialist</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #e2e8f0;
            background: #0f172a;
            min-height: 100vh;
            padding: 20px;
            position: relative;
            overflow-x: hidden;
        }
        
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 50%, rgba(66, 133, 244, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(52, 168, 83, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 40% 20%, rgba(251, 188, 4, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 60% 90%, rgba(234, 67, 53, 0.1) 0%, transparent 50%);
            z-index: 0;
            animation: pulse 15s ease-in-out infinite;
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.8; }
        }
        
        body::after {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(rgba(66, 133, 244, 0.03) 1px, transparent 1px),
                linear-gradient(90deg, rgba(66, 133, 244, 0.03) 1px, transparent 1px);
            background-size: 50px 50px;
            z-index: 0;
            animation: gridMove 20s linear infinite;
        }
        
        @keyframes gridMove {
            0% { transform: translate(0, 0); }
            100% { transform: translate(50px, 50px); }
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(15, 23, 42, 0.95);
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.5);
            overflow: hidden;
            backdrop-filter: blur(10px);
            position: relative;
            z-index: 1;
        }
        
        header {
            background: linear-gradient(135deg, #4285f4 0%, #34a853 50%, #fbbc04 75%, #ea4335 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 1px, transparent 1px);
            background-size: 50px 50px;
            animation: moveBackground 20s linear infinite;
        }
        
        @keyframes moveBackground {
            0% { transform: translate(0, 0); }
            100% { transform: translate(50px, 50px); }
        }
        
        .header-content {
            position: relative;
            z-index: 1;
        }
        
        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }
        
        .tagline {
            font-size: 1.3em;
            margin-bottom: 20px;
            opacity: 0.95;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(255,255,255,0.2);
            padding: 8px 16px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 25px;
        }
        
        .social-btn {
            background: white;
            color: #4285f4;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 600;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }
        
        .social-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
        }
        
        .content {
            padding: 40px;
            color: #e2e8f0;
        }
        
        .section {
            margin-bottom: 50px;
            animation: fadeIn 0.8s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        h2 {
            color: #60a5fa;
            font-size: 2em;
            margin-bottom: 25px;
            padding-bottom: 10px;
            border-bottom: 3px solid #fbbc04;
            display: inline-block;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .stat-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            transition: transform 0.3s;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
        }
        
        .stat-number {
            font-size: 2.5em;
            font-weight: bold;
            margin-bottom: 10px;
        }
        
        .stat-label {
            font-size: 1.1em;
            opacity: 0.9;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .skill-category {
            background: rgba(30, 41, 59, 0.8);
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #4285f4;
            backdrop-filter: blur(5px);
        }
        
        .skill-category h3 {
            color: #e2e8f0;
            margin-bottom: 15px;
            font-size: 1.3em;
        }
        
        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill-tag {
            background: rgba(66, 133, 244, 0.2);
            color: #60a5fa;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: 600;
            box-shadow: 0 2px 5px rgba(0,0,0,0.3);
            border: 1px solid rgba(66, 133, 244, 0.3);
        }
        
        .experience-item, .project-item {
            background: rgba(30, 41, 59, 0.6);
            padding: 30px;
            border-radius: 15px;
            margin-bottom: 25px;
            border-left: 5px solid #34a853;
            transition: box-shadow 0.3s, transform 0.3s;
            backdrop-filter: blur(5px);
        }
        
        .experience-item:hover, .project-item:hover {
            box-shadow: 0 5px 20px rgba(66, 133, 244, 0.3);
            transform: translateX(5px);
        }
        
        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            flex-wrap: wrap;
            margin-bottom: 15px;
        }
        
        .job-title {
            font-size: 1.5em;
            color: #e2e8f0;
            font-weight: bold;
        }
        
        .company {
            color: #60a5fa;
            font-size: 1.2em;
            font-weight: 600;
            margin-top: 5px;
        }
        
        .date-location {
            text-align: right;
            color: #94a3b8;
            font-weight: 600;
        }
        
        .responsibilities {
            list-style: none;
            margin-top: 15px;
        }
        
        .responsibilities li {
            padding-left: 25px;
            margin-bottom: 10px;
            position: relative;
            color: #cbd5e1;
        }
        
        .responsibilities li::before {
            content: '▸';
            color: #60a5fa;
            font-weight: bold;
            position: absolute;
            left: 0;
        }
        
        .cert-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 20px;
        }
        
        .cert-card {
            background: linear-gradient(135deg, #4285f4 0%, #34a853 100%);
            color: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .cert-name {
            font-weight: bold;
            font-size: 1.1em;
            margin-bottom: 8px;
        }
        
        .cert-issuer {
            opacity: 0.9;
            font-size: 0.95em;
        }
        
        .download-section {
            background: linear-gradient(135deg, #ea4335 0%, #fbbc04 100%);
            color: white;
            padding: 50px;
            text-align: center;
            border-radius: 15px;
            margin-top: 40px;
        }
        
        .download-btn {
            background: white;
            color: #ea4335;
            padding: 18px 40px;
            font-size: 1.2em;
            font-weight: bold;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
            transition: transform 0.3s, box-shadow 0.3s;
            text-decoration: none;
            display: inline-block;
            margin-top: 20px;
        }
        
        .download-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.3);
        }
        
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 30px;
            margin-top: 40px;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2em;
            }
            
            .tagline {
                font-size: 1.1em;
            }
            
            .content {
                padding: 20px;
            }
            
            .job-header {
                flex-direction: column;
            }
            
            .date-location {
                text-align: left;
                margin-top: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="header-content">
                <h1>Ayush Ghodake</h1>
                <p class="tagline">Digital Marketing Specialist | Growth Strategist | AI-Powered Campaign Expert</p>
                
                <div class="contact-info">
                    <div class="contact-item">
                        <span>📧</span>
                        <a href="mailto:ayushghodake91@gmail.com" style="color: white; text-decoration: none;">ayushghodake91@gmail.com</a>
                    </div>
                    <div class="contact-item">
                        <span>📱</span>
                        <span>7758046516</span>
                    </div>
                    <div class="contact-item">
                        <span>📍</span>
                        <span>Pune, Maharashtra</span>
                    </div>
                </div>
                
                <div class="social-links">
                    <a href="https://ayushghodake91-maker.github.io" class="social-btn" target="_blank">🌐 Website</a>
                    <a href="https://github.com/ayushghodake91-maker" class="social-btn" target="_blank">GitHub</a>
                    <a href="https://www.linkedin.com/in/ayush-ghodake-46" class="social-btn" target="_blank">LinkedIn</a>
                    <a href="https://www.youtube.com/@DollarWise9" class="social-btn" target="_blank">YouTube</a>
                    <a href="https://twitter.com/AyushGhoda90403" class="social-btn" target="_blank">X (Twitter)</a>
                </div>
            </div>
        </header>
        
        <div class="content">
            <section class="section">
                <h2>Key Achievements</h2>
                <div class="stats-grid">
                    <div class="stat-card">
                        <div class="stat-number">25%+</div>
                        <div class="stat-label">ROI Improvement</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">40%</div>
                        <div class="stat-label">Content Creation Time Reduced</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">35%</div>
                        <div class="stat-label">Email Engagement Increase</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">100+</div>
                        <div class="stat-label">Successful Campaigns</div>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2>Professional Experience</h2>
                
                <div class="experience-item">
                    <div class="job-header">
                        <div>
                            <div class="job-title">Business Development Executive</div>
                            <div class="company">The Enterprise Globe Magazine</div>
                        </div>
                        <div class="date-location">
                            <div>Sep 2025 – Present</div>
                            <div>Pune, Maharashtra</div>
                        </div>
                    </div>
                    <ul class="responsibilities">
                        <li>Spearhead digital marketing initiatives, expanding brand reach for B2B enterprise publication</li>
                        <li>Collaborate with editorial teams to create compelling content for C-suite executives, driving measurable engagement</li>
                        <li>Manage end-to-end social media strategies across Facebook, Instagram, and LinkedIn, increasing engagement rates</li>
                        <li>Analyze campaign performance using Google Analytics, optimizing conversion rates and improving ROI by 25%+</li>
                        <li>Set up and optimize Google Ads campaigns (Search & Display), managing budgets to maximize ROAS</li>
                        <li>Design and launch Meta ad campaigns with strategic targeting, achieving cost-efficient customer acquisition</li>
                    </ul>
                </div>
                
                <div class="experience-item">
                    <div class="job-header">
                        <div>
                            <div class="job-title">Freelance Digital Marketing Specialist</div>
                            <div class="company">Self-Employed</div>
                        </div>
                        <div class="date-location">
                            <div>Jan 2025 – Present</div>
                            <div>Pune, Maharashtra</div>
                        </div>
                    </div>
                    <ul class="responsibilities">
                        <li>Spearhead digital marketing initiatives, expanding brand reach for B2B enterprise publication</li>
                        <li>Collaborate with editorial teams to create compelling content for C-suite executives, driving measurable engagement</li>
                        <li>Manage end-to-end social media strategies across Facebook, Instagram, and LinkedIn, increasing engagement rates</li>
                        <li>Analyze campaign performance using Google Analytics, optimizing conversion rates and improving ROI by 25%+</li>
                        <li>Set up and optimize Google Ads campaigns (Search & Display), managing budgets to maximize ROAS</li>
                        <li>Design and launch Meta ad campaigns with strategic targeting, achieving cost-efficient customer acquisition</li>
                    </ul>
                </div>
            </section>
            
            <section class="section">
                <h2>Technical Skills</h2>
                <div class="skills-container">
                    <div class="skill-category">
                        <h3>Marketing Platforms & Analytics</h3>
                        <div class="skill-list">
                            <span class="skill-tag">Google Ads</span>
                            <span class="skill-tag">Google Analytics</span>
                            <span class="skill-tag">Google Tag Manager</span>
                            <span class="skill-tag">Search Console</span>
                            <span class="skill-tag">Facebook Ads Manager</span>
                            <span class="skill-tag">LinkedIn Campaign Manager</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h3>SEO & Research Tools</h3>
                        <div class="skill-list">
                            <span class="skill-tag">SEMrush</span>
                            <span class="skill-tag">Ahrefs</span>
                            <span class="skill-tag">Moz Pro</span>
                            <span class="skill-tag">Screaming Frog</span>
                            <span class="skill-tag">Ubersuggest</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h3>Marketing Automation & CRM</h3>
                        <div class="skill-list">
                            <span class="skill-tag">HubSpot</span>
                            <span class="skill-tag">Mailchimp</span>
                            <span class="skill-tag">ActiveCampaign</span>
                            <span class="skill-tag">Klaviyo</span>
                            <span class="skill-tag">Salesforce</span>
                            <span class="skill-tag">Pipedrive</span>
                            <span class="skill-tag">Zoho CRM</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h3>Lead Generation & Outreach</h3>
                        <div class="skill-list">
                            <span class="skill-tag">Apollo.io</span>
                            <span class="skill-tag">Hunter.io</span>
                            <span class="skill-tag">ZoomInfo</span>
                            <span class="skill-tag">LinkedIn Sales Navigator</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h3>Web Development & Design</h3>
                        <div class="skill-list">
                            <span class="skill-tag">WordPress</span>
                            <span class="skill-tag">Shopify</span>
                            <span class="skill-tag">WooCommerce</span>
                            <span class="skill-tag">Canva</span>
                            <span class="skill-tag">Adobe Creative Suite</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h3>Conversion & Optimization</h3>
                        <div class="skill-list">
                            <span class="skill-tag">Hotjar</span>
                            <span class="skill-tag">Crazy Egg</span>
                            <span class="skill-tag">Optimizely</span>
                            <span class="skill-tag">A/B Testing</span>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2>Core Competencies</h2>
                <div class="skill-list" style="margin-top: 20px;">
                    <span class="skill-tag">Digital Marketing Strategy</span>
                    <span class="skill-tag">SEO & Technical SEO</span>
                    <span class="skill-tag">Google Ads & PPC</span>
                    <span class="skill-tag">Paid Social Media</span>
                    <span class="skill-tag">Content Marketing</span>
                    <span class="skill-tag">Email Marketing</span>
                    <span class="skill-tag">Marketing Automation</span>
                    <span class="skill-tag">Lead Generation</span>
                    <span class="skill-tag">Conversion Optimization</span>
                    <span class="skill-tag">Data Analytics</span>
                    <span class="skill-tag">AI-Powered Marketing</span>
                    <span class="skill-tag">B2B Marketing</span>
                </div>
            </section>
            
            <section class="section">
                <h2>Featured Project</h2>
                <div class="project-item">
                    <div class="job-title">AI-Powered Campaign Strategy Project</div>
                    <ul class="responsibilities">
                        <li>Leveraged ChatGPT and Jasper.ai to develop high-performing marketing content</li>
                        <li>Implemented AI-driven ad creative optimization using Canva AI and AdCreative.ai</li>
                        <li>Conducted competitive analysis and keyword research using advanced AI tools</li>
                        <li>Achieved 40% reduction in content creation time while maintaining quality</li>
                        <li>Improved CTR through data-driven A/B testing methodologies</li>
                    </ul>
                </div>
            </section>
            
            <section class="section">
                <h2>Certifications</h2>
                <div class="cert-grid">
                    <div class="cert-card">
                        <div class="cert-name">Google Digital Marketing Certification</div>
                        <div class="cert-issuer">Google Digital Garage</div>
                    </div>
                    <div class="cert-card">
                        <div class="cert-name">Google Ads Certification</div>
                        <div class="cert-issuer">Google Skillshop</div>
                    </div>
                    <div class="cert-card">
                        <div class="cert-name">Meta Digital Marketing Associate</div>
                        <div class="cert-issuer">Meta Blueprint</div>
                    </div>
                    <div class="cert-card">
                        <div class="cert-name">HubSpot Content Marketing Certification</div>
                        <div class="cert-issuer">HubSpot Academy</div>
                    </div>
                    <div class="cert-card">
                        <div class="cert-name">Keyword Research Essentials</div>
                        <div class="cert-issuer">Semrush Academy</div>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2>Education</h2>
                <div class="experience-item">
                    <div class="job-header">
                        <div>
                            <div class="job-title">Higher Secondary (12th Science)</div>
                            <div class="company">Sir Parashurambhau College</div>
                        </div>
                        <div class="date-location">
                            <div>May 2025</div>
                            <div>Pune, Maharashtra</div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="section">
                <h2>Professional Development</h2>
                <ul class="responsibilities">
                    <li>Regular attendee of digital marketing conferences and webinars</li>
                    <li>Active member of digital marketing communities and forums</li>
                    <li>Continuous learning through industry blogs, podcasts, and online courses</li>
                    <li>Stay current with algorithm updates, platform changes, and industry trends</li>
                </ul>
            </section>
            
            <div class="download-section">
                <h2 style="color: white; border: none; margin-bottom: 10px;">Download My Resume</h2>
                <p style="font-size: 1.1em; margin-bottom: 20px;">Get a comprehensive PDF version of my professional experience and qualifications</p>
                <button class="download-btn" onclick="downloadResume()">⬇️ Download Resume PDF</button>
            </div>
        </div>
        
        <footer>
            <p>&copy; 2026 Ayush Ghodake. All rights reserved.</p>
            <p style="margin-top: 10px; opacity: 0.8;">Designed to showcase data-driven digital marketing expertise</p>
        </footer>
    </div>
    
    <script>
        function downloadResume() {
            // Create a printable version of the resume
            const resumeContent = `
AYUSH GHODAKE
Digital Marketing Specialist | Growth Strategist | AI-Powered Campaign Expert

Contact Information:
Email: ayushghodake91@gmail.com
Phone: 7758046516
Location: Pune, Maharashtra
Website: https://ayushghodake91-maker.github.io
LinkedIn: https://www.linkedin.com/in/ayush-ghodake-46

KEY ACHIEVEMENTS:
• Improved ROI by 25%+ through data-driven campaign optimization
• Reduced content creation time by 40% using AI-powered tools
• Increased email engagement by 35% with automated workflows
• Managed 100+ successful digital marketing campaigns

PROFESSIONAL EXPERIENCE:

Business Development Executive | Sep 2025 – Present
The Enterprise Globe Magazine, Pune, Maharashtra
• Spearhead digital marketing initiatives, expanding brand reach for B2B enterprise publication
• Collaborate with editorial teams to create compelling content for C-suite executives, driving measurable engagement
• Manage end-to-end social media strategies across Facebook, Instagram, and LinkedIn, increasing engagement rates
• Analyze campaign performance using Google Analytics, optimizing conversion rates and improving ROI by 25%+
• Set up and optimize Google Ads campaigns (Search & Display), managing budgets to maximize ROAS
• Design and launch Meta ad campaigns with strategic targeting, achieving cost-efficient customer acquisition

Freelance Digital Marketing Specialist | Jan 2025 – Present
Self-Employed, Pune, Maharashtra
• Execute ROI-focused campaigns across multiple industries, improving visibility and generating qualified leads for startups and SMBs
• Conduct comprehensive SEO audits using Semrush and Ubersuggest, improving organic rankings and traffic growth
• Develop comprehensive lead generation strategies across LinkedIn, Meta, email marketing, and content syndication
• Implement data-driven strategies using marketing automation to accelerate revenue growth
• Leveraged ChatGPT and Jasper.ai to generate high-performing content, reducing creation time by 40%
• Designed data-driven ad creatives using Canva AI and AdCreative.ai with A/B testing to optimize CTR
• Automated email workflows with Mailchimp AI, achieving 35% improvement in engagement metrics
• Spearhead digital marketing initiatives, expanding brand reach for B2B enterprise publication
• Collaborate with editorial teams to create compelling content for C-suite executives, driving measurable engagement
• Manage end-to-end social media strategies across Facebook, Instagram, and LinkedIn, increasing engagement rates
• Analyze campaign performance using Google Analytics, optimizing conversion rates and improving ROI by 25%+
• Set up and optimize Google Ads campaigns (Search & Display), managing budgets to maximize ROAS
• Design and launch Meta ad campaigns with strategic targeting, achieving cost-efficient customer acquisition

TECHNICAL SKILLS:
Marketing Platforms: Google Ads, Google Analytics, Google Tag Manager, Google Search Console, Facebook Ads Manager, LinkedIn Campaign Manager, Twitter Ads
SEO Tools: SEMrush, Ahrefs, Moz Pro, Screaming Frog, Ubersuggest
Marketing Automation: HubSpot, Mailchimp, ActiveCampaign, Klaviyo
Lead Generation: Apollo.io, Hunter.io, ZoomInfo, LinkedIn Sales Navigator
CRM: Salesforce, Pipedrive, Zoho CRM
Web Platforms: WordPress, Shopify, WooCommerce
Design: Canva, Adobe Creative Suite
Optimization: Hotjar, Crazy Egg, Optimizely

CERTIFICATIONS:
• Google Digital Marketing Certification – Google Digital Garage
• Google Ads Certification – Google Skillshop
• Meta Digital Marketing Associate – Meta Blueprint
• HubSpot Content Marketing Certification – HubSpot Academy
• Keyword Research Essentials with Semrush – Semrush Academy

EDUCATION:
Higher Secondary (12th Science) | May 2025
Sir Parashurambhau College, Pune, Maharashtra

FEATURED PROJECT:
AI-Powered Campaign Strategy Project
• Leveraged ChatGPT and Jasper.ai to develop high-performing marketing content
• Implemented AI-driven ad creative optimization using Canva AI and AdCreative.ai
• Achieved 40% reduction in content creation time while maintaining quality
• Improved CTR through data-driven A/B testing methodologies

Last Updated: January 1, 2026
`;

            // Create a blob with the resume content
            const blob = new Blob([resumeContent], { type: 'text/plain' });
            const url = window.URL.createObjectURL(blob);
            
            // Create a temporary link and trigger download
            const a = document.createElement('a');
            a.href = url;
            a.download = 'Ayush_Ghodake_Resume.txt';
            document.body.appendChild(a);
            a.click();
            
            // Cleanup
            window.URL.revokeObjectURL(url);
            document.body.removeChild(a);
            
            // Show success message
            const btn = event.target;
            const originalText = btn.innerHTML;
            btn.innerHTML = '✓ Resume Downloaded!';
            btn.style.background = '#34a853';
            btn.style.color = 'white';
            
            setTimeout(() => {
                btn.innerHTML = originalText;
                btn.style.background = 'white';
                btn.style.color = '#ea4335';
            }, 3000);
        }
        
        // Smooth scroll behavior
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });
        
        // Add animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);
        
        document.querySelectorAll('.section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(20px)';
            section.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(section);
        });
    </script>
</body>
</html>

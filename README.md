https://quickshare.samsungcloud.com/nwjZdQTcVyGQ      text-align: center;
      transition: transform 0.6s;
      transform-style: preserve-3d;
    }
    .flip-card:hover .flip-card-inner {
      transform: rotateY(180deg);
    }
    .flip-card-front, .flip-card-back {
      position: absolute;
      width: 100%;
      height: 100%;
      backface-visibility: hidden;
      border-radius: 14px;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.18);
    }
    .flip-card-front {
      background: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(10px);
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 18px;
      border: 2px solid rgba(255, 255, 255, 0.3);
    }
    .flip-card-front h3 {
      margin: 8px 0 4px;
      font-size: 20px;
    }
    .flip-card-front p {
      margin: 0;
      opacity: 0.9;
      font-size: 13px;
    }
    .flip-card-back {
      background: white;
      color: #2c3e50;
      transform: rotateY(180deg);
      padding: 16px;
      overflow-y: auto;
    }
    .flip-card-back h4 {
      margin: 0 0 8px;
      font-size: 14px;
      color: #667eea;
      text-align: left;
    }
    .flip-card-back ul {
      margin: 6px 0;
      padding-left: 18px;
      text-align: left;
      font-size: 11px;
      line-height: 1.5;
    }
    .flip-card-back li {
      margin-bottom: 6px;
    }
    .flip-card-back p {
      font-size: 10px;
      font-style: italic;
      margin: 8px 0 0 0;
      text-align: left;
    }
    .flip-cards-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      max-width: 600px;
      margin: 20px auto;
    }

    /* Search Box Styling */
    .search-container {
      max-width: 600px;
      margin: 20px auto 30px;
      position: relative;
    }
    .search-box {
      width: 100%;
      padding: 14px 45px 14px 20px;
      border: 2px solid rgba(255, 255, 255, 0.3);
      border-radius: 12px;
      font-size: 15px;
      background: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(10px);
      color: white;
      transition: all 0.3s ease;
    }
    .search-box::placeholder {
      color: rgba(255, 255, 255, 0.7);
    }
    .search-box:focus {
      outline: none;
      background: rgba(255, 255, 255, 0.3);
      border-color: rgba(255, 255, 255, 0.5);
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
    }
    .search-icon {
      position: absolute;
      right: 15px;
      top: 50%;
      transform: translateY(-50%);
      font-size: 20px;
      pointer-events: none;
    }
    .no-results {
      text-align: center;
      color: white;
      padding: 20px;
      font-size: 16px;
      display: none;
    }

    .section-container { max-width: 1100px; margin: 0 auto 50px; }
    .section-header { text-align: center; margin-bottom: 30px; animation: fadeInUp 0.6s ease-out; }
    .section-title {
      font-size: 28px;
      font-weight: 700;
      color: white;
      margin-bottom: 8px;
      text-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
    }
    .section-subtitle { font-size: 16px; color: rgba(255, 255, 255, 0.9); }

    /* Group Header Styling */
    .group-header {
      font-size: 16px;
      font-weight: 600;
      color: white;
      margin: 25px 0 12px 0;
      text-align: center;
      text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      border: none;
      border-radius: 16px;
      padding: 28px;
      text-align: center;
      cursor: pointer;
      transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
      position: relative;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
      overflow: hidden;
      animation: fadeInUp 0.6s ease-out forwards;
      opacity: 0;
    }

    .card:nth-child(1) { animation-delay: 0.1s; }
    .card:nth-child(2) { animation-delay: 0.15s; }
    .card:nth-child(3) { animation-delay: 0.2s; }
    .card:nth-child(4) { animation-delay: 0.25s; }
    .card:nth-child(5) { animation-delay: 0.3s; }
    .card:nth-child(6) { animation-delay: 0.35s; }
    .card:nth-child(7) { animation-delay: 0.4s; }
    .card:nth-child(8) { animation-delay: 0.45s; }
    .card:nth-child(9) { animation-delay: 0.5s; }
    .card:nth-child(10){ animation-delay: 0.55s; }
    .card:nth-child(11){ animation-delay: 0.6s; }
    .card:nth-child(12){ animation-delay: 0.65s; }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px) scale(0.95); }
      to { opacity: 1; transform: translateY(0) scale(1); }
    }
    @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

    .card::before {
      content: '';
      position: absolute;
      top: 0; left: -100%;
      width: 100%; height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
      transition: left 0.6s ease;
    }
    .card:hover::before { left: 100%; }
    .card:hover { transform: translateY(-10px) scale(1.02); box-shadow: 0 25px 50px rgba(0, 0, 0, 0.25); }
    .card:active { transform: translateY(-8px) scale(0.98); }

    .card-number {
      position: absolute;
      top: 14px; right: 14px;
      width: 36px; height: 36px;
      border-radius: 50%;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      font-weight: 700;
      font-size: 15px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
    }

    .card-icon {
      font-size: 48px;
      margin-bottom: 16px;
      display: inline-block;
      animation: float 3s ease-in-out infinite;
      filter: drop-shadow(0 4px 8px rgba(0, 0, 0, 0.1));
    }
    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      25% { transform: translateY(-8px) rotate(-2deg); }
      75% { transform: translateY(-8px) rotate(2deg); }
    }

    .card-title {
      font-size: 20px;
      font-weight: 700;
      color: #2c3e50;
      margin-bottom: 10px;
      line-height: 1.3;
    }

    .card-description {
      font-size: 14px;
      color: #7f8c8d;
      line-height: 1.6;
      margin-bottom: 0;
    }

    .card-tag {
      position: absolute;
      top: 14px; left: 14px;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      padding: 6px 12px;
      border-radius: 20px;
      font-size: 11px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      box-shadow: 0 4px 12px rgba(102, 126, 234, 0.3);
    }

    /* AI Tips Banner Card */
    .ai-tips-banner {
      background: white;
      border-radius: 16px;
      padding: 24px 32px;
      cursor: pointer;
      transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
      margin: 30px auto;
      max-width: 1100px;
      display: flex;
      align-items: center;
      gap: 20px;
      position: relative;
      overflow: hidden;
    }
    .ai-tips-banner::before {
      content: '';
      position: absolute;
      top: 0; left: -100%;
      width: 100%; height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
      transition: left 0.6s ease;
    }
    .ai-tips-banner:hover::before { left: 100%; }
    .ai-tips-banner:hover {
      transform: translateY(-6px) scale(1.01);
      box-shadow: 0 20px 45px rgba(0, 0, 0, 0.25);
    }
    .ai-tips-banner .banner-icon {
      font-size: 56px;
      animation: float 3s ease-in-out infinite;
      filter: drop-shadow(0 4px 8px rgba(0, 0, 0, 0.1));
    }
    .ai-tips-banner .banner-content {
      flex: 1;
    }
    .ai-tips-banner .banner-title {
      font-size: 24px;
      font-weight: 700;
      color: #2c3e50;
      margin: 0 0 6px 0;
    }
    .ai-tips-banner .banner-description {
      font-size: 14px;
      color: #7f8c8d;
      margin: 0;
    }
    .ai-tips-banner .banner-tag {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      padding: 6px 16px;
      border-radius: 20px;
      font-size: 11px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      box-shadow: 0 4px 12px rgba(102, 126, 234, 0.3);
    }
    
    /* Prompt Card Styling for Modal */
    .prompt-card {
      background: white;
      border: 1px solid #e0e0e0;
      border-radius: 12px;
      padding: 20px;
      margin-bottom: 16px;
      transition: all 0.3s ease;
    }
    .prompt-card:hover {
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      transform: translateY(-2px);
    }
    .prompt-card h4 {
      color: #667eea;
      margin: 0 0 8px 0;
      font-size: 16px;
      font-weight: 700;
    }
    .prompt-card p {
      color: #7f8c8d;
      margin: 0 0 12px 0;
      font-size: 14px;
    }
    .prompt-text {
      background: #f8f9fa;
      border: 1px solid #e0e0e0;
      border-radius: 8px;
      padding: 14px;
      font-family: 'Consolas', 'Monaco', monospace;
      font-size: 13px;
      line-height: 1.5;
      color: #2c3e50;
      margin-bottom: 10px;
      white-space: pre-wrap;
      word-wrap: break-word;
    }
    .copy-btn {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      border: none;
      padding: 8px 16px;
      border-radius: 8px;
      cursor: pointer;
      font-weight: 600;
      font-size: 13px;
      transition: all 0.3s ease;
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }
    .copy-btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 16px rgba(102, 126, 234, 0.4);
    }
    .copy-btn:active {
      transform: translateY(0);
    }
    .prompt-tip {
      font-size: 12px;
      color: #95a5a6;
      margin: 8px 0 0 0;
      font-style: italic;
    }
    
    /* Quick Reference copy buttons */
    .ref-item {
      display: flex;
      align-items: center;
      gap: 8px;
      margin-bottom: 10px;
    }
    .ref-item-content {
      flex: 1;
    }
    .mini-copy-btn {
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      border: none;
      padding: 4px 8px;
      border-radius: 6px;
      cursor: pointer;
      font-weight: 600;
      font-size: 11px;
      transition: all 0.3s ease;
      white-space: nowrap;
      flex-shrink: 0;
    }
    .mini-copy-btn:hover {
      transform: translateY(-1px);
      box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
    }
    .mini-copy-btn:active {
      transform: translateY(0);
    }

    .modal-overlay {
      display: none;
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0, 0, 0, 0.7);
      backdrop-filter: blur(4px);
      z-index: 999;
      animation: fadeIn 0.3s ease;
    }
    .modal-overlay.show { display: flex; align-items: center; justify-content: center; }
    .modal-content {
      background: white;
      border-radius: 20px;
      max-width: 900px;
      width: 90%;
      max-height: 85vh;
      overflow-y: auto;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
      animation: scaleIn 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
    }
    @keyframes scaleIn {
      from { transform: scale(0.8); opacity: 0; }
      to { transform: scale(1); opacity: 1; }
    }
    .modal-header {
      padding: 30px 30px 20px;
      border-bottom: 2px solid #ecf0f1;
      display: flex;
      align-items: center;
      gap: 20px;
      position: relative;
    }
    .modal-icon { font-size: 50px; }
    .modal-title-section { flex: 1; }
    .modal-title { font-size: 26px; font-weight: 700; color: #2c3e50; margin: 0; }
    .modal-badge {
      display: inline-block;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      padding: 4px 12px;
      border-radius: 12px;
      font-size: 12px;
      font-weight: 700;
      margin-top: 8px;
    }
    .close-btn {
      background: transparent;
      border: none;
      font-size: 36px;
      color: #95a5a6;
      cursor: pointer;
      transition: color 0.3s ease;
      line-height: 1;
      padding: 0;
      width: 36px;
      height: 36px;
    }
    .close-btn:hover { color: #e74c3c; }
    .modal-body {
      padding: 25px 30px 30px;
      color: #34495e;
      line-height: 1.8;
      font-size: 15px;
    }
    .modal-body h3 {
      color: #2c3e50;
      margin-top: 25px;
      margin-bottom: 12px;
      font-size: 18px;
    }
    .modal-body h4 {
      color: #667eea;
      margin-top: 20px;
      margin-bottom: 10px;
      font-size: 16px;
    }
    .modal-body ul {
      margin: 12px 0;
      padding-left: 25px;
    }
    .modal-body li {
      margin-bottom: 10px;
    }
    .modal-body pre {
      background: #f8f9fa;
      padding: 15px;
      border-radius: 8px;
      overflow-x: auto;
      font-size: 13px;
      line-height: 1.5;
    }

    /* System card styling */
    .sys-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 140px));
      gap: 12px;
      margin-bottom: 40px;
      max-width: 1100px;
      margin-left: auto;
      margin-right: auto;
      justify-content: center;
    }
    .sys-card {
      background: white;
      border-radius: 10px;
      padding: 12px;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 3px 12px rgba(0, 0, 0, 0.08);
      position: relative;
      overflow: hidden;
      text-align: center;
    }
    .sys-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
    }
    .sys-card::before {
      content: '';
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 2px;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    }
    .sys-tag {
      display: inline-block;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
      padding: 2px 6px;
      border-radius: 6px;
      font-size: 8px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      margin-bottom: 8px;
    }
    .sys-ico { font-size: 28px; margin: 4px 0; }
    .sys-title {
      font-size: 12px;
      font-weight: 700;
      color: #2c3e50;
      margin: 4px 0 3px;
      line-height: 1.2;
    }
    .sys-sub {
      font-size: 10px;
      color: #7f8c8d;
      margin: 0;
      line-height: 1.2;
    }
  </style>
</head>
<body>
<div class="top-bar">
<a href="https://www.nationwide.com" target="_blank">Nationwide.com</a>
<a href="https://outlook.office.com/mail/" target="_blank">Outlook</a>
<a href="https://teams.microsoft.com" target="_blank">Teams</a>
<a href="https://onyourside.sharepoint.com" target="_blank">SharePoint</a>
</div>
<div class="container">
<div class="hero-header">
<h1 class="main-title">NSS CL Inside Sales Hub</h1>
<p class="main-subtitle">Your centralized command center for tools, scripts, and workflows</p>
<!-- Flip Cards for Sales Handling and Quick Reference -->
<div class="flip-cards-container">
<!-- SALES HANDLING FLIP CARD -->
<div class="flip-card">
<div class="flip-card-inner">
<div class="flip-card-front">
<div style="font-size: 42px;">📋</div>
<h3>Sales Handling</h3>
<p>Hover for quick procedures</p>
</div>
<div class="flip-card-back">
<h4>Quick Procedures</h4>
<ul>
<li><strong>Lead Intake:</strong> Qualify prospects, verify appetite</li>
<li><strong>Quote Process:</strong> ClearQuote → PolicyCenter</li>
<li><strong>Binding:</strong> Follow bind checklist, PRD setup</li>
<li><strong>Agency Codes:</strong> Check Quick Reference →</li>
</ul>
<button onclick="openLink('https://onyourside.sharepoint.com/:u:/r/sites/CIERRATEAM/SitePages/Cierra-Inside-Sales.aspx?csf=1&amp;web=1&amp;e=BtgVwk')" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; border: none; padding: 6px 14px; border-radius: 6px; cursor: pointer; font-weight: 600; margin-top: 8px; font-size: 11px;">View Full Procedures</button>
</div>
</div>
</div>
<!-- QUICK REFERENCE FLIP CARD -->
<div class="flip-card">
<div class="flip-card-inner">
<div class="flip-card-front">
<div style="font-size: 42px;">📖</div>
<h3>Quick Reference</h3>
<p>Hover for key contacts</p>
</div>
<div class="flip-card-back">
<h4>📞 Key Contacts</h4>
<ul>
<li><strong>SC Agents:</strong> 1-800-896-2277</li>
<li><strong>SC Customers:</strong> 1-888-282-3717</li>
<li><strong>KMA:</strong> 1-800-730-8413</li>
<li><strong>Insureon:</strong> 1-877-588-2392</li>
<li><strong>IOA:</strong> 1-877-588-2380</li>
</ul>
<h4>🔗 UW &amp; Service</h4>
<ul>
<li><strong>Trevor Sharp:</strong> <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="fdaeb5bcafada9c9bd939c899492938a949998d39e9290">[email&#160;protected]</a></li>
<li><strong>UW New Business:</strong> <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="f0b1839bb3bcbe9587b28583999e958383b09e9184999f9e87999495de939f9d">[email&#160;protected]</a></li>
</ul>
<button onclick="openQuickRefModal()" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; border: none; padding: 6px 14px; border-radius: 6px; cursor: pointer; font-weight: 600; margin-top: 4px; font-size: 11px;">View All Details</button>
</div>
</div>
</div>
</div>
<!-- Search Box -->
<div class="search-container">
<input class="search-box" id="searchBox" onkeyup="searchTiles()" placeholder="Search for systems, tools, or resources..." type="text"/>
<span class="search-icon">🔍</span>
</div>
<div class="no-results" id="noResults">No results found. Try a different search term.</div>
</div>
<!-- AI TIPS BANNER CARD -->
<div class="ai-tips-banner" onclick="openAITipsModal()">
<span class="banner-icon">🤖</span>
<div class="banner-content">
<h3 class="banner-title">AI Tips &amp; Prompts</h3>
<p class="banner-description">Copy-ready prompts for underwriting questions, checklists, CLNSS formatting, coverage summaries, and professional email support</p>
</div>
<span class="banner-tag">Click to View</span>
</div>
<!-- MAIN SYSTEMS SECTION -->
<div class="section-container">
<h2 class="group-header">🚀 Core Systems</h2>
<div class="sys-grid"><div class="sys-card" onclick="openLink('https://clnss.lightning.force.com/lightning/page/home')" title="Salesforce">
<div class="sys-tag">PRIMARY</div>
<div class="sys-ico">☁️</div>
<div class="sys-title">Salesforce (Amplo/Veruna)</div>
<p class="sys-sub">CRM + sales management</p>
</div><div class="sys-card" onclick="openLink('https://clpolicycenter.apps.nwie.net/pc/service/launch/PolicyCenter.do')" title="PolicyCenter">
<div class="sys-tag">POLICY</div>
<div class="sys-ico" style="display:flex;align-items:center;justify-content:center;height:38px;margin:4px 0;">
  <img src="data:image/png;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/4gHYSUNDX1BST0ZJTEUAAQEAAAHIAAAAAAQwAABtbnRyUkdCIFhZWiAH4AABAAEAAAAAAABhY3NwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQAA9tYAAQAAAADTLQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAlkZXNjAAAA8AAAACRyWFlaAAABFAAAABRnWFlaAAABKAAAABRiWFlaAAABPAAAABR3dHB0AAABUAAAABRyVFJDAAABZAAAAChnVFJDAAABZAAAAChiVFJDAAABZAAAAChjcHJ0AAABjAAAADxtbHVjAAAAAAAAAAEAAAAMZW5VUwAAAAgAAAAcAHMAUgBHAEJYWVogAAAAAAAAb6IAADj1AAADkFhZWiAAAAAAAABimQAAt4UAABjaWFlaIAAAAAAAACSgAAAPhAAAts9YWVogAAAAAAAA9tYAAQAAAADTLXBhcmEAAAAAAAQAAAACZmYAAPKnAAANWQAAE9AAAApbAAAAAAAAAABtbHVjAAAAAAAAAAEAAAAMZW5VUwAAACAAAAAcAEcAbwBvAGcAbABlACAASQBuAGMALgAgADIAMAAxADb/2wBDAAUDBAQEAwUEBAQFBQUGBwwIBwcHBw8LCwkMEQ8SEhEPERETFhwXExQaFRERGCEYGh0dHx8fExciJCIeJBweHx7/2wBDAQUFBQcGBw4ICA4eFBEUHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh7/wAARCAAtAKcDASIAAhEBAxEB/8QAGwABAAIDAQEAAAAAAAAAAAAAAAUGAQcIBAP/xAA8EAABAwQBAQUDBwsFAAAAAAABAgMEAAUGERIHCBMUITEVUWEWGCJBVXGBCRcyNEJScpGUsdNDY2el4//EABgBAQEBAQEAAAAAAAAAAAAAAAABAgME/8QAHhEBAQEAAgMAAwAAAAAAAAAAAAERAjEDEiEiMmH/2gAMAwEAAhEDEQA/AOYaVvPsq9HsZ6qtZEvIZ13im2KjBnwDraOXed7y5c0K3+gNa19dbv8AmhdNftzLf6uP/gr2cvJx43K804WzXDtK7i+aF01+3Mt/q4/+Ctd9ojs94X076ZScnslzyCRMakMtJRMfZU2QtWjsJaSd/jSeXjbi3hY5hpSldGClKyhKlrCEJKlKOgANkmgxSsrSpCyhaSlSTogjRBrFApSlApSlApSlApSlApSlApSlB1x+Tw/V83/jg/2kVpXKsUuOcdpbJMWtL0VmbPyG4JaXJUpLYKXHVnkUpUfRJ9Aa3V+Tw/V83/jg/wBpFayzPHOrFj685HluJ4jk6ZDd8mvQprNlcfQpK3HByTybUhQKVHR0R57FcZfzrpf1ic+aF1K+3MS/q5H+Cqt1S7PeadO8Reya93PH5ENp1DSkQ33lOErOhoKaSNfjXvyDrh2h8dkNxsgu9ztD7qObbc6wx2FLTvXIBbIJGxrddAdraQ9L7MaJchfN55UFxxWgOSlEEnQ8vU09ucs0zjZccJV0O5bOoaMewkYXgduvFokWCM5KL2OxpDTr5W4F948tvkPII2eY0PPy9a54q59Ubpb7nHw9MCU3IMPGo0WQEf6bqXHSpB+ICh/OunKaxLiczvBIMvN8lmY3NtFqxSFNEdE2VLIjB8oClsNKAUp3SueuIV9EAnQI3HYzjFyxrqphYmKiyIs26Q3oc2I8HY8lHiEpJQse5QIKTpQI0QK9VjFqy7pdb8VVkFssd2stxky20XF0ssTGn0NAkOaIDiC1rStbCvI+RFSbl1sFhn9N8XavsO6CxXo3C5XGOVGM0XXmCW21qAKkoSzyKgNEqOt6rO3pfnat3iPcHGM8kR7fbHobV0bEmS+0DIjkvO8Ayr1SFEEK16gCvNDwC6O26DKmXOyWt64tB2BEnTQ09IQTpKgNEISo70pwoB9d686lHrvbE431HieNZL1wukVyGkK33yUvvFSkkeRACgfxqUyu3WDPJ0DKWM2sNmZVboka4Q56nEvw3GGEMqDbaUEupUGwpPD97R1omrtMUC8Y5crVY7VepKWVQrr3wjONOBf0ml8HEq16EEg/EKB9DV5xzCmMVOU3vM7exPXjUaJwtnektuS5Xmyh4p0eKEhalpBGynjv1FSHQ+RZLlZLvZMkWXbZjkhOUMK4HTgZIbeY+AeCmgPige+oHFM0iXG4ZZAzWQ6iBlx72XNZbK1xJSXC408Eb+kgKUoKSPPio68wAVt6Mj4r6p3uVGkwLtZsZuFrfbUhMH2MxHQyoghK21MpQtCkk72Fefod1D2DDbhdbMb0/PtdothfMdqTcZHdJedABUltIBUrQI2QNDY2RuphOC2CE6qTeOouOKtiElQXbFOSZLx+pKGShJCj71lAHvq0Yxe7feOllks0K44hBu9ickofYyGG0oSGnXC4lxpxaFAKBUUlGwToEU3OjvtR4fT3J5eWvYvHjR13FuIqajUlHdPMBvvA425vipKkeYO9fdXxvWFz7bZUXlm5Wi52/wASmK+/Ald4mM8oEpS4CARsJVpQBSeJ0TV1ayuKc3uqp+QWyWxGxGdaokmFB8JHUtUVwJabQACR3jhSFEDfl5Aaqp45coMfpZl1rflIRLmTLc5HZJ+k4Gy/zI+7mP51dqZEh1IwOJjdnx6bBvNuluTrY2++y1L7xbjqnnUcmkhI23pCR94VXmk9M79HU/EVNsy7zHZU89ZkTUqmoSlPJSeGuJWlIJLYUVjR8tjVS93udt9n9Psri3K3STYYceNLtinSmSXWpbrpHDWigpWk8t68yPUaq43zIo0LKZeZWHLsBagOOOzoLosjS7olatqS0tru+Qc5HiVlQT6q39VZ2xcjVuO4BeLzjQybxtpt1m8U5EVMnyw0hLqEoVw1oqKiHAQEgk8Ve41K4zmVtiMWFu6xoU1mAzO7+O5BRp0mOtDCVKCdnzVre/Le/UA1HXC6QnOjVos6JSDNayCdJdjg+aW1sRUoWR7iULA+41T61m9puLLn8zH5Em3xMbClQYEUxkurYDbj5DiyXV+8q5cvMnQIT+zSq1StRG3Ozv1p/NG3e0fJr217VLB347w/dd13n+2vlvvPhrX17rbHzzf+N/8Au/8AwrkulYvj427Wpzs+Nl9oHqr+djIrdd/YPsbwUTw3deL8Rz+mVct8Ea9da0atPVXtCfLrpY1g3yR9n8BHHi/aXe77rX7HdJ9dfveXxrRdKvpPn8T2pSlK0hSlKBSlKCwtZZJj4W/i8G122E1LUgz5rSXDJmJQsrQhalLKQkK0dISnZSknZFV6lKBSlKBSlKBSlKBSlKBSlKD/2Q==" alt="PolicyCenter" style="width:108px;height:auto;mix-blend-mode:multiply;"/>
</div>
<div class="sys-title">PolicyCenter</div>
<p class="sys-sub">Quote, issue, PRD, docs</p>
</div><div class="sys-card" onclick="openLink('https://clearquote.apps.nwie.net/?_gl=1*4banrq*_ga*Nzg1ODE2OTc1LjE3NzE1MjM3NTc.*_ga_GLJSQEPWL4*czE3NzE5MDgzNjIkbzckZzEkdDE3NzE5MDkxNTIkajEwJGwwJGgwdg==')" title="ClearQuote"><div class="sys-tag">QUOTE</div><div class="sys-ico" style="display:flex;align-items:center;justify-content:center;height:38px;margin:4px 0;"><img src="data:image/png;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/4gHYSUNDX1BST0ZJTEUAAQEAAAHIAAAAAAQwAABtbnRyUkdCIFhZWiAH4AABAAEAAAAAAABhY3NwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQAA9tYAAQAAAADTLQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAlkZXNjAAAA8AAAACRyWFlaAAABFAAAABRnWFlaAAABKAAAABRiWFlaAAABPAAAABR3dHB0AAABUAAAABRyVFJDAAABZAAAAChnVFJDAAABZAAAAChiVFJDAAABZAAAAChjcHJ0AAABjAAAADxtbHVjAAAAAAAAAAEAAAAMZW5VUwAAAAgAAAAcAHMAUgBHAEJYWVogAAAAAAAAb6IAADj1AAADkFhZWiAAAAAAAABimQAAt4UAABjaWFlaIAAAAAAAACSgAAAPhAAAts9YWVogAAAAAAAA9tYAAQAAAADTLXBhcmEAAAAAAAQAAAACZmYAAPKnAAANWQAAE9AAAApbAAAAAAAAAABtbHVjAAAAAAAAAAEAAAAMZW5VUwAAACAAAAAcAEcAbwBvAGcAbABlACAASQBuAGMALgAgADIAMAAxADb/2wBDAAUDBAQEAwUEBAQFBQUGBwwIBwcHBw8LCwkMEQ8SEhEPERETFhwXExQaFRERGCEYGh0dHx8fExciJCIeJBweHx7/2wBDAQUFBQcGBw4ICA4eFBEUHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh7/wAARCAAdAG0DASIAAhEBAxEB/8QAGwAAAwACAwAAAAAAAAAAAAAAAAYHBAUBAgP/xAAsEAABBAEDAwMEAQUAAAAAAAABAgMEBREABhIHEyEiMUEUFSNRMhYzQoGh/8QAFgEBAQEAAAAAAAAAAAAAAAAAAQAC/8QAJREAAgECBgEFAQAAAAAAAAAAAREAIfACMUGxwdFREiJhceGh/9oADAMBAAIRAxEAPwCZaNGqZuiXC2FDpqWsoaWZMfgMT502xhIlKcW6OXbQFghKAMDwAT+9WQZ+t+oOqu6yZ6NUiGzA3Vtbcsys27AgTH59YxHaaGQ244XEr7ZV5QlSgDxBwPA+NZF50hm19baOsSrV2VVsKff79I9HiuJR/cDT6jhZHkjKU8gPGrF7W9OgeZpMgCS/RqijpmlzbEi1ZtLLvMVpsPzUrrMR0JTyUht9RHJQGf8AHBx4PzrL2/06o3N1bYqZt+9KftI7U5+I1DKO2wpgulPc5H1eOIwPY58e2n0+bz6MyCwxduS/Rqk7e3XV328YtLM2dt5qksZCIaWY8FCJEdK1cUrS+B3CsZBJJIOPYZ1ot5bPG3ojUkT/AKgO2kyAEdrjx+nWlPLOfPLl7YGMfOrDhOIgDX87EaNa/hPBino1QrTp3ApX7l693KqJW19gK9l5qAXXZL3ALOG+YCQEnJJVrYMbD25W1e4nLazkzUt1UexrJkWJkFl11CUucS6n1ElSShXgeTkkAayCCGLo9ogMgeSv6t5LdMFbs3cNhWMWMWGwWZIWYyXJjLbsjh/LtNKWFuYII9KT5GPfTnU9HLCZDr0vSbRqfYRkvshqledht8xlCXZAOEkgjOEqCfk6NvW1ExTx6betnV2NbCZdbXXv1zybGI6lSz2477aeJBXxPrcAxkFIx5cVGNbcyKojKKx6ebyG5P6dNKv7n9L9Z2e83js4/ny5ccf79/HvpV1e1dXaQ79CQGRWhwo+79pfcMUsZ7HDhzx38Kz/AMx51BNF3ecYadG95VFjS18Ddm2VWz9a2GIsyPPMV3sA5DS/QsLA9gcAgfOkvRrT0lHRW+m48ezZp6GLVJlSoUiMlhwlMcxiopyFAlajyGVZHkZx5177p3zU3TVg+jbcmLZT0/kd+7uKjtrJytaGQkYz58FSgM+2kTRrJDzugHAi6uU6x6qx5qLSQqglpsLOqVXSF/dlGOnLfDmhko9PsDjkfnGM50tzd6zjuWlv61kQpdTDjRm8r7gWWUBHI+B4UM5T+jjOlXRrRPe/ZmUEr06lX2r1T27t+1lT4WxlMqnKbXJZTYhUdK0K5BxttTRKFAklPqIGlxveNZKpGK2/opVmYtg/NYdTY9kqLuCpDuGzzBKQcpKD+saS9GoEgsXaj83kuZQrTqJAupFy1e7aVLrbGwFgywzPLTsV7gEHDnAhQKRggp11c6ixZM+wRO24lVPJq2qxmDHmFtTDLS0rRhwpVyOQckp85+NT/RrIAAQui2pJ1d5veUJXUOumQ4KrjbkmZYQoqYqXmbZxhp5KBhsutpTlSgMZKVJzjU+WorWVKJJJySTnXGjSaly0UNGjRqlP/9k=" alt="ClearQuote" style="width:96px;height:auto;mix-blend-mode:multiply;"/></div><div class="sys-title">ClearQuote</div><p class="sys-sub">Quote setup &amp; readiness</p></div><div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/sites/NSSCLDirect')" title="Inside Sales Home">
<div class="sys-tag">HUB</div>
<div class="sys-ico">🏠</div>
<div class="sys-title">Inside Sales Home</div>
<p class="sys-sub">Main SharePoint site</p>
</div>
<!-- Alphabetically ordered cards for Core Systems -->
<div class="sys-card" onclick="openLink('https://agentcenter.nwie.net/home')" title="Agent Center">
<div class="sys-tag">AGENT</div>
<div class="sys-ico">🧭</div>
<div class="sys-title">Agent Center</div>
<p class="sys-sub">Agent-facing workflows</p>
</div>
<div class="sys-card" onclick="openLink('https://clnss.lightning.force.com/lightning/r/Report/00OVu000006RSb3MAG/view?queryScope=userFolders')" title="Agent Pipeline Report">
<div class="sys-tag">REPORTS</div>
<div class="sys-ico">📊</div>
<div class="sys-title">Agent Pipeline Report</div>
<p class="sys-sub">Salesforce pipeline tracking</p>
</div>
<div class="sys-card" onclick="openLink('https://app.askkodiak.com/#/carriers')" title="Ask Kodiak">
<div class="sys-tag">APPETITE</div>
<div class="sys-ico">🧭</div>
<div class="sys-title">Ask Kodiak</div>
<p class="sys-sub">Carrier appetite search</p>
</div>
<div class="sys-card" onclick="openLink('https://nwpcknowledge.nationwide.com/')" title="PCKC Knowledge">
<div class="sys-tag">KNOWLEDGE</div>
<div class="sys-ico">📚</div>
<div class="sys-title">PCKC Knowledge</div>
<p class="sys-sub">Nationwide knowledge base</p>
</div>

<div class="sys-card" onclick="openLink('https://app.powerbi.com/links/sOR2l6hJ0s?ctid=22140e4c-d390-45c2-b297-a26c516dc461&amp;pbi_source=linkShare')" title="Power BI Reports">
<div class="sys-tag">ANALYTICS</div>
<div class="sys-ico">📈</div>
<div class="sys-title">Power BI Reports</div>
<p class="sys-sub">Business intelligence dashboards</p>
</div>

<div class="sys-card" onclick="openLink('https://www.secstates.com/')" title="Secretary of State">
<div class="sys-tag">SEARCH</div>
<div class="sys-ico">🏛️</div>
<div class="sys-title">Secretary of State</div>
<p class="sys-sub">Business entity verification</p>
</div>
<div class="sys-card" onclick="openLink('https://gateway-login.verisk.com/app/prometrix/auth/login')" title="Verisk Prometrix">
<div class="sys-tag">VERISK</div>
<div class="sys-ico">🏢</div>
<div class="sys-title">Verisk Prometrix</div>
<p class="sys-sub">Verisk login + Prometrix access</p>
</div>
<div class="sys-card" onclick="openLink('https://inside.nationwide.com/')" title="Inside"><div class="sys-tag">INTRANET</div><div class="sys-ico" style="display:flex;align-items:center;justify-content:center;height:38px;margin:4px 0;"><img src="data:image/png;base64,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" alt="InSide" style="width:72px;height:auto;mix-blend-mode:multiply;"/></div><div class="sys-title">Inside</div><p class="sys-sub">Nationwide intranet</p></div><div class="sys-card" onclick="openLink('https://www.docusign.com/')" title="DocuSign"><div class="sys-tag">ESIGN</div><div class="sys-ico">✍️</div><div class="sys-title">DocuSign</div><p class="sys-sub">E-signature for client documents</p></div></div>
<h2 class="group-header">🏠 Inside Sales Resources</h2>
<div class="sys-grid">
<!-- Alphabetically ordered cards for Inside Sales Resources -->
<div class="sys-card" onclick="openLink('https://forms.office.com/r/SfcW0WC7rQ')" title="All In One Form">
<div class="sys-tag">FORM</div>
<div class="sys-ico">📝</div>
<div class="sys-title">All In One Form</div>
<p class="sys-sub">Unified submission form</p>
</div>
<div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/sites/NSSCLDirect/Inside%20Sales%20Document/Cross-Sell/Cross-Sell%20List%20Ongoing.xlsx?d=w40c4791f6e84489a8614bfa7fb3e4bf4&amp;csf=1&amp;web=1&amp;e=tCtrvt')" title="Cross-Sell List">
<div class="sys-tag">SALES</div>
<div class="sys-ico">💼</div>
<div class="sys-title">Cross-Sell List</div>
<p class="sys-sub">Ongoing cross-sell opportunities</p>
</div>
<div class="sys-card" onclick="openLink('https://planner.cloud.microsoft/webui/plan/2gOdG9Cn7kWxhG6dZzbpmWQAFCaf/view/board?tid=22140e4c-d390-45c2-b297-a26c516dc461')" title="Daily Tasks &amp; Problems">
<div class="sys-tag">PLANNER</div>
<div class="sys-ico">✅</div>
<div class="sys-title">Daily Tasks &amp; Problems</div>
<p class="sys-sub">Task management board</p>
</div>
<div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/sites/NSSCLDirect/SitePages/Inside-Sales-Handling-Procedures.aspx')" title="Handling Procedures">
<div class="sys-tag">GUIDE</div>
<div class="sys-ico">📖</div>
<div class="sys-title">Handling Procedures</div>
<p class="sys-sub">Process documentation</p>
</div>
<div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/sites/NSSCLDirect/SitePages/NSS-CL-Inside-Sales.aspx')" title="Huddle Board">
<div class="sys-tag">BOARD</div>
<div class="sys-ico">📋</div>
<div class="sys-title">Huddle Board</div>
<p class="sys-sub">Team huddle dashboard</p>
</div>
<div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/:p:/r/sites/NSSCLDirect/Inside%20Sales%20Document/Archive/Inside%20Sales%202026%20Team%20Plans.pptx?d=w87f77cc73e834af2b5bfe5e865680571&amp;csf=1&amp;web=1&amp;e=aoNk4q')" title="2026 Team Plans">
<div class="sys-tag">PLAN</div>
<div class="sys-ico">🗂️</div>
<div class="sys-title">Inside Sales 2026 Plans</div>
<p class="sys-sub">Team plan deck (PPT)</p>
</div>

<div class="sys-card" onclick="openLink('https://onyourside-my.sharepoint.com/:o:/g/personal/moraj13_nationwide_com/EhEHrprw8DRFlR39ussBnaQBcCAj3M1o1e33E4ngT4RDbg')" title="Team OneNote">
<div class="sys-tag">NOTES</div>
<div class="sys-ico">📓</div>
<div class="sys-title">Team OneNote</div>
<p class="sys-sub">Shared team notebook</p>
</div>
</div>
<h2 class="group-header">📧 Underwriting &amp; Support</h2>
<div class="sys-grid"><div class="sys-card" onclick="openLink('https://referenceconnect.guidewire.com/')" title="ReferenceConnect"><div class="sys-tag">UW REF</div><div class="sys-ico">📘</div><div class="sys-title">ReferenceConnect</div><p class="sys-sub">Underwriting guidelines &amp; references</p></div>
<!-- Alphabetically ordered cards for Underwriting & Support -->
<div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/:b:/s/AppetiteSprints/IQCMhKzOqdXwTYTc5XYBye-oAfJM6HM3H1sEtMtmYxGVrqc?e=bFZ3O4')" title="Appetite Sprint Updates">
<div class="sys-tag">UPDATE</div>
<div class="sys-ico">🔁</div>
<div class="sys-title">Appetite Sprint Updates</div>
<p class="sys-sub">Latest appetite sprint artifact</p>
</div>
<div class="sys-card" onclick="openLink('https://commservicing.nwie.net/certificate/acentry.htm?_gl=1*1dnt0vc*_ga*OTUyNzQxMTA1LjE3NzAxMzQ5MjY.*_ga_GLJSQEPWL4*czE3NzEyNTg1NjQkbzkkZzEkdDE3NzEyNTg3NjQkajU4JGwwJGgw')" title="Certificates of Insurance">
<div class="sys-tag">COI</div>
<div class="sys-ico">🧾</div>
<div class="sys-title">Certificates of Insurance</div>
<p class="sys-sub">COI entry (AC Entry)</p>
</div>
<div class="sys-card" onclick="openLink('https://nwpcknowledge.nationwide.com/groups/59210/posts/5798822-premium-audit-minimum-payroll-state-specific-information?words=Premium&amp;words=Audit&amp;words=-&amp;words=Minimum&amp;words=Payroll/State&amp;words=Specific&amp;words=Information#State_Information')" title="Premium Audit Info">
<div class="sys-tag">REF</div>
<div class="sys-ico">🧾</div>
<div class="sys-title">Premium Audit Info</div>
<p class="sys-sub">Minimum payroll/state-specific reference</p>
</div>
<div class="sys-card" onclick="openLink('https://onyourside.sharepoint.com/sites/SmallCommercialIdentityandAppetite')" title="Small Commercial Identity &amp; Appetite">
<div class="sys-tag">SITE</div>
<div class="sys-ico">📌</div>
<div class="sys-title">Small Comm Appetite Site</div>
<p class="sys-sub">Identity + appetite monitoring</p>
</div>
<div class="sys-card" onclick="openLink('mailto:AskCLExistingBusiness@nationwide.com')" title="UW Existing Business">
<div class="sys-tag">UW</div>
<div class="sys-ico">✉️</div>
<div class="sys-title">UW Existing Business</div>
<p class="sys-sub"><a class="__cf_email__" data-cfemail="a9e8dac2eae5ecd1c0daddc0c7ceebdcdac0c7ccdadae9c7c8ddc0c6c7dec0cdcc87cac6c4" href="/cdn-cgi/l/email-protection">[email protected]</a></p>
</div>
<div class="sys-card" onclick="openLink('mailto:AskCLNewBusiness@nationwide.com')" title="UW New Business">
<div class="sys-tag">UW</div>
<div class="sys-ico">✉️</div>
<div class="sys-title">UW New Business</div>
<p class="sys-sub"><a class="__cf_email__" data-cfemail="3f7e4c547c73715a487d4a4c56515a4c4c7f515e4b56505148565b5a115c5052" href="/cdn-cgi/l/email-protection">[email protected]</a></p>
</div>
</div>
<h2 class="group-header">🤖 AI Agents</h2>
<div class="sys-grid">
<!-- Alphabetically ordered cards for AI Agents -->
<div class="sys-card" onclick="openLink('https://teams.microsoft.com/l/app/f6405520-7907-4464-8f6e-9889e2fb7d8f?templateInstanceId=2c02fb02-638f-4794-b04d-da8dea6be7e0&amp;environment=Default-22140e4c-d390-45c2-b297-a26c516dc461')" title="AgentWriter">
<div class="sys-tag">AI</div>
<div class="sys-ico">✍️</div>
<div class="sys-title">AgentWriter</div>
<p class="sys-sub">Draft emails fast</p>
</div>
<div class="sys-card" onclick="openLink('https://teams.microsoft.com/l/app/f6405520-7907-4464-8f6e-9889e2fb7d8f?templateInstanceId=a4d062d3-c9ab-4ea1-9f61-da5a7d7ded1d&amp;environment=Default-22140e4c-d390-45c2-b297-a26c516dc461')" title="Dash">
<div class="sys-tag">AI</div>
<div class="sys-ico">🛠️</div>
<div class="sys-title">CL Sidekick</div>
<p class="sys-sub">General support tool</p>
</div>
<div class="sys-card" onclick="openLink('https://teams.microsoft.com/l/app/f6405520-7907-4464-8f6e-9889e2fb7d8f?templateInstanceId=00a01ab3-4aa3-4d71-aa75-b25d881c5889&amp;environment=Default-22140e4c-d390-45c2-b297-a26c516dc461')" title="Scout">
<div class="sys-tag">AI</div>
<div class="sys-ico">🧠</div>
<div class="sys-title">Scout UW Coach</div>
<p class="sys-sub">Classification + UW help</p>
</div>
</div>
<h2 class="group-header">👥 People &amp; HR</h2>
<div class="sys-grid">
<!-- Alphabetically ordered cards for People & HR -->
<div class="sys-card" onclick="openLink('https://hrconnect.nationwide.com/')" title="HR Connect">
<div class="sys-tag">HR</div>
<div class="sys-ico">👥</div>
<div class="sys-title">HR Connect</div>
<p class="sys-sub">HR resources + support</p>
</div>
<div class="sys-card" onclick="openLink('https://www.myworkday.com/nationwide/d/inst/13102!CK5mGhIKBggDEMenAhIICgYI1A0QmQE~*mMeOGB47owk~/cacheable-task/12709$14.htmld')" title="Time Entry/Request Off">
<div class="sys-tag">TIME</div>
<div class="sys-ico">🕐</div>
<div class="sys-title">Time Entry/Request Off</div>
<p class="sys-sub">Enter time + request time off</p>
</div>
<div class="sys-card" onclick="openLink('https://www.myworkday.com/nationwide/learning')" title="Workday Learning">
<div class="sys-tag">LEARN</div>
<div class="sys-ico">🎓</div>
<div class="sys-title">Workday Learning</div>
<p class="sys-sub">Training + learning modules</p>
</div>
</div>
</div>
<!-- Modal -->
<div class="modal-overlay" id="modal" onclick="closeModal(event)">
<div class="modal-content" onclick="event.stopPropagation()">
<div class="modal-header">
<div class="modal-icon" id="modal-icon"></div>
<div class="modal-title-section">
<h2 class="modal-title" id="modal-title"></h2>
<div class="modal-badge" id="modal-badge"></div>
</div>
<button class="close-btn" onclick="closeModal()">×</button>
</div>
<div class="modal-body" id="modal-body"></div>
</div>
</div>
</div>
<script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script>
    function openLink(url){
      window.open(url, '_blank', 'noopener,noreferrer');
    }

    function scrollToSection(id) {
      const element = document.getElementById(id);
      if (element) {
        element.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }
    }

    function closeModal(event) {
      if (event && event.target !== event.currentTarget) return;
      document.getElementById('modal').classList.remove('show');
    }

    function openModal(icon, title, badge, content) {
      document.getElementById('modal-icon').textContent = icon;
      document.getElementById('modal-title').textContent = title;
      document.getElementById('modal-badge').textContent = badge;
      document.getElementById('modal-body').innerHTML = content;
      document.getElementById('modal').classList.add('show');
    }

    // Search functionality
    function searchTiles() {
      const searchInput = document.getElementById('searchBox').value.toLowerCase();
      const tiles = document.querySelectorAll('.sys-card');
      const sections = document.querySelectorAll('.section-container');
      let visibleCount = 0;

      tiles.forEach(tile => {
        const title = tile.querySelector('.sys-title').textContent.toLowerCase();
        const subtitle = tile.querySelector('.sys-sub').textContent.toLowerCase();
        const tag = tile.querySelector('.sys-tag').textContent.toLowerCase();
        
        const isMatch = title.includes(searchInput) || 
                       subtitle.includes(searchInput) || 
                       tag.includes(searchInput);
        
        if (isMatch || searchInput === '') {
          tile.style.display = '';
          visibleCount++;
        } else {
          tile.style.display = 'none';
        }
      });

      // Show/hide sections based on visible tiles
      sections.forEach(section => {
        const sectionTiles = section.querySelectorAll('.sys-card');
        const visibleInSection = Array.from(sectionTiles).some(tile => tile.style.display !== 'none');
        const header = section.querySelector('.group-header');
        
        if (header) {
          header.style.display = visibleInSection || searchInput === '' ? '' : 'none';
        }
      });

      // Show/hide no results message
      const noResults = document.getElementById('noResults');
      if (visibleCount === 0 && searchInput !== '') {
        noResults.style.display = 'block';
      } else {
        noResults.style.display = 'none';
      }
    }

    function openAITipsModal() {
      const content = `
        <div style="background:#0ea5e9;color:white;padding:20px;border-radius:12px;margin-bottom:20px;">
          <h2 style="margin:0 0 8px 0;font-size:1.6rem;font-weight:700;">AI Tips & Prompts — Agent Training</h2>
          <p style="margin:0;font-size:0.95rem;opacity:0.95;">Practical, call-ready AI guidance tailored for Inside Sales: underwriting questions, checklists, forms, CLNSS formatting, coverage summaries, and professional email support.</p>
        </div>

        <div style="background:#f8f9fa;border:1px solid #e0e0e0;padding:16px;border-radius:10px;margin-bottom:20px;">
          <h3 style="margin:0 0 10px 0;color:#667eea;font-size:1.2rem;">Quick View: What This Section Helps You Do</h3>
          <ul style="margin:0;padding-left:20px;font-size:0.9rem;line-height:1.6;color:#2c3e50;">
            <li>Create clean agent-ready <strong>email checklists</strong> with Yes/No fields.</li>
            <li>Generate simple <strong>underwriting question forms</strong> for WC, Auto, BOP, GL & Property.</li>
            <li>Extract ACORD/email/PDF data into <strong>Salesforce-ready CLNSS format</strong>.</li>
            <li>Identify correct <strong>SIC/NAICS and class codes</strong> with appetite notes.</li>
            <li>Produce <strong>coverage summaries</strong> & <strong>side-by-side comparisons</strong>.</li>
            <li>Rewrite emails for <strong>professional, clear communication</strong>.</li>
            <li>Draft <strong>neutral, compliant declination statements</strong>.</li>
            <li>Pull all data into clean, organized, easy-to-copy blocks.</li>
          </ul>
        </div>

        <div style="background:#f8f9fa;border:1px solid #e0e0e0;padding:18px;border-radius:10px;margin-bottom:20px;">
          <h3 style="margin:0 0 10px 0;color:#667eea;font-size:1.2rem;">Tip: Set Up Copilot Personalization</h3>
          <p style="margin:0 0 8px 0;font-size:0.9rem;color:#2c3e50;">Paste the following into your Copilot Personalization settings to ensure responses align with Inside Sales, CLNSS, underwriting, and quoting workflows.</p>
          <div style="background:#fff;border:1px solid #e0e0e0;border-radius:8px;padding:12px;font:13px/1.5 monospace;white-space:pre-wrap;overflow-x:auto;max-height:300px;overflow-y:auto;color:#2c3e50;">I am an Inside Sales Agent supporting Nationwide Commercial Lines.

My work involves:
- Lead intake and qualification
- Quoting and binding commercial policies
- Managing opportunities in Salesforce (CLNSS)
- Using ClearQuote for quote setup and readiness
- Using PolicyCenter (Commercial Lines) for policy lifecycle steps
- Using Agent Center for agent-facing workflows and servicing guidance
- Using SharePoint resources and NWPC Knowledge

When answering sales, quoting, underwriting, or policy questions:
- Use Nationwide systems and Microsoft 365 content I have access to
- Identify which system the answer is based on (CLNSS, ClearQuote, PolicyCenter, Agent Center, SharePoint)
- If required information is not accessible, say so instead of guessing
- Keep responses concise, practical, and usable during live sales calls
- Provide step-by-step guidance, checklists, talk tracks, or email templates

When creating a form, format, template, checklist, procedure, or workflow:
- Present it in checklist or bullet-point style
- Keep content simple, clear, and easy to follow
- Use step-by-step flow when appropriate
- Prioritize readability and actionability (usable during calls, quoting, or Salesforce work)</div>
          <p style="margin-top:8px;font-size:0.8rem;color:#7f8c8d;">Tip: Update these personalization settings every few months as processes evolve or systems change.</p>
        </div>

        <h3 style="color:#2c3e50;margin:20px 0 16px 0;font-size:1.3rem;">Copy-Ready Prompts</h3>
        <p style="font-size:0.9rem;color:#7f8c8d;margin-bottom:20px;">Click the copy button next to any prompt to use it in your AI tool (Copilot, ChatGPT, Claude, etc.).</p>

        <div class="prompt-card">
          <h4>1) Email Checklist (Agent)</h4>
          <p>Creates a concise email with Yes/No items and short fill-ins.</p>
          <div class="prompt-text" data-prompt="prompt1">Create a professional email with a clean yes/no checklist using the information below. Keep it concise, agent-friendly, and ready to send. Include clear spacing, bullet points, and simple underwriting questions.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt1', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Tip: Paste your case details under the checklist in the same email.</p>
        </div>

        <div class="prompt-card">
          <h4>2) Underwriting Question Form</h4>
          <p>Turns rough notes into a simple, call-friendly form.</p>
          <div class="prompt-text" data-prompt="prompt2">Convert this information into a simple underwriting question form. Use clear bullet points, checkboxes, and short prompts. Format it so an agent can easily complete it during a call.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt2', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Use for WC, Auto, BOP, GL, Property, or specialty risks.</p>
        </div>

        <div class="prompt-card">
          <h4>3) Salesforce / CLNSS Extraction</h4>
          <p>Extracts ACORD/email/PDF details into clean text for CLNSS.</p>
          <div class="prompt-text" data-prompt="prompt3">Extract all insured, location, vehicle, driver, and coverage details from this document and return everything in a clean, Salesforce-ready text format. Use labels, line breaks, and logical field order for fast data entry.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt3', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Paste directly into your CLNSS notes or fields.</p>
        </div>

        <div class="prompt-card">
          <h4>4) Class Codes & Eligibility</h4>
          <p>Gets SIC/NAICS and GL/WC classes with quick appetite notes.</p>
          <div class="prompt-text" data-prompt="prompt4">Based on this business description, provide the correct SIC/NAICS and GL/WC class codes using publicly available info. Include eligibility concerns, typical exposures, and underwriting red flags.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt4', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Add the business description below the prompt.</p>
        </div>

        <div class="prompt-card">
          <h4>5) Coverage Summary (Client-Friendly)</h4>
          <p>Summarizes coverages, limits, endorsements, and gaps.</p>
          <div class="prompt-text" data-prompt="prompt5">Summarize all major coverages and limits from this policy in a clear, client-friendly bullet list. Include main limits, key endorsements, and any obvious coverage gaps or missing protections.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt5', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Great for quote delivery emails.</p>
        </div>

        <div class="prompt-card">
          <h4>6) Policy Comparison (Side-by-Side)</h4>
          <p>Highlights differences vs. competing carriers clearly.</p>
          <div class="prompt-text" data-prompt="prompt6">Compare these two policies side-by-side and highlight their differences in coverages, limits, endorsements, exclusions, and notable gaps. Make it easy for an agent or client to understand at a glance.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt6', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Attach both dec pages or full forms for best results.</p>
        </div>

        <div class="prompt-card">
          <h4>7) Professional Email Rewrite</h4>
          <p>Polishes tone and clarity without changing meaning.</p>
          <div class="prompt-text" data-prompt="prompt7">Rewrite this message to sound professional, friendly, and easy to understand for an agent or client. Keep it concise, improve clarity, and polish the tone without changing the meaning.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt7', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Paste your draft text under the prompt.</p>
        </div>

        <div class="prompt-card">
          <h4>8) Declination Statement (Neutral)</h4>
          <p>Compliance-safe, non-judgmental wording.</p>
          <div class="prompt-text" data-prompt="prompt8">Write a neutral, professional declination statement explaining why we cannot offer a quote. Keep the wording compliant, non-judgmental, and avoid implying wrongdoing by the insured.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt8', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Optionally include alternative markets or next steps.</p>
        </div>

        <div class="prompt-card">
          <h4>9) Data Extraction (ACORDs/Emails/PDFs)</h4>
          <p>Pulls all usable info into a single, easy-copy block.</p>
          <div class="prompt-text" data-prompt="prompt9">Extract all available insured, coverage, property, vehicle, and driver information from this file. Return it in a clean, easy-to-copy text block organized by category.</div>
          <button class="copy-btn" onclick="copyPrompt('prompt9', this)">📋 Copy Prompt</button>
          <p class="prompt-tip">Great when submissions arrive as mixed emails + attachments.</p>
        </div>

        <div style="background:#f8f9fa;border:1px solid #e0e0e0;padding:14px;border-radius:10px;margin-top:20px;">
          <p style="margin:0;font-size:0.85rem;color:#7f8c8d;">Note: These prompts work with any AI assistant (Copilot, ChatGPT, Claude, etc.). Simply copy the prompt text and paste it into your conversation, then add your specific details below.</p>
        </div>
      `;
      openModal('🤖', 'AI Tips & Prompts', 'AGENT TRAINING', content);
    }

    function copyPrompt(promptId, button) {
      const promptElement = document.querySelector(`[data-prompt="${promptId}"]`);
      if (!promptElement) return;
      const text = promptElement.textContent.trim();
      // fallback function to copy via a temporary textarea
      const doCopy = () => {
        const textarea = document.createElement('textarea');
        textarea.value = text;
        // Avoid scrolling to bottom on iOS
        textarea.style.position = 'fixed';
        textarea.style.top = '-9999px';
        document.body.appendChild(textarea);
        textarea.focus();
        textarea.select();
        try {
          document.execCommand('copy');
        } catch (err) {
          console.error('Fallback copy failed:', err);
        }
        document.body.removeChild(textarea);
      };
      // Use Clipboard API when available and permitted
      if (navigator.clipboard && navigator.clipboard.writeText) {
        navigator.clipboard.writeText(text).catch(() => {
          doCopy();
        });
      } else {
        doCopy();
      }
      // Provide user feedback on the button
      const originalText = button.innerHTML;
      button.innerHTML = '✓ Copied!';
      button.style.background = '#10b981';
      setTimeout(() => {
        button.innerHTML = originalText;
        button.style.background = '';
      }, 2000);
    }

    function openQuickRefModal() {
      const content = `
        <h3>Quick Reference Guide – Inside Sales Partnerships</h3>
        <p>Essential information for daily operations – partnership agency codes, binding procedures, and renewal handling.</p>

        <!-- Smart Choice pre‑renewal call‑out -->
        <h4>🔥 Smart Choice Pre‑Renewal Process</h4>
        <p>As our #1 partner, Smart Choice requires proactive pre‑renewal handling. Use the following ready-to-copy values when setting the Pre‑Renewal Direction (PRD) in PolicyCenter:</p>
        <div style="background:#f7f8fa;border:1px solid #e0e0e0;padding:12px;border-radius:8px;margin-bottom:12px;font-size:0.9rem;">
          <p style="margin:4px 0;"><strong>Direction:</strong> <span data-prompt="sc-direction">&ldquo;Refer to Customer Service Representative&rdquo;</span> <button class="copy-btn" onclick="copyPrompt('sc-direction', this)" style="margin-left:8px;font-size:0.8rem;">📋 Copy</button></p>
          <p style="margin:4px 0;"><strong>Subject:</strong> <span data-prompt="sc-subject">"Refer to CSR"</span> <button class="copy-btn" onclick="copyPrompt('sc-subject', this)" style="margin-left:8px;font-size:0.8rem;">📋 Copy</button></p>
          <p style="margin:4px 0;"><strong>Text (Copy/Paste):</strong> <span data-prompt="sc-text">At renewal update agency code to 68159 please keep producer the same. This is part of transfer between agency codes that has been vetted by NSS with proper documentation. Please allow 68159 to service the policy prior to the agency code update at the upcoming renewal. POST BIND CONTACT: Contact CLInside@nationwide.com regarding any post-bind 1st term underwriting concerns prior to contacting primary listed agent due to this being sell-on-behalf business from the NSS CL Inside Sales team.</span> <button class="copy-btn" onclick="copyPrompt('sc-text', this)" style="margin-left:8px;font-size:0.8rem;">📋 Copy</button></p>
        </div>
        <p><strong>NB &amp; Renewal Codes:</strong> NB code 61650, Renewal code 68159</p>

        <!-- Full Smart Choice process inserted verbatim from reference text -->
        <div id="sc-full-section">
        <h4>📘 Smart Choice Full Handling Process</h4>
        <p>The following section details the complete Smart Choice Inside Sales process, including agent and customer contact, quoting, binding, pre‑renewal direction, follow‑up, and email templates. Please follow these steps verbatim:</p>
        <pre style="white-space: pre-wrap; background: #f7f8fa; border: 1px solid #e0e0e0; padding: 12px; border-radius: 8px; font-size: 12px; line-height: 1.5;">
Smart Choice - Agent Contact
1) Obtain new lead via email - Identify if agent requests direct contact
If agent requests customer contact, proceed to Smart Choice Customer Contact section

Email for Smart Choice should come into the CLSmart@nationwide.com address only&#x27;

2) Review submission to determine eligibility
Give benefit of doubt if unsure if eligible, always lean to gather information or call agent unless certain the risk is ineligible.

3) Gather information and prepare quote
Make outbound calls to agents as primary mode of contact to obtain basic information needed to quote the risk.

Questions emails may be sent if we receive no answer to these calls.

Full underwriting questions can be sent via email along with an Indication, suggested not to try to ask all on phone unless agent requests to do so.

4) Quote the risk
Agency Codes - Use the correct agency codes &amp; producer for the partnership (see table above)

(Smart Choice New Business: 61650 &amp; Producer: Ashley Wingate)

Workers Compensation

Owner Inclusion/Exclusion rules must be reviewed and documented at quote to ensure compliance including required forms are obtained prior to or shortly after bind.

5) Present Quote
Quotes should be presented to the customer by the agent if we are working with the agent directly.

Send the Approved Quote email template with proposal attached

Include notation of any pre-bind or trailing documents such as WC forms

Read all required statements prior to presenting a rate by phone:

Conditional Quote: “All quotes are calculated based upon our current rates, and the information that you provide during the application process, supplemented by publicly available data. Any information provided or discovered at a later date could affect your rate and/or eligibility.”

6) Bind Request
Agents should reply to our Approved Quote email answering all of our bind questions.

Agents may also call in and provide the answers to our bind questions if desired. Interaction should be clearly documented.

If agent requests to provide payment information for customer and did not email in a bind request, ask if they reviewed payment instructions in email.

Proceed to bind coverage once all bind questions have been answered.

7) Bind Coverage
Make any final updates or corrections to the policy including:

Updating Effective and Expiration Dates

Updating Mailing/Billing Address

Proceed to Issue the policy based on the payment options selected by the agent

If taking payment information from the agent, ask them to read you the EFT account numbers to enter in the system, or to type the Credit Card number into the phone with Semafone.

Payment information must be entered into the system as you bind. Do not write down or save any payment information.

If REFT is established, the REFT form must be sent to the customer via Docusign immediately post bind. This form can be found on the post-bind screen in Policy Center.

Send to CLAmendment@nationwide.com when signature is obtained.

Once issued, download Application and Dec pages to be attached

Send a reply email to the agent with the Bind template completed

Send a separate Bind email template to the Customer if elected by agent (ensure it is sent FROM CLSmart@nationwide.com for this partnership)

8) Pre-Renewal Direction
A PRD must be set for each new account bound from the Account Summary Screen in Policy Center

Choose Actions, then Pre-Renewal Direction, and fill in as follows:

Direction: “Refer to Customer Service Representative”

Subject: &quot;Refer to CSR&quot;

Text (Copy/Paste): At renewal update agency code to 57850 please keep producer the same. This is part of transfer between agency codes that has been vetted by NSS with proper documentation. Please allow 57850 to service the policy prior to the agency code update at the upcoming renewal. POST BIND CONTACT: Contact CLInside@nationwide.com regarding any post‑bind 1st term underwriting concerns prior to contacting primary listed agent due to this being sell‑on‑behalf business from the NSS CL Inside Sales team.

AOR/BOR Requests

We can accept an AOR for Quotes

Refer agents to their Smart Choice rep if we receive an AOR for an active account.

Middle Market

Review with leader to determine if we may be able to get a SM exception.

These may be referred to the Smart Choice contact for middle market using the middle market email template.

Reply Emails

Ensure reply emails continue to contain our email templates to allow for clarity in next steps.

(Example: You send an Indication Present, agent replies with a question, you should re-send the Indication Present email (with the unanswered questions) and put your reply to their question at the top. 

Follow Ups

Follow up calls and emails should be made consistently on outstanding accounts.

Pre-Quote - Make additional follow up call after initial call attempt (at least 1 suggested at this stage)

Quote - Make 1 follow up call within 24 hours of sending a proposal to allow for objections to be overcome. 3 total follow ups over time should be made. (suggest no more than 1 week in between unless accurate effective date necessitates future calls)

Email Templates

More Information Needed - Agent does not answer, need a lot more information to consider the risk

Quote Questions - Agent does not answer, send limited number of basic questions to help with eligibility and to prepare an indication

Indication Present - To send an indication (prior to verifying all application questions) and must include all outstanding questions in the email body.

Approved Quote - Only to be sent if there are no outstanding questions, application is fully approved and ready to bind.

Decline - Risk is ineligible, provide accurate description of ineligibility. Include any online references if these lead to the decline.

 


Smart Choice - Customer Contact
1) Obtain new lead via email
If agent requests direct contact, proceed to Smart Choice Agent Contact section

Email for Smart Choice should come into the CLSmart@nationwide.com address only

2) Review submission to determine eligibility
Give benefit of doubt if unsure if eligible, always lean to gather information or call agent unless certain the risk is ineligible.

If found to be ineligible right away, proceed to 6. Ineligible Risks

3) Outbound Call
Answer: “Hi, this is &lt;name&gt; from Nationwide Insurance calling on behalf of &lt;Sub‑Agency Name&gt; regarding a requested insurance quote. Do you have a few minutes to discuss?”
No Answer: “This is &lt;name&gt; from Nationwide Insurance calling on behalf of &lt;Sub‑Agency Name&gt; regarding your request for a quote. We need additional information to complete your quote. Please give me a call back at &lt;agent direct number&gt; or reply to my email when you have a moment to speak”

Sent no answer email template

CRITICAL: Use the name of the Sub‑Agency, NOT “Smart Choice”. The customers will not know who “Smart Choice” is.

TCPA Statement: “Though your consent to receive a call is not required to make a purchase, Nationwide and its Agents may use automated technology to contact you for sales purposes. You may revoke consent at any time. Do you agree to receive such calls at the phone number you provided?”

4) Gather information and prepare quote
If call is answered, set up the account and be prepared to quote the account while on the phone with the customer.

Full underwriting questions should be asked on the phone while quoting.

If unable to quote by phone due to complexity, set an appointment to contact the customer back to present later that day.

5) Quote the risk
Agency Codes - Use the correct agency codes &amp; producer for the partnership (see table above)

(Smart Choice New Business: 61650 &amp; Producer: Ashley Wingate)

Workers Compensation

Owner Inclusion/Exclusion rules must be reviewed and documented at quote to ensure compliance including required forms are obtained prior to or shortly after bind.

6) Ineligible Risks
Pre-Customer Call: If risk can be determined ineligible prior to calling customer, email agent the Decline email template with reason.

Post-Customer Call: If risk is ineligible for coverage with Nationwide, advise the customer by phone and advise that their agent (&quot;Sub‑Agent/Agency Name&quot;) may have other options and you will make them aware.

Send agent the Decline email template and advise if you contacted the customer.

7) Present Quote
Quotes should be presented to the customer fully when working directly with the customer.

Present all base coverages including limits, deductibles, and a coverage example. For endorsements, at least one coverage must also be presented and explained. 

Ask customers if they have any additional questions on coverages or limits.

Read all required statements prior to presenting a rate:

Conditional Quote: “All quotes are calculated based upon our current rates, and the information that you provide during the application process, supplemented by publicly available data. Any information provided or discovered at a later date could affect your rate and/or eligibility.”

Present the rate to the customer and explain our payment options (Including monthly payment, REFT, etc.)

Ask for the sale &amp; Handle objections

If not sold, request to set a date to follow up with the customer

8) Bind
Required: Read the Required Pre‑Bind Statements (See other section below - click here) and then return here to proceed. 

Make any final updates or corrections to the policy including:

Updating Effective and Expiration Dates

Updating Mailing/Billing Address

Read the Required Payment Statements (See other section below) and then return here to proceed.

Proceed to Issue the policy based on the payment options selected

Once issued, download Application and Dec pages to be attached

Send the Application DocuSign via PolicyCenter

Advise customer of the NW Service Center and contact information for certificates or future needs.

Customer may contact us directly if additional lines of business are needed in the future.

Email

Send an email to the agent with the Bind template completed

Send a separate Bind email template to the Customer

CRITICAL (ensure email is sent FROM CLSmart@nationwide.com for this partnership)

9) Pre‑Renewal Direction
A PRD must be set for each new account bound from the Account Summary Screen in Policy Center

Choose Actions, then Pre‑Renewal Direction, and fill in as follows:

Direction: “Refer to Customer Service Representative”

Subject: &quot;Refer to CSR&quot;

Text (Copy/Paste): At renewal update agency code to 57850 please keep producer the same. This is part of transfer between agency codes that has been vetted by NSS with proper documentation. Please allow 57850 to service the policy prior to the agency code update at the upcoming renewal. POST BIND CONTACT: Contact CLInside@nationwide.com regarding any post‑bind 1st term underwriting concerns prior to contacting primary listed agent due to this being sell‑on‑behalf business from the NSS CL Inside Sales team.

AOR/BOR Requests

We can accept an AOR for Quotes

Middle Market

Review with leader to determine if we may be able to get a SM exception.

These may be referred to the Smart Choice contact for middle market using the middle market email template.

Follow Ups

Follow up calls and emails should be made consistently on outstanding accounts.

Pre‑Quote - Make additional follow up call after initial call attempt (at least 1 suggested at this stage)

Quote - 3 total follow ups over time should be made based upon customer reaction and timeline. (suggest no more than 1 week in between unless accurate effective date necessitates future calls)

Email Templates

SC Customer No Answer - Initial call attempt unsuccessful, email to ask them to call you back.

SC Customer Quote Presentation - Proposal attached and contact information to call back to bind.


        </pre>
        </div>

        <h4>📋 Agency Codes</h4>
        <p><strong>Format:</strong> 5-digit numeric (e.g., 61650, 68159)</p>
        
        <h4>By Partnership (NB/Renewal)</h4>
        <ul>
          <li><strong>Smart Choice:</strong> NB: 61650 | Renewal: 68159 | Producer: Ashley Wingate</li>
          <li><strong>KMA Insurance Group:</strong> NB: 62549 | Renewal: 68159</li>
          <li><strong>Insureon:</strong> NB: 62719 | Renewal: 62788</li>
          <li><strong>IOA:</strong> NB: 67667</li>
          <li><strong>NSS All States (Except CA):</strong> 75095</li>
          <li><strong>NSS California Only:</strong> 75104</li>
          <li><strong>USI:</strong> NB: 66783 | Renewal: 63850</li>
        </ul>

        <h4>✅ Binding Instructions</h4>
        <ol>
          <li><strong>Complete Quote:</strong> PolicyCenter/carrier system, all UW questions answered</li>
          <li><strong>Read Pre-Bind Statements:</strong> Privacy (All States/CA/VT) + Fraud statement</li>
          <li><strong>Confirm Details:</strong> Effective date, mailing/billing address, correct agency code</li>
          <li><strong>Payment:</strong> Enter directly (CC via Semafone, EFT with authorization script)</li>
          <li><strong>Issue Policy:</strong> Bind in PolicyCenter, download App & Dec pages</li>
          <li><strong>Post-Bind:</strong> Send DocuSign if needed (WC, REFT), use bind email templates</li>
        </ol>

        <h4>📧 Bind Email Addresses</h4>
        <ul>
          <li><strong>Smart Choice:</strong> CLSmart@nationwide.com</li>
          <li><strong>KMA & Others:</strong> CLInside@nationwide.com</li>
        </ul>

        <h4>🔄 Renewal (PRD) Instructions</h4>
        <p><strong>At NB Bind - Set PRD in PolicyCenter:</strong></p>
        <ul>
          <li>Actions → Pre-Renewal Direction</li>
          <li>Direction: &ldquo;Refer to Customer Service Representative&rdquo;</li>
          <li>Subject: "Refer to CSR"</li>
        </ul>
        <p><strong>PRD Text (Smart Choice):</strong> Update agency code to 68159, keep producer same, allow 68159 to service prior to code update</p>
        <p><strong>PRD Text (KMA):</strong> Update agency code to 68159, keep producer same, allow 68159 to service prior to code update</p>

        <h4>📞 Key Partnership Contacts</h4>
        <ul>
          <li><strong>Smart Choice Agents:</strong> 1-800-896-2277</li>
          <li><strong>Smart Choice Customers:</strong> 1-888-282-3717</li>
          <li><strong>KMA:</strong> 1-800-730-8413 | Ineligible: 423-375-2370 (Jared Allen)</li>
          <li><strong>Insureon:</strong> 1-877-588-2392</li>
          <li><strong>IOA:</strong> 1-877-588-2380</li>
        </ul>

        <h4>🔗 UW & Service</h4>
        <ul>
          <li><strong>P&C UW (All Partnerships):</strong> NSS Queue Underwriters</li>
          <li><strong>Bonds (Smart Choice):</strong> Trevor Sharp - SHARPT4@nationwide.com | 515-508-6432</li>
          <li><strong>1st-Term UW Concerns:</strong> CLInside@nationwide.com (before contacting agent)</li>
          <li><strong>UW New Business:</strong> AskCLNewBusiness@nationwide.com</li>
          <li><strong>UW Existing Business:</strong> AskCLExistingBusiness@nationwide.com</li>
        </ul>

        <!-- Placeholder for Smart Choice section to be moved to end -->
        <div id="sc-placeholder"></div>
        <p><em>F8or complete procedures, refer to the <strong>Handling Procedures</strong> site in Inside Sales Resources.</em></p>
      `;
      openModal('📖', 'Quick Reference Guide', 'PARTNERSHIPS', content);
      // After opening the modal, move the Smart Choice full section to the placeholder at the bottom
      setTimeout(() => {
        const scSection = document.getElementById('sc-full-section');
        const placeholder = document.getElementById('sc-placeholder');
        if (scSection && placeholder) {
          placeholder.appendChild(scSection);
        }
      }, 0);
    }
    
    function copyRefText(dataId, button) {
      const element = document.querySelector(`[data-copy="${dataId}"]`);
      if (!element) return;
      const text = element.textContent.trim();
      const doCopy = () => {
        const textarea = document.createElement('textarea');
        textarea.value = text;
        textarea.style.position = 'fixed';
        textarea.style.top = '-9999px';
        document.body.appendChild(textarea);
        textarea.focus();
        textarea.select();
        try {
          document.execCommand('copy');
        } catch (err) {
          console.error('Fallback copy failed:', err);
        }

    // Attach a global click handler to ensure copy buttons work even when inline onclick attributes are stripped
    document.addEventListener('click', function(event) {
      const target = event.target;
      // Handle AI prompt copy buttons
      if (target && target.classList && target.classList.contains('copy-btn')) {
        // Find the prompt text associated with this button
        const parent = target.closest('.prompt-card');
        if (parent) {
          const promptElement = parent.querySelector('.prompt-text');
          if (promptElement) {
            const promptId = promptElement.getAttribute('data-prompt');
            if (promptId) {
              copyPrompt(promptId, target);
            }
          }
        }
      }
    });
        document.body.removeChild(textarea);
      };
      if (navigator.clipboard && navigator.clipboard.writeText) {
        navigator.clipboard.writeText

<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>টাকা আয় করুন - বিজ্ঞাপন দেখুন</title>
    <script src='//libtl.com/sdk.js' data-zone='9472189' data-sdk='show_9472189'></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --primary-color: #4a6bff;
            --secondary-color: #ff7d4a;
            --success-color: #28a745;
            --danger-color: #dc3545;
            --warning-color: #ffc107;
            --dark-color: #1a1a2e;
            --light-color: #f8f9fa;
            --card-bg: #16213e;
            --text-color: #e6e6e6;
            --text-muted: #adb5bd;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            color: var(--text-color);
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            padding: 15px;
            padding-bottom: 70px;
        }
        
        .container {
            max-width: 500px;
            width: 100%;
            margin: 0 auto;
            background: rgba(22, 33, 62, 0.9);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            overflow: hidden;
            padding-bottom: 20px;
            backdrop-filter: blur(10px);
        }
        
        .header {
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 20px;
            text-align: center;
            position: relative;
            border-bottom: 5px solid rgba(255, 255, 255, 0.1);
        }
        
        .header h1 {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 5px;
        }
        
        .badge {
            display: inline-block;
            background-color: rgba(255, 255, 255, 0.2);
            padding: 5px 12px;
            border-radius: 50px;
            font-size: 12px;
            font-weight: 600;
            margin-top: 10px;
        }
        
        .user-card, .stat-card, .progress-container, .referral-section, .rate-info, .withdraw-section, .ad-status {
            background-color: var(--card-bg);
            margin: 15px;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }
        
        .user-card {
            display: flex;
            align-items: center;
        }
        
        .user-avatar {
            width: 50px;
            height: 50px;
            background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 20px;
            color: white;
            margin-right: 15px;
        }
        
        .stats-container {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
        }
        
        .stat-card {
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
        }
        
        .stat-card h3 {
            font-size: 12px;
            color: var(--text-muted);
            margin-bottom: 10px;
        }
        
        .stat-card p {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary-color);
        }
        
        .progress-container {
            background: linear-gradient(to right, #0f0c29, #302b63);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .progress-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
        }
        
        .progress-bar {
            height: 10px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
            overflow: hidden;
            margin-bottom: 10px;
        }
        
        .progress-fill {
            height: 100%;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            border-radius: 5px;
            width: 0%;
            transition: width 0.5s ease;
        }
        
        .progress-text {
            display: flex;
            justify-content: space-between;
            font-size: 12px;
            color: var(--text-muted);
        }
        
        .action-buttons {
            display: grid;
            grid-template-columns: 1fr;
            gap: 10px;
            margin: 15px;
        }
        
        .btn {
            padding: 15px;
            border: none;
            border-radius: 10px;
            font-weight: 600;
            font-size: 16px;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
        }
        
        .btn-primary { background: linear-gradient(to right, var(--primary-color), #6a11cb); color: white; }
        .btn-success { background: linear-gradient(to right, var(--success-color), #11998e); color: white; }
        .btn-danger { background: linear-gradient(to right, var(--danger-color), #ff416c); color: white; }
        .btn-warning { background: linear-gradient(to right, var(--warning-color), #ff7e5f); color: white; }
        .btn-secondary { background: linear-gradient(to right, #2c3e50, #4ca1af); color: var(--text-color); border: 1px solid rgba(255, 255, 255, 0.1); }
        
        .btn:hover { transform: translateY(-3px); box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3); }
        .btn:active { transform: translateY(0); }
        .btn:disabled { opacity: 0.6; cursor: not-allowed; transform: none; box-shadow: none; }
        .btn i { margin-right: 8px; font-size: 18px; }
        
        .section-title {
            font-size: 18px;
            margin-bottom: 15px;
            color: white;
            display: flex;
            align-items: center;
        }
        
        .section-title i { margin-right: 10px; color: var(--secondary-color); }
        
        .referral-stats {
            display: flex;
            justify-content: space-between;
            background-color: rgba(0, 0, 0, 0.2);
            padding: 10px 15px;
            border-radius: 8px;
            margin-bottom: 15px;
        }
        
        .referral-link-container { display: flex; margin-top: 15px; }
        
        #referral-link {
            flex: 1;
            padding: 12px;
            background-color: rgba(0, 0, 0, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 8px 0 0 8px;
            color: var(--text-color);
            font-size: 14px;
            outline: none;
        }
        
        #copy-referral {
            padding: 0 15px;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            border: none;
            border-radius: 0 8px 8px 0;
            color: white;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .withdraw-section { display: none; }
        .form-group { margin-bottom: 15px; }
        .form-group label { display: block; margin-bottom: 8px; font-size: 14px; color: var(--text-muted); }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            background-color: rgba(0, 0, 0, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 8px;
            color: var(--text-color);
            font-size: 14px;
            outline: none;
        }
        
        #withdraw-status { margin-top: 15px; font-size: 14px; text-align: center; padding: 10px; border-radius: 8px; }
        .success-message { background-color: rgba(40, 167, 69, 0.2); color: var(--success-color); }
        .error-message { background-color: rgba(220, 53, 69, 0.2); color: var(--danger-color); }
        
        .footer { text-align: center; margin-top: 20px; font-size: 12px; color: var(--text-muted); }
        
        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 15px;
            border-radius: 8px;
            background: var(--card-bg);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            z-index: 1000;
            display: flex;
            align-items: center;
            transform: translateX(150%);
            transition: transform 0.5s ease;
        }
        .notification.show { transform: translateX(0); }
        .notification.success { border-left: 4px solid var(--success-color); }
        .notification.error { border-left: 4px solid var(--danger-color); }
        
        .bottom-nav {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: var(--card-bg);
            display: flex;
            justify-content: space-around;
            padding: 10px 0;
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.2);
            z-index: 1000;
        }
        
        .nav-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            color: var(--text-muted);
            text-decoration: none;
            font-size: 12px;
            padding: 5px 10px;
            border-radius: 10px;
            width: 20%;
        }
        
        .nav-item.active { color: var(--primary-color); background: rgba(74, 107, 255, 0.2); }
        .nav-item i { font-size: 20px; margin-bottom: 5px; }
        
        .page-section { display: none; }
        .page-section.active { display: block; }
        
        .ad-container {
            margin: 15px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 90px;
            background-color: rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            overflow: hidden;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>টাকা আয় করুন - বিজ্ঞাপন দেখুন</h1>
            <p>বিজ্ঞাপন দেখে আসল টাকা আয় করুন</p>
            <div class="badge">সক্রিয়</div>
        </div>
        
        <div class="ad-container">
            <center>
                <script type="text/javascript">
                    atOptions = { 'key' : 'af3ac5da264d48edf05886e0c3d572c2', 'format' : 'iframe', 'height' : 50, 'width' : 320, 'params' : {} };
                </script>
                <script type="text/javascript" src="//www.highperformanceformat.com/af3ac5da264d48edf05886e0c3d572c2/invoke.js"></script>
            </center>
        </div>
        
        <!-- হোম পেজ -->
        <div class="page-section active" id="home-page">
            <div class="user-card">
                <div class="user-avatar" id="user-avatar">U</div>
                <div class="user-info">
                    <h3 id="user-name">ব্যবহারকারী</h3>
                    <p>আইডি: <span id="user-id">12345</span></p>
                </div>
            </div>
            
            <div class="stats-container">
                <div class="stat-card"><h3>দেখা বিজ্ঞাপন</h3><p id="watched-ads">0</p></div>
                <div class="stat-card"><h3>আয়কৃত টাকা</h3><p id="earned-money">0.00 <small>টাকা</small></p></div>
            </div>
            
            <div class="progress-container">
                <div class="progress-header"><h3>আজকের অগ্রগতি</h3><span id="ads-progress">0/20</span></div>
                <div class="progress-bar"><div class="progress-fill" id="progress-fill"></div></div>
            </div>
            
            <div class="ad-status" id="ad-status"><i class="fas fa-check-circle"></i> বিজ্ঞাপন দেখতে প্রস্তুত</div>
            
            <div class="action-buttons">
                <button class="btn btn-primary" id="watch-ad-btn" onclick="watchAd()"><i class="fas fa-play"></i> বিজ্ঞাপন দেখুন (২ টাকা)</button>
                <button class="btn btn-success" id="auto-ad-btn" onclick="startAutoAds()"><i class="fas fa-robot"></i> স্বয়ংক্রিয় বিজ্ঞাপন</button>
                <button class="btn btn-danger" id="stop-auto-btn" onclick="stopAutoAds()" disabled><i class="fas fa-stop"></i> বন্ধ করুন</button>
                <button class="btn btn-secondary" onclick="showWithdrawForm()"><i class="fas fa-wallet"></i> টাকা উত্তোলন</button>
            </div>
        </div>
        
        <!-- একাউন্ট অ্যাক্টিভ পেজ -->
        <div class="page-section" id="active-page">
            <h3 class="section-title"><i class="fas fa-user-shield"></i> Account Active</h3>
            <div class="stat-card" style="text-align: center; padding: 20px;">
                <i class="fas fa-exclamation-circle" style="font-size: 40px; color: var(--warning-color); margin-bottom: 15px;"></i>
                <h3 style="font-size: 18px; color: white; margin-bottom: 10px;">আপনার অ্যাকাউন্টটি অ্যাক্টিভ করুন</h3>
                <p style="font-size: 15px; margin-bottom: 20px; color: var(--text-muted); line-height: 1.5;">
                    কন্টাক্ট <b style="color: var(--secondary-color);">@fxtrader3642</b> মেসেজ দেন একাউন্ট এক্টিভেট করতে।
                </p>
                <a href="https://t.me/fxtrader3642" target="_blank" class="btn btn-success" style="justify-content: center;">
                    <i class="fab fa-telegram-plane"></i> কন্টাক্ট করুন (@fxtrader3642)
                </a>
            </div>
        </div>

        <!-- আর্ন পেজ -->
        <div class="page-section" id="earn-page">
            <h3 class="section-title"><i class="fas fa-coins"></i> টাকা আয় করার উপায়</h3>
            <div class="action-buttons">
                <button class="btn btn-primary" onclick="watchAd()"><i class="fas fa-play"></i> বিজ্ঞাপন দেখুন (২ টাকা)</button>
            </div>
        </div>
        
        <!-- উত্তোলন পেজ -->
        <div class="page-section" id="withdraw-page">
            <h3 class="section-title"><i class="fas fa-wallet"></i> টাকা উত্তোলন</h3>
            <div class="stat-card"><h3>মোট আয়</h3><p id="total-earned-withdraw">0.00 <small>টাকা</small></p></div>
            <div class="withdraw-section" id="withdraw-section" style="display:block;">
                <div class="form-group"><label>পরিমাণ (টাকা)</label><input type="number" id="withdraw-amount" class="form-control" placeholder="টাকার পরিমাণ"></div>
                <div class="form-group"><label>পেমেন্ট মাধ্যম</label><select id="payment-method" class="form-control"><option value="bkash">bKash</option><option value="nagad">Nagad</option></select></div>
                <div class="form-group"><label>মোবাইল নম্বর</label><input type="text" id="withdraw-phone" class="form-control" placeholder="01XXXXXXXXX"></div>
                <button class="btn btn-primary" onclick="withdrawPoints()">অনুরোধ পাঠান</button>
                <div id="withdraw-status"></div>
            </div>
        </div>
        
        <!-- নোটিশ পেজ -->
        <div class="page-section" id="notice-page">
            <h3 class="section-title"><i class="fas fa-bell"></i> নোটিশ</h3>
            <div class="stat-card"><p>সবার অ্যাকাউন্ট অ্যাক্টিভ করতে হবে। কন্টাক্ট @fxtrader3642 মেসেজ দেন একাউন্ট এক্টিভেট করতে।</p></div>
        </div>
        
        <div class="footer"><p>© ২০২৬ টাকা আয় করুন অ্যাপ।</p></div>
    </div>

    <!-- নেভিগেশন বার -->
    <div class="bottom-nav">
        <a href="#" class="nav-item active" onclick="showPage('home-page', this)"><i class="fas fa-home"></i><span>হোম</span></a>
        <a href="#" class="nav-item" onclick="showPage('active-page', this)"><i class="fas fa-user-check"></i><span>Account Active</span></a>
        <a href="#" class="nav-item" onclick="showPage('earn-page', this)"><i class="fas fa-coins"></i><span>আর্ন</span></a>
        <a href="#" class="nav-item" onclick="showPage('withdraw-page', this)"><i class="fas fa-wallet"></i><span>উত্তোলন</span></a>
        <a href="#" class="nav-item" onclick="showPage('notice-page', this)"><i class="fas fa-bell"></i><span>নোটিশ</span></a>
    </div>

    <div id="notification" class="notification"><i class="fas fa-check-circle"></i><span id="notification-text"></span></div>

    <script>
        let watchedAdsCount = 0;
        let earnedPoints = 0.00;
        let userId = "12345";
        let isAutoMode = false;
        let isAdLoading = false;

        function showPage(pageId, element) {
            document.querySelectorAll('.page-section').forEach(p => p.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');
            document.querySelectorAll('.nav-item').forEach(i => i.classList.remove('active'));
            element.classList.add('active');
        }

        function watchAd() {
            if (isAdLoading) return;
            if (typeof window.show_9472189 !== 'function') {
                alert('বিজ্ঞাপন লোড হচ্ছে, একটু অপেক্ষা করুন!');
                return;
            }
            isAdLoading = true;
            window.show_9472189().then(() => {
                watchedAdsCount++;
                earnedPoints += 2.00;
                document.getElementById('watched-ads').textContent = watchedAdsCount;
                document.getElementById('earned-money').textContent = earnedPoints.toFixed(2);
                isAdLoading = false;
            }).catch(err => {
                isAdLoading = false;
            });
        }
        
        function withdrawPoints() {
            alert('টাকা উত্তোলনের আগে অ্যাকাউন্ট অ্যাক্টিভ করুন। কন্টাক্ট @fxtrader3642 মেসেজ দেন একাউন্ট এক্টিভেট করতে।');
        }
    </script>
</body>
</html>
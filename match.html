<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>تاكسي نواكشوط</title>
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link rel="manifest" href="/manifest.json">
  <meta name="theme-color" content="#075e54">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', Tahoma, sans-serif;
      overflow: hidden;
      height: 100vh;
      touch-action: pan-y;
      background: #f5f5f5;
      opacity: 0;
      transition: opacity 0.3s ease-in;
    }

    .header {
      background: linear-gradient(90deg, #075e54, #128C7E);
      color: white;
      padding: 15px 20px;
      text-align: center;
      font-weight: bold;
      font-size: 20px;
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .menu-toggle {
      background: none; border: none; color: white; font-size: 24px; cursor: pointer;
    }

    .sidebar {
      position: fixed;
      top: 60px;
      right: -300px;
      width: 300px;
      height: calc(100% - 60px);
      background: white;
      box-shadow: -4px 0 15px rgba(0,0,0,0.1);
      z-index: 2000;
      transition: right 0.4s ease;
      padding: 20px;
      overflow-y: auto;
    }
    .sidebar.open { right: 0; }
    .sidebar h3 { color: #075e54; margin-bottom: 20px; }
    .form-group {
      margin-bottom: 15px;
    }
    .form-group label {
      display: block;
      margin-bottom: 5px;
      font-weight: bold;
      color: #333;
    }
    .form-group input {
      width: 100%;
      padding: 10px;
      border: 1px solid #ddd;
      border-radius: 8px;
      font-size: 16px;
      transition: all 0.3s ease;
    }
    .form-group input:focus {
      border-color: #128C7E;
      box-shadow: 0 0 0 2px rgba(18, 140, 126, 0.2);
      outline: none;
    }
    .btn {
      background: #075e54;
      color: white;
      border: none;
      border-radius: 30px;
      padding: 12px 20px;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      width: 100%;
      margin-top: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      transition: all 0.3s ease;
    }
    .btn:hover { background: #054a43; transform: translateY(-2px); }
    .btn-outline {
      background: transparent;
      border: 2px solid #075e54;
      color: #075e54;
    }
    .btn:disabled {
      opacity: 0.6;
      cursor: not-allowed;
      transform: none !important;
    }

    .register-type {
      display: flex;
      gap: 10px;
      margin: 15px 0;
    }
    .register-type button {
      flex: 1;
      padding: 12px;
      font-weight: bold;
      border-radius: 12px;
    }

    .section { margin-top: 30px; }
    .section-title {
      font-size: 18px;
      font-weight: bold;
      color: #075e54;
      margin-bottom: 10px;
      padding-bottom: 5px;
      border-bottom: 2px solid #e0e0e0;
    }
    .driver-list { list-style: none; }
    .driver-item {
      display: flex !important;
      justify-content: space-between !important;
      align-items: center !important;
      padding: 12px 15px !important;
      background: #f9f9f9;
      border-radius: 8px;
      margin-bottom: 8px;
      cursor: pointer;
      transition: all 0.2s;
    }
    .driver-item:hover {
      background: #f0f0f0;
      transform: translateX(4px);
    }
    .driver-item.inactive { opacity: 0.6; }
    .driver-item strong { color: #075e54; }

    .unread-badge {
      background: #ff4444;
      color: white;
      border-radius: 50%;
      width: 22px;
      height: 22px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 12px;
      font-weight: bold;
    }
    .driver-item i {
      font-size: 18px;
      cursor: pointer;
      padding: 6px;
      border-radius: 50%;
      transition: background 0.2s;
    }
    .driver-item i:hover {
      background: rgba(0,0,0,0.05);
    }

    .map-container {
      position: fixed;
      top: 60px;
      left: 0;
      right: 0;
      bottom: 0;
      z-index: 5;
    }
    #map { width: 100%; height: 100%; }

    #permissionScreen {
      position: fixed;
      top: 60px; left: 0; right: 0; bottom: 0;
      background: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 20px;
      z-index: 100;
    }
    #permissionScreen h2 { color: #075e54; margin: 15px 0; font-size: 24px; }
    #permissionScreen p { color: #444; line-height: 1.7; margin: 15px 0; max-width: 380px; }
    .requirement {
      background: #e8f5e9;
      border-right: 4px solid #4caf50;
      padding: 12px;
      margin: 12px 0;
      border-radius: 0 8px 8px 0;
      text-align: right;
    }
    #allowBtn {
      background: #075e54;
      color: white;
      border: none;
      border-radius: 30px;
      padding: 14px 36px;
      font-size: 18px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 4px 12px rgba(7, 94, 84, 0.4);
      display: flex;
      align-items: center;
      gap: 10px;
      margin-top: 10px;
      transition: all 0.3s ease;
    }
    #allowBtn:hover:not(:disabled) { background: #054a43; transform: translateY(-2px); }
    #allowBtn:disabled { opacity: 0.7; transform: none !important; }

    .control-btns {
      position: fixed;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);
      z-index: 100;
      display: none;
    }

    .driver-info-card {
      position: fixed;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);
      background: white;
      border-radius: 16px;
      padding: 20px;
      width: 90%;
      max-width: 400px;
      box-shadow: 0 -4px 30px rgba(0,0,0,0.25);
      z-index: 999;
      display: none;
      animation: slideUp 0.4s ease;
    }

    @keyframes slideUp {
      from { bottom: -200px; opacity: 0; }
      to { bottom: 20px; opacity: 1; }
    }

    .driver-info-card h4 {
      color: #075e54;
      margin: 0 0 15px;
      text-align: center;
    }

    .driver-info-card p {
      margin: 8px 0;
      color: #555;
    }

    .driver-info-card .btn-group {
      display: flex;
      gap: 10px;
      margin-top: 20px;
    }

    .btn-chat, .btn-call {
      flex: 1;
      padding: 12px;
      font-size: 15px;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      transition: all 0.3s ease;
    }

    .btn-chat {
      background: #128C7E;
      color: white;
    }

    .btn-call {
      background: #4CAF50;
      color: white;
    }

    .btn-chat:hover { background: #075e54; transform: translateY(-2px); }
    .btn-call:hover { background: #388E3C; transform: translateY(-2px); }

    .overlay {
      position: fixed;
      top: 60px;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(0,0,0,0.4);
      z-index: 1999;
      display: none;
    }
    .overlay.active { display: block; }

    .alert {
      padding: 10px;
      margin: 10px 0;
      border-radius: 6px;
      font-size: 14px;
      text-align: center;
    }
    .alert-success { 
      background: #e8f5e9; 
      color: #2e7d32; 
      border-right: 3px solid #4caf50;
    }
    .alert-error { 
      background: #ffebee; 
      color: #c62828; 
      border-right: 3px solid #f44336;
    }

    .register-modal {
      position: fixed;
      top: 60px;
      right: -300px;
      width: 300px;
      height: calc(100% - 60px);
      background: white;
      box-shadow: -4px 0 15px rgba(0,0,0,0.2);
      z-index: 2500;
      transition: right 0.4s ease;
      padding: 20px;
      overflow-y: auto;
    }
    .register-modal.open {
      right: 0;
    }
    .modal-title {
      color: #075e54;
      font-size: 20px;
      font-weight: bold;
      margin-bottom: 20px;
      text-align: center;
    }
    .close-modal {
      position: absolute;
      top: 15px;
      left: 15px;
      background: none;
      border: none;
      font-size: 20px;
      color: #666;
      cursor: pointer;
    }

    .chat-modal {
      position: fixed;
      bottom: -500px;
      left: 50%;
      transform: translateX(-50%);
      width: 95%;
      max-width: 400px;
      height: 450px;
      background: white;
      border-radius: 15px 15px 0 0;
      box-shadow: 0 -5px 25px rgba(0,0,0,0.2);
      z-index: 3000;
      display: flex;
      flex-direction: column;
      transition: bottom 0.3s ease;
    }

    .chat-modal.open {
      bottom: 0;
    }

    .chat-header {
      background: linear-gradient(90deg, #075e54, #128C7E);
      color: white;
      padding: 15px;
      border-radius: 15px 15px 0 0;
      text-align: center;
      position: relative;
    }

    .chat-header h4 {
      margin: 0;
      font-size: 16px;
    }

    .close-chat {
      position: absolute;
      left: 15px;
      top: 50%;
      transform: translateY(-50%);
      background: none;
      border: none;
      color: white;
      font-size: 20px;
      cursor: pointer;
    }

    #chatDriverInfo {
      font-size: 12px;
      margin-top: 5px;
      opacity: 0.9;
    }

    .chat-messages {
      flex: 1;
      padding: 15px;
      overflow-y: auto;
      background: #f0f0f0;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .message {
      max-width: 80%;
      padding: 10px 15px;
      border-radius: 18px;
      font-size: 14px;
      line-height: 1.4;
      word-wrap: break-word;
    }

    .message.sent {
      background: #dcf8c6;
      align-self: flex-end;
      border-bottom-right-radius: 5px;
    }

    .message.received {
      background: white;
      align-self: flex-start;
      border-bottom-left-radius: 5px;
      box-shadow: 0 1px 2px rgba(0,0,0,0.1);
    }

    .message-time {
      font-size: 11px;
      color: #666;
      margin-top: 5px;
      text-align: right;
    }

    .chat-input {
      display: flex;
      padding: 15px;
      background: white;
      border-top: 1px solid #e0e0e0;
      gap: 10px;
    }

    .chat-input input {
      flex: 1;
      padding: 12px 15px;
      border: 1px solid #ddd;
      border-radius: 25px;
      font-size: 14px;
      outline: none;
    }

    .chat-input input:focus {
      border-color: #128C7E;
    }

    .chat-input button {
      background: #128C7E;
      color: white;
      border: none;
      border-radius: 50%;
      width: 45px;
      height: 45px;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .chat-input button:hover {
      background: #075e54;
    }

    .chat-input button:disabled {
      background: #ccc;
      cursor: not-allowed;
    }

    .chat-toggle-btn {
      position: fixed;
      bottom: 20px;
      left: 20px;
      width: 60px;
      height: 60px;
      background: #128C7E;
      color: white;
      border: none;
      border-radius: 50%;
      box-shadow: 0 4px 15px rgba(0,0,0,0.2);
      cursor: pointer;
      z-index: 2000;
      display: none;
      align-items: center;
      justify-content: center;
      font-size: 20px;
      transition: all 0.3s ease;
    }

    .chat-toggle-btn:hover {
      background: #075e54;
      transform: scale(1.05);
    }

    .chat-toggle-btn.has-unread::after {
      content: '';
      position: absolute;
      top: 5px;
      right: 5px;
      width: 12px;
      height: 12px;
      background: #ff4444;
      border-radius: 50%;
      border: 2px solid white;
    }

    .drivers-section-hidden .section-title,
    .drivers-section-hidden .driver-list {
      display: none !important;
    }

    .user-marker {
      background: #075e54;
      border: 3px solid white;
      border-radius: 50%;
      width: 20px;
      height: 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.3);
    }

    .driver-marker {
      background: #ff9800;
      border: 3px solid white;
      border-radius: 50%;
      width: 24px;
      height: 24px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.3);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 12px;
      color: white;
      font-weight: bold;
    }

    .typing-indicator {
      font-style: italic;
      color: #666;
      font-size: 12px;
      padding: 5px 15px;
    }

    .privacy-settings {
      background: #f8f9fa;
      border-radius: 10px;
      padding: 15px;
      margin: 15px 0;
    }

    .privacy-setting-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 0;
      border-bottom: 1px solid #e9ecef;
    }

    .privacy-setting-item:last-child {
      border-bottom: none;
    }

    .switch {
      position: relative;
      display: inline-block;
      width: 50px;
      height: 24px;
    }

    .switch input {
      opacity: 0;
      width: 0;
      height: 0;
    }

    .slider {
      position: absolute;
      cursor: pointer;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: #ccc;
      transition: .4s;
      border-radius: 24px;
    }

    .slider:before {
      position: absolute;
      content: "";
      height: 16px;
      width: 16px;
      left: 4px;
      bottom: 4px;
      background-color: white;
      transition: .4s;
      border-radius: 50%;
    }

    input:checked + .slider {
      background-color: #075e54;
    }

    input:checked + .slider:before {
      transform: translateX(26px);
    }

    .refresh-indicator {
      position: fixed;
      top: 70px;
      left: 50%;
      transform: translateX(-50%);
      background: rgba(7, 94, 84, 0.9);
      color: white;
      padding: 8px 16px;
      border-radius: 20px;
      font-size: 12px;
      z-index: 1000;
      display: none;
    }

    .field-error {
      animation: shake 0.5s ease-in-out;
    }

    @keyframes shake {
      0%, 100% { transform: translateX(0); }
      25% { transform: translateX(-5px); }
      75% { transform: translateX(5px); }
    }

    input:valid {
      border-color: #4CAF50 !important;
    }

    input:invalid:not(:focus):not(:placeholder-shown) {
      border-color: #f44336 !important;
    }

    .performance-optimized {
      image-rendering: -webkit-optimize-contrast;
      image-rendering: crisp-edges;
    }

    @media (prefers-reduced-motion: reduce) {
      * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
      }
    }

    @media (max-width: 768px) {
      .sidebar, .register-modal {
        width: 300px;
        right: -300px;
      }
      .driver-info-card {
        width: 95%;
      }
    }
  </style>
</head>
<body>
  <header class="header">
    <div></div>
    🚖 تاكسي نواكشوط
    <button class="menu-toggle" id="menuToggle">
      <i class="fas fa-bars"></i>
    </button>
  </header>

  <div class="refresh-indicator" id="refreshIndicator">
    <i class="fas fa-sync-alt fa-spin"></i> جاري التحديث...
  </div>

  <div class="overlay" id="overlay"></div>

  <aside class="sidebar" id="sidebar">
    <h3>لوحة التحكم</h3>
    
    <!-- قسم الإعدادات -->
    <div class="section" id="settingsSection" style="display:none;">
      <div class="section-title">⚙️ الإعدادات</div>
      <div class="privacy-settings">
        <div class="privacy-setting-item">
          <span>مشاركة الموقع</span>
          <label class="switch">
            <input type="checkbox" id="shareLocationSetting" checked>
            <span class="slider"></span>
          </label>
        </div>
        <div class="privacy-setting-item">
          <span>ظهور للحسابات الأخرى</span>
          <label class="switch">
            <input type="checkbox" id="showProfileSetting" checked>
            <span class="slider"></span>
          </label>
        </div>
        <div class="privacy-setting-item">
          <span>استقبال دردشات</span>
          <label class="switch">
            <input type="checkbox" id="allowChatSetting" checked>
            <span class="slider"></span>
          </label>
        </div>
      </div>
      <button class="btn btn-outline" id="saveSettingsBtn">
        <i class="fas fa-save"></i> حفظ الإعدادات
      </button>
    </div>

    <div id="authSection">
      <div class="form-group">
        <label><i class="fas fa-envelope"></i> البريد الإلكتروني</label>
        <input type="email" id="email" placeholder="example@gmail.com">
      </div>
      <div class="form-group">
        <label><i class="fas fa-lock"></i> كلمة المرور</label>
        <input type="password" id="password" placeholder="أدخل كلمة المرور">
      </div>
      <button class="btn" id="loginBtn">🔐 تسجيل الدخول</button>
      
      <div class="register-type">
        <button class="btn btn-outline" id="registerDriverBtn">
          🚖 سائق
        </button>
        <button class="btn btn-outline" id="registerUserBtn">
          👤 زبون
        </button>
      </div>
    </div>

    <div id="userProfileSection" style="display:none;">
      <div class="alert alert-success" id="welcomeMsg">مرحبًا، <span id="userName"></span>!</div>
      <button class="btn btn-outline" id="logoutBtn">🚪 تسجيل الخروج</button>

      <div class="section">
        <div class="form-group">
          <label><i class="fas fa-user"></i> الاسم الكامل</label>
          <input type="text" id="profileName" placeholder="أدخل الاسم">
        </div>
        <div class="form-group" id="profileIdCardGroup" style="display:none;">
          <label><i class="fas fa-id-card"></i> رقم البطاقة / الرخصة</label>
          <input type="text" id="profileIdCard" placeholder="12345678">
        </div>
        <div class="form-group" id="profilePhoneGroup" style="display:none;">
          <label><i class="fas fa-phone"></i> رقم الهاتف</label>
          <input type="tel" id="profilePhone" placeholder="46XXXXXX">
        </div>
        <button class="btn" id="saveProfileBtn">💾 حفظ المعلومات</button>
        <button class="btn" id="startTrackingBtn" style="display:none;">📍 تفعيل تحديث الموقع</button>
      </div>
    </div>

    <div class="section drivers-section" id="driversSection">
      <div class="section-title">السائقون النشطون</div>
      <ul class="driver-list" id="driverList">
        <li class="driver-item" style="padding:15px; text-align:center; color:#666;">يجب تفعيل الموقع وتسجيل الدخول</li>
      </ul>
    </div>
  </aside>

  <!-- نوافذ التسجيل -->
  <div id="registerDriverModal" class="register-modal">
    <button class="close-modal" id="closeRegisterDriverModal">&times;</button>
    <div class="modal-title">📝 تسجيل سائق</div>

    <div class="form-group">
      <label><i class="fas fa-user"></i> الاسم الكامل</label>
      <input type="text" id="regDriverName" placeholder="أدخل الاسم">
    </div>
    <div class="form-group">
      <label><i class="fas fa-id-card"></i> رقم البطاقة / الرخصة</label>
      <input type="text" id="regDriverIdCard" placeholder="12345678">
    </div>
    <div class="form-group">
      <label><i class="fas fa-phone"></i> رقم الهاتف</label>
      <input type="tel" id="regDriverPhone" placeholder="46XXXXXX">
    </div>
    <div class="form-group">
      <label><i class="fas fa-envelope"></i> البريد الإلكتروني</label>
      <input type="email" id="regDriverEmail" placeholder="example@gmail.com">
    </div>
    <div class="form-group">
      <label><i class="fas fa-lock"></i> كلمة المرور</label>
      <input type="password" id="regDriverPassword" placeholder="أدخل كلمة المرور">
    </div>
    <div class="form-group">
      <input type="checkbox" id="driverTermsCheck" required>
      <label for="driverTermsCheck">
        أوافق على شروط الاستخدام، وأتعهد بعدم تعريض أي مستخدم لأي خطر.
      </label>
    </div>
    <button class="btn" id="submitDriverRegister">✅ تسجيل السائق</button>
  </div>

  <div id="registerUserModal" class="register-modal">
    <button class="close-modal" id="closeRegisterUserModal">&times;</button>
    <div class="modal-title">📝 تسجيل زبون</div>

    <div class="form-group">
      <label><i class="fas fa-user"></i> الاسم الكامل</label>
      <input type="text" id="regUserName" placeholder="أدخل الاسم">
    </div>
    <div class="form-group">
      <label><i class="fas fa-envelope"></i> البريد الإلكتروني</label>
      <input type="email" id="regUserEmail" placeholder="example@gmail.com">
    </div>
    <div class="form-group">
      <label><i class="fas fa-lock"></i> كلمة المرور</label>
      <input type="password" id="regUserPassword" placeholder="أدخل كلمة المرور">
    </div>
    <button class="btn" id="submitUserRegister">✅ تسجيل الزبون</button>
  </div>

  <!-- نافذة الدردشة -->
  <div id="chatModal" class="chat-modal">
    <div class="chat-header">
      <button class="close-chat" id="closeChat">&times;</button>
      <h4>💬 محادثة مع <span id="chatPartnerName">---</span></h4>
      <div id="chatPartnerInfo"></div>
      <div id="typingIndicator" class="typing-indicator" style="display:none;">
        <i class="fas fa-pencil-alt"></i> <span id="typingUserName">---</span> يكتب...
      </div>
    </div>
    <div class="chat-messages" id="chatMessages">
      <div style="text-align:center;color:#888;margin-top:20px;">افتح دردشة مع مستخدم آخر</div>
    </div>
    <div class="chat-input">
      <input type="text" id="messageInput" placeholder="اكتب رسالتك هنا..." maxlength="500">
      <button id="sendMessageBtn">📤</button>
    </div>
  </div>

  <button class="chat-toggle-btn" id="chatToggleBtn">
    <i class="fas fa-comments"></i>
  </button>

  <!-- شاشة الإذن -->
  <div id="permissionScreen">
    <div class="emoji">📍</div>
    <h2>تفعيل الموقع مطلوب</h2>
    <p>لرؤية المستخدمين على الخريطة، يجب مشاركة موقعك المباشر.</p>
    <div class="requirement">✅ نستخدم موقعك فقط أثناء الجلسة</div>
    <div class="requirement">✅ لا يتم تخزينه أو مشاركته</div>
    <div class="requirement">✅ يمكنك إيقافه في أي وقت من الإعدادات</div>
    <button id="allowBtn">
      <span class="emoji">🧭</span> تفعيل الموقع الآن
    </button>
  </div>

  <main class="map-container" id="mapContainer" style="display:none;">
    <div id="map"></div>
  </main>

  <div class="control-btns" id="controlBtns">
    <button class="btn" id="requestBtn">
      <span class="emoji">🚕</span> طلب تاكسي
    </button>
  </div>

  <div class="driver-info-card" id="userInfoCard">
    <h4 id="cardUserName">--- المستخدم ---</h4>
    <p><strong>الدور:</strong> <span id="cardUserRole">---</span></p>
    <p><strong>الهاتف:</strong> <span id="cardUserPhone">---</span></p>
    <p><strong>المسافة:</strong> <span class="user-distance" id="cardDistanceText">--</span></p>
    <div class="btn-group">
      <button class="btn-chat" id="cardChatBtn">
        <i class="fas fa-comments"></i> دردشة
      </button>
      <a class="btn-call" id="cardCallBtn" href="#">
        <i class="fas fa-phone"></i> اتصال
      </a>
    </div>
  </div>

  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-auth-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore-compat.js"></script>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

  <script>
    const firebaseConfig = {
      apiKey: "AIzaSyCd72265mC_yNPAXYl-8jXxJgZk-afC7Y4",
      authDomain: "ryada-6773b.firebaseapp.com",
      projectId: "ryada-6773b",
      storageBucket: "ryada-6773b.firebasestorage.app",
      messagingSenderId: "567927086495",
      appId: "1:567927086495:web:1cf92498647022f017b1aa",
      measurementId: "G-F08ZYR9FTH"
    };

    firebase.initializeApp(firebaseConfig);
    const auth = firebase.auth();
    const db = firebase.firestore();

    let map = null;
    let userMarker = null;
    let userLatLng = null;
    let trackingInterval = null;
    let userMarkers = new Map();
    let currentChatRoom = null;
    let chatUnsubscribe = null;
    let currentChatPartner = null;
    let lastLocationUpdate = 0;
    let currentUserRole = null;
    let typingTimeout = null;
    let isLocationEnabled = false;

    // ==================== نظام التخزين المؤقت ====================
    const cache = {
      users: { data: null, timestamp: 0, ttl: 30000 },
      drivers: { data: null, timestamp: 0, ttl: 15000 }
    };

    // ==================== نظام إدارة التحميل ====================
    const loadingManager = {
      show: function(message = 'جاري التحميل...') {
        const loader = document.createElement('div');
        loader.id = 'globalLoader';
        loader.innerHTML = `
          <div style="position:fixed; top:0; left:0; right:0; bottom:0; background:rgba(0,0,0,0.5); z-index:10000; display:flex; align-items:center; justify-content:center;">
            <div style="background:white; padding:20px; border-radius:12px; text-align:center; box-shadow:0 4px 20px rgba(0,0,0,0.15);">
              <div class="fas fa-spinner fa-spin" style="font-size:24px; color:#075e54; margin-bottom:10px;"></div>
              <div style="color:#333; font-weight:500;">${message}</div>
            </div>
          </div>
        `;
        document.body.appendChild(loader);
      },
      
      hide: function() {
        const loader = document.getElementById('globalLoader');
        if (loader) loader.remove();
      }
    };

    // ==================== نظام الإشعارات ====================
    const notificationManager = {
      show: function(title, message, type = 'info', duration = 4000) {
        const notification = document.createElement('div');
        const bgColor = type === 'success' ? '#4CAF50' : 
                       type === 'error' ? '#f44336' : 
                       type === 'warning' ? '#ff9800' : '#2196F3';
        
        notification.innerHTML = `
          <div style="position:fixed; top:80px; right:20px; background:white; padding:15px; border-radius:12px; box-shadow:0 4px 20px rgba(0,0,0,0.15); border-right:4px solid ${bgColor}; z-index:10000; max-width:350px; min-width:300px;">
            <div style="display:flex; align-items:center; gap:10px;">
              <div style="color:${bgColor}; font-size:18px;">
                ${type === 'success' ? '✅' : type === 'error' ? '❌' : type === 'warning' ? '⚠️' : 'ℹ️'}
              </div>
              <div style="flex:1;">
                <div style="font-weight:bold; color:#333; margin-bottom:5px;">${title}</div>
                <div style="color:#666; font-size:14px;">${message}</div>
              </div>
              <button onclick="this.parentElement.parentElement.remove()" style="background:none; border:none; color:#999; cursor:pointer; padding:5px;">✕</button>
            </div>
          </div>
        `;
        
        document.body.appendChild(notification);
        
        setTimeout(() => {
          if (notification.parentNode) notification.remove();
        }, duration);
      }
    };

    // ==================== نظام إدارة الخصوصية ====================
    const privacyManager = {
      settings: {
        shareLocation: true,
        showProfile: true,
        allowChat: true,
        onlineStatus: true
      },
      
      init: function() {
        this.loadSettings();
        this.applySettings();
      },
      
      loadSettings: function() {
        const saved = localStorage.getItem('privacySettings');
        if (saved) {
          this.settings = { ...this.settings, ...JSON.parse(saved) };
        }
        this.updateUI();
      },
      
      saveSettings: function() {
        localStorage.setItem('privacySettings', JSON.stringify(this.settings));
        this.applySettings();
        notificationManager.show('تم الحفظ', 'تم حفظ الإعدادات بنجاح', 'success');
      },
      
      applySettings: function() {
        const user = auth.currentUser;
        if (!user) return;
        
        db.collection('users').doc(user.uid).update({
          privacySettings: this.settings,
          isVisible: this.settings.shareLocation && this.settings.onlineStatus
        });
      },
      
      updateUI: function() {
        document.getElementById('shareLocationSetting').checked = this.settings.shareLocation;
        document.getElementById('showProfileSetting').checked = this.settings.showProfile;
        document.getElementById('allowChatSetting').checked = this.settings.allowChat;
      }
    };

    // ==================== نظام إدارة الدردشة ====================
    const chatManager = {
      typingIndicator: function(roomId, isTyping) {
        if (!roomId) return;
        
        db.collection('chats').doc(roomId).update({
          [`typing.${auth.currentUser.uid}`]: isTyping,
          lastActivity: firebase.firestore.FieldValue.serverTimestamp()
        });
      }
    };

    // ==================== دوال مساعدة محسنة ====================
    function debounce(func, wait) {
      let timeout;
      return function executedFunction(...args) {
        const later = () => {
          clearTimeout(timeout);
          func(...args);
        };
        clearTimeout(timeout);
        timeout = setTimeout(later, wait);
      };
    }

    function calculateDistance(lat1, lon1, lat2, lon2) {
      const R = 6371;
      const dLat = (lat2 - lat1) * Math.PI / 180;
      const dLon = (lon2 - lon1) * Math.PI / 180;
      const a = 
        Math.sin(dLat/2) * Math.sin(dLat/2) +
        Math.cos(lat1 * Math.PI / 180) * Math.cos(lat2 * Math.PI / 180) * 
        Math.sin(dLon/2) * Math.sin(dLon/2);
      const c = 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1-a));
      return R * c;
    }

    function toLatLng(loc) {
      if (!loc) return null;
      return L.latLng(loc.latitude || loc.lat, loc.longitude || loc.lng);
    }

    // ==================== نظام التحقق من الصلاحيات ====================
    async function checkUserPermission(requiredRole = null) {
      const user = auth.currentUser;
      if (!user) throw new Error('يجب تسجيل الدخول');
      
      const userDoc = await db.collection('users').doc(user.uid).get();
      if (!userDoc.exists) throw new Error('المستخدم غير موجود');
      
      const userData = userDoc.data();
      if (requiredRole && userData.role !== requiredRole) {
        throw new Error('غير مصرح بهذا الإجراء');
      }
      
      return userData;
    }

    // ==================== دوال الموقع والتحديث ====================
    async function updateUserLocation(uid, location) {
      try {
        await checkUserPermission();
        await db.collection('users').doc(uid).update({
          location: {
            latitude: location.latitude,
            longitude: location.longitude,
            timestamp: firebase.firestore.FieldValue.serverTimestamp()
          },
          lastSeen: firebase.firestore.FieldValue.serverTimestamp()
        });
      } catch (error) {
        console.error('فشل تحديث الموقع:', error);
      }
    }

    let locationUpdateQueue = [];
    let isUpdatingLocation = false;

    async function optimizedLocationUpdate(location) {
      locationUpdateQueue.push(location);
      
      if (!isUpdatingLocation) {
        isUpdatingLocation = true;
        
        while (locationUpdateQueue.length > 0) {
          const latestLocation = locationUpdateQueue[locationUpdateQueue.length - 1];
          locationUpdateQueue = [];
          
          try {
            await updateUserLocation(auth.currentUser.uid, latestLocation);
          } catch (error) {
            console.error('فشل تحديث الموقع:', error);
          }
          
          await new Promise(resolve => setTimeout(resolve, 2000));
        }
        
        isUpdatingLocation = false;
      }
    }

    // ==================== دوال الخريطة المحسنة ====================
    async function enableLocationAndInitMap() {
      return new Promise((resolve, reject) => {
        if (!navigator.geolocation) {
          reject(new Error('الموقع غير مدعوم في متصفحك'));
          return;
        }

        loadingManager.show('جاري تفعيل الموقع...');

        navigator.geolocation.getCurrentPosition(
          async (position) => {
            try {
              const { latitude, longitude } = position.coords;
              userLatLng = { latitude, longitude };

              document.getElementById('permissionScreen').style.display = 'none';
              document.getElementById('mapContainer').style.display = 'block';

              if (!map) {
                map = L.map('map').setView([latitude, longitude], 14);
                
                if (navigator.hardwareConcurrency && navigator.hardwareConcurrency <= 4) {
                  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                    attribution: '&copy; OpenStreetMap',
                    detectRetina: false
                  }).addTo(map);
                } else {
                  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                    attribution: '&copy; OpenStreetMap'
                  }).addTo(map);
                }

                const userIcon = L.divIcon({ 
                  html: '<div class="user-marker"></div>', 
                  className: 'user-marker-icon',
                  iconSize: [20, 20],
                  iconAnchor: [10, 10]
                });
                
                userMarker = L.marker([latitude, longitude], {
                  title: 'موقعك',
                  icon: userIcon,
                  zIndexOffset: 1000
                }).addTo(map);
                userMarker.bindPopup("أنت هنا").openPopup();

                setTimeout(() => {
                  if (map) map.invalidateSize();
                }, 300);
              } else {
                userMarker.setLatLng([latitude, longitude]);
                map.setView([latitude, longitude], 14);
                setTimeout(() => {
                  if (map) map.invalidateSize();
                }, 100);
              }

              startLocationTracking();
              await loadActiveUsersOnMap();
              enableLocationDependentFeatures();
              isLocationEnabled = true;
              
              resolve();
            } catch (error) {
              reject(error);
            } finally {
              loadingManager.hide();
            }
          },
          (error) => {
            loadingManager.hide();
            let msg = 'فشل الحصول على الموقع';
            if (error.code === error.PERMISSION_DENIED) {
              msg = 'يرجى تمكين الموقع في إعدادات المتصفح';
            } else if (error.code === error.POSITION_UNAVAILABLE) {
              msg = 'الموقع غير متوفر — تأكد من تفعيل GPS';
            } else if (error.code === error.TIMEOUT) {
              msg = 'انتهت مدة الانتظار — حاول مجددًا';
            }
            reject(new Error(msg));
          },
          { 
            enableHighAccuracy: true, 
            timeout: 20000, 
            maximumAge: 10000 
          }
        );
      });
    }

    // ==================== تفعيل الميزات المعتمدة على الموقع ====================
    function enableLocationDependentFeatures() {
      const user = auth.currentUser;
      if (!user) return;

      if (currentUserRole === 'user') {
        document.getElementById('controlBtns').style.display = 'flex';
        notificationManager.show('جاهز', 'يمكنك الآن طلب تاكسي', 'success');
      }

      document.getElementById('chatToggleBtn').style.display = 'flex';
      
      console.log('✅ تم تفعيل الميزات المعتمدة على الموقع');
    }

    function disableLocationDependentFeatures() {
      document.getElementById('controlBtns').style.display = 'none';
      document.getElementById('chatToggleBtn').style.display = 'none';
      isLocationEnabled = false;
    }

    function startLocationTracking() {
      if (trackingInterval) {
        navigator.geolocation.clearWatch(trackingInterval);
      }

      trackingInterval = navigator.geolocation.watchPosition(
        async (position) => {
          const { latitude, longitude } = position.coords;
          userLatLng = { latitude, longitude };
          
          if (userMarker) {
            userMarker.setLatLng([latitude, longitude]);
          }

          const now = Date.now();
          if (now - lastLocationUpdate > 10000 && privacyManager.settings.shareLocation) {
            lastLocationUpdate = now;
            const user = auth.currentUser;
            if (user) {
              await optimizedLocationUpdate({ latitude, longitude });
            }
          }
        },
        (error) => {
          console.warn('خطأ في تتبع الموقع:', error);
          notificationManager.show('تحذير', 'فقدان الاتصال بالموقع', 'warning');
        },
        { 
          enableHighAccuracy: true, 
          maximumAge: 10000, 
          timeout: 15000 
        }
      );
    }

    // ==================== دوال تحميل المستخدمين ====================
    async function loadActiveUsersWithCache() {
      const now = Date.now();
      if (cache.users.data && (now - cache.users.timestamp < cache.users.ttl)) {
        return cache.users.data;
      }
      
      const cutoff = firebase.firestore.Timestamp.fromMillis(Date.now() - 120000);
      const usersSnapshot = await db.collection('users')
        .where('location.timestamp', '>=', cutoff)
        .limit(50)
        .get();
      
      cache.users.data = usersSnapshot;
      cache.users.timestamp = now;
      
      return usersSnapshot;
    }

    async function loadActiveUsersOnMap() {
      if (!map) return;

      try {
        document.getElementById('refreshIndicator').style.display = 'block';
        
        const usersSnapshot = await loadActiveUsersWithCache();
        const currentUser = auth.currentUser;

        userMarkers.forEach(marker => marker.remove());
        userMarkers.clear();

        const userList = [];
        const listEl = document.getElementById('driverList');

        if (usersSnapshot.empty) {
          listEl.innerHTML = '<li class="driver-item" style="text-align:center;color:#888;">لا مستخدمين نشطين</li>';
          document.getElementById('refreshIndicator').style.display = 'none';
          return;
        }

        listEl.innerHTML = '';

        usersSnapshot.forEach(doc => {
          const user = doc.data();
          if (!user.location?.latitude || user.uid === currentUser?.uid) return;

          const userLatLng = toLatLng(user.location);
          const distanceKm = calculateDistance(
            userLatLng?.latitude || 18.0859,
            userLatLng?.longitude || -15.9707,
            user.location.latitude,
            user.location.longitude
          );

          const isDriver = user.role === 'driver';
          const iconClass = isDriver ? 'driver-marker' : 'user-marker';
          const iconText = isDriver ? '🚗' : '👤';
          
          const userIcon = L.divIcon({ 
            html: `<div class="${iconClass}">${iconText}</div>`, 
            className: `${iconClass}-icon`,
            iconSize: isDriver ? [24, 24] : [20, 20],
            iconAnchor: isDriver ? [12, 12] : [10, 10]
          });
          
          const marker = L.marker(userLatLng, { icon: userIcon }).addTo(map)
            .bindTooltip(`<b>${user.name}</b><br>${isDriver ? 'سائق' : 'زبون'} - ${distanceKm.toFixed(1)} كم`);
          
          marker.on('click', () => showUserInfoCard(user, distanceKm));
          userMarkers.set(user.uid, marker);

          if (user.role === 'driver' && userList.length < 10) {
            userList.push({ ...user, distanceKm });
          }
        });

        updateUserListInSidebar(userList);
        document.getElementById('refreshIndicator').style.display = 'none';
        
      } catch (error) {
        console.error('فشل تحميل المستخدمين:', error);
        document.getElementById('refreshIndicator').style.display = 'none';
        notificationManager.show('خطأ', 'فشل تحميل البيانات', 'error');
      }
    }

    // ==================== دوال الواجهة ====================
    function showUserInfoCard(user, distanceKm) {
      if (!isLocationEnabled) {
        notificationManager.show('خطأ', 'يجب تفعيل الموقع أولاً', 'error');
        return;
      }

      const card = document.getElementById('userInfoCard');
      document.getElementById('cardUserName').textContent = user.name || '---';
      document.getElementById('cardUserRole').textContent = user.role === 'driver' ? 'سائق' : 'زبون';
      document.getElementById('cardUserPhone').textContent = user.phone || '---';
      document.getElementById('cardDistanceText').textContent = `${distanceKm.toFixed(1)} كم`;

      document.getElementById('cardChatBtn').onclick = () => {
        if (!privacyManager.settings.allowChat) {
          notificationManager.show('خطأ', 'الدردشة معطلة من الإعدادات', 'error');
          return;
        }
        openChatWithUser(user);
        card.style.display = 'none';
      };

      const callBtn = document.getElementById('cardCallBtn');
      if (user.phone) {
        callBtn.href = `tel:${user.phone}`;
        callBtn.style.display = 'flex';
      } else {
        callBtn.style.display = 'none';
      }

      card.style.display = 'block';
    }

    function updateUserListInSidebar(users) {
      const list = document.getElementById('driverList');
      const currentUserRole = window.currentUserRole;
      
      if (currentUserRole !== 'user') {
        list.innerHTML = '<li class="driver-item" style="text-align:center;color:#888;">القائمة متاحة للزبائن فقط</li>';
        return;
      }

      if (users.length === 0) {
        list.innerHTML = '<li class="driver-item" style="text-align:center;color:#888;">لا سائقين نشطين</li>';
        return;
      }

      list.innerHTML = '';
      users.forEach(user => {
        const item = document.createElement('li');
        item.className = 'driver-item';
        item.innerHTML = `
          <div>
            <strong>${user.name || '---'}</strong><br>
            <small>${user.distanceKm.toFixed(1)} كم</small>
          </div>
          <div>
            <i class="fas fa-comments" title="دردشة"></i>
          </div>
        `;

        item.addEventListener('click', (e) => {
          if (e.target.closest('i')) return;
          if (!privacyManager.settings.allowChat) {
            notificationManager.show('خطأ', 'الدردشة معطلة من الإعدادات', 'error');
            return;
          }
          openChatWithUser(user);
        });

        list.appendChild(item);
      });
    }

    // ==================== دوال الدردشة المحسنة ====================
    async function openChatWithUser(user) {
      if (!isLocationEnabled) {
        notificationManager.show('خطأ', 'يجب تفعيل الموقع أولاً لاستخدام الدردشة', 'error');
        return;
      }

      if (!auth.currentUser) {
        notificationManager.show('خطأ', 'يجب تسجيل الدخول أولاً', 'error');
        return;
      }
      
      if (!privacyManager.settings.allowChat) {
        notificationManager.show('خطأ', 'الدردشة معطلة من الإعدادات', 'error');
        return;
      }
      
      currentChatPartner = user;
      const currentUser = auth.currentUser;
      const uids = [currentUser.uid, user.uid].sort();
      currentChatRoom = uids.join('_');

      document.getElementById('chatPartnerName').textContent = user.name || '---';
      document.getElementById('chatPartnerInfo').textContent = `${user.role === 'driver' ? 'سائق' : 'زبون'} - ${user.phone || 'لا يوجد هاتف'}`;
      document.getElementById('chatMessages').innerHTML = '<div style="text-align:center;color:#888;">جارٍ التحميل...</div>';

      if (chatUnsubscribe && typeof chatUnsubscribe === 'function') chatUnsubscribe();

      chatUnsubscribe = db.collection('chats').doc(currentChatRoom).collection('messages')
        .orderBy('timestamp', 'asc')
        .onSnapshot({ includeMetadataChanges: true }, (snapshot) => {
          renderMessages(snapshot.docs);
          markMessagesAsRead();
        });

      db.collection('chats').doc(currentChatRoom).onSnapshot((doc) => {
        const data = doc.data();
        if (data && data.typing) {
          const typingUsers = Object.entries(data.typing)
            .filter(([uid, isTyping]) => uid !== auth.currentUser.uid && isTyping);
          
          if (typingUsers.length > 0) {
            document.getElementById('typingUserName').textContent = user.name;
            document.getElementById('typingIndicator').style.display = 'block';
          } else {
            document.getElementById('typingIndicator').style.display = 'none';
          }
        }
      });

      document.getElementById('chatModal').classList.add('open');
      document.getElementById('messageInput').focus();
      document.getElementById('chatToggleBtn').classList.remove('has-unread');
    }

    function renderMessages(messageDocs) {
      const container = document.getElementById('chatMessages');
      const user = auth.currentUser;
      if (!user) return;
      
      container.innerHTML = '';
      
      if (messageDocs.length === 0) {
        container.innerHTML = '<div style="text-align:center;color:#888;margin-top:20px;">لا توجد رسائل بعد. ابدأ المحادثة!</div>';
        return;
      }

      messageDocs.forEach(doc => {
        const msg = doc.data();
        if (!msg.text || !msg.sender || !msg.timestamp) return;
        
        const isSent = msg.sender === user.uid;
        const time = msg.timestamp?.toDate?.() || new Date(msg.timestamp?.seconds ? msg.timestamp.seconds * 1000 : Date.now());
        const timeStr = time.toLocaleTimeString('ar-EG', { hour: '2-digit', minute: '2-digit' });
        
        const div = document.createElement('div');
        div.className = `message ${isSent ? 'sent' : 'received'}`;
        div.innerHTML = `<div>${msg.text}</div><div class="message-time">${timeStr}</div>`;
        container.appendChild(div);
      });
      
      container.scrollTop = container.scrollHeight;
    }

    async function markMessagesAsRead() {
      if (!currentChatRoom || !auth.currentUser || !currentChatPartner) return;
      try {
        const batch = db.batch();
        const ref = db.collection('chats').doc(currentChatRoom).collection('messages');
        const snap = await ref.where('sender', '==', currentChatPartner.uid).where('read', '==', false).get();
        snap.docs.forEach(doc => batch.update(doc.ref, { read: true }));
        if (snap.size > 0) await batch.commit();
      } catch (error) { 
        console.error('خطأ في تحديد الرسائل كمقروءة:', error); 
      }
    }

    async function sendMessage() {
      const input = document.getElementById('messageInput');
      const text = input.value.trim();
      if (!text || !currentChatRoom || !auth.currentUser) return;
      
      const btn = document.getElementById('sendMessageBtn');
      btn.disabled = true;
      
      try {
        await db.collection('chats').doc(currentChatRoom).collection('messages').add({
          text, 
          sender: auth.currentUser.uid,
          timestamp: firebase.firestore.FieldValue.serverTimestamp(),
          read: false
        });
        input.value = '';
        
        chatManager.typingIndicator(currentChatRoom, false);
        
      } catch (error) {
        notificationManager.show('خطأ', 'فشل إرسال الرسالة', 'error');
      } finally {
        btn.disabled = false;
      }
    }

    // ==================== دوال إدارة الأدوار المحسنة ====================
    function updateUIBasedOnRole(userData) {
      const isDriver = userData?.role === 'driver';
      const isUser = userData?.role === 'user';
      window.currentUserRole = userData?.role;

      const userNameSpan = document.getElementById('userName');
      const profileName = document.getElementById('profileName');
      const profileIdCard = document.getElementById('profileIdCard');
      const profilePhone = document.getElementById('profilePhone');
      const driversSection = document.getElementById('driversSection');
      const chatToggleBtn = document.getElementById('chatToggleBtn');
      const controlBtns = document.getElementById('controlBtns');
      const startTrackingBtn = document.getElementById('startTrackingBtn');
      const settingsSection = document.getElementById('settingsSection');

      const displayName = userData.name || userData.email?.split('@')[0] || 'مستخدم';
      userNameSpan.textContent = displayName;
      document.getElementById('welcomeMsg').innerHTML = `مرحبًا، <strong>${displayName}</strong>!`;
      profileName.value = userData.name || '';

      settingsSection.style.display = 'block';
      privacyManager.init();

      disableLocationDependentFeatures();

      if (isDriver) {
        document.getElementById('profileIdCardGroup').style.display = 'block';
        document.getElementById('profilePhoneGroup').style.display = 'block';
        document.getElementById('saveProfileBtn').style.display = 'block';
        startTrackingBtn.style.display = 'block';
        profileIdCard.value = userData.idCard || '';
        profilePhone.value = userData.phone || '';
        
        driversSection.classList.add('drivers-section-hidden');

        if (isLocationEnabled) {
          chatToggleBtn.style.display = 'flex';
        }

      } else if (isUser) {
        document.getElementById('profileIdCardGroup').style.display = 'none';
        document.getElementById('profilePhoneGroup').style.display = 'none';
        document.getElementById('saveProfileBtn').style.display = 'none';
        startTrackingBtn.style.display = 'none';
        
        driversSection.classList.remove('drivers-section-hidden');

        if (isLocationEnabled) {
          controlBtns.style.display = 'block';
          chatToggleBtn.style.display = 'flex';
        }
      }

      if (isLocationEnabled) {
        enableLocationDependentFeatures();
      }
    }

    // ==================== دوال التحقق من التسجيل ====================
    function validateDriverRegistration(data) {
        const { name, email, password, idCard, phone, terms } = data;
        
        if (!name || name.trim().length < 2) {
            return 'الاسم يجب أن يحتوي على حرفين على الأقل';
        }
        
        const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        if (!email || !emailRegex.test(email.trim())) {
            return 'البريد الإلكتروني غير صالح';
        }
        
        if (!password || password.length < 6) {
            return 'كلمة المرور يجب أن تكون 6 أحرف على الأقل';
        }
        
        if (!idCard || idCard.trim().length < 4) {
            return 'رقم البطاقة/الرخصة غير صالح';
        }
        
        const phoneRegex = /^[\d\s\-\+]{8,15}$/;
        if (!phone || !phoneRegex.test(phone.trim())) {
            return 'رقم الهاتف غير صالح';
        }
        
        if (!terms) {
            return 'يجب الموافقة على شروط الاستخدام';
        }
        
        return null;
    }

    function validateUserRegistration(data) {
        const { name, email, password } = data;
        
        if (!name || name.trim().length < 2) {
            return 'الاسم يجب أن يحتوي على حرفين على الأقل';
        }
        
        const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        if (!email || !emailRegex.test(email.trim())) {
            return 'البريد الإلكتروني غير صالح';
        }
        
        if (!password || password.length < 6) {
            return 'كلمة المرور يجب أن تكون 6 أحرف على الأقل';
        }
        
        return null;
    }

    // ==================== دوال التسجيل المحسنة ====================
    async function registerDriver() {
        const btn = document.getElementById('submitDriverRegister');
        const originalText = btn.innerHTML;
        
        try {
            const formData = {
                name: document.getElementById('regDriverName').value.trim(),
                idCard: document.getElementById('regDriverIdCard').value.trim(),
                phone: document.getElementById('regDriverPhone').value.trim(),
                email: document.getElementById('regDriverEmail').value.trim(),
                password: document.getElementById('regDriverPassword').value,
                terms: document.getElementById('driverTermsCheck').checked
            };

            const validationError = validateDriverRegistration(formData);
            if (validationError) {
                throw new Error(validationError);
            }

            btn.disabled = true;
            btn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> جاري إنشاء الحساب...';

            const userCredential = await auth.createUserWithEmailAndPassword(
                formData.email, 
                formData.password
            );
            const user = userCredential.user;

            const userData = {
                uid: user.uid,
                name: formData.name,
                email: formData.email,
                role: 'driver',
                phone: formData.phone,
                idCard: formData.idCard,
                privacySettings: privacyManager.settings,
                isOnline: false,
                createdAt: firebase.firestore.FieldValue.serverTimestamp(),
                lastSeen: firebase.firestore.FieldValue.serverTimestamp()
            };

            await db.collection('users').doc(user.uid).set(userData);

            document.getElementById('registerDriverModal').classList.remove('open');
            document.getElementById('overlay').classList.remove('active');

            if (userLatLng) {
                await activateDriverImmediately(user.uid, userLatLng);
            }

            notificationManager.show(
                'تم التسجيل بنجاح!', 
                'مرحباً ' + formData.name + '! تم إنشاء حساب السائق بنجاح.', 
                'success'
            );

            if (map) {
                setTimeout(() => {
                    loadActiveUsersOnMap();
                }, 2000);
            }

        } catch (error) {
            console.error('خطأ في تسجيل السائق:', error);
            
            let errorMessage = 'فشل إنشاء الحساب';
            if (error.code === 'auth/email-already-in-use') {
                errorMessage = 'هذا البريد الإلكتروني مستخدم بالفعل';
            } else if (error.code === 'auth/weak-password') {
                errorMessage = 'كلمة المرور ضعيفة جداً';
            } else if (error.code === 'auth/invalid-email') {
                errorMessage = 'البريد الإلكتروني غير صالح';
            } else if (error.message) {
                errorMessage = error.message;
            }
            
            notificationManager.show('خطأ في التسجيل', errorMessage, 'error');
        } finally {
            btn.disabled = false;
            btn.innerHTML = originalText;
        }
    }

    async function registerUser() {
        const btn = document.getElementById('submitUserRegister');
        const originalText = btn.innerHTML;
        
        try {
            const formData = {
                name: document.getElementById('regUserName').value.trim(),
                email: document.getElementById('regUserEmail').value.trim(),
                password: document.getElementById('regUserPassword').value
            };

            const validationError = validateUserRegistration(formData);
            if (validationError) {
                throw new Error(validationError);
            }

            btn.disabled = true;
            btn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> جاري إنشاء الحساب...';

            const userCredential = await auth.createUserWithEmailAndPassword(
                formData.email, 
                formData.password
            );
            const user = userCredential.user;

            const userData = {
                uid: user.uid,
                name: formData.name,
                email: formData.email,
                role: 'user',
                privacySettings: privacyManager.settings,
                createdAt: firebase.firestore.FieldValue.serverTimestamp(),
                lastSeen: firebase.firestore.FieldValue.serverTimestamp()
            };

            await db.collection('users').doc(user.uid).set(userData);

            document.getElementById('registerUserModal').classList.remove('open');
            document.getElementById('overlay').classList.remove('active');

            notificationManager.show(
                'تم التسجيل بنجاح!', 
                'مرحباً ' + formData.name + '! تم إنشاء حساب الزبون بنجاح.', 
                'success'
            );

        } catch (error) {
            console.error('خطأ في تسجيل الزبون:', error);
            
            let errorMessage = 'فشل إنشاء الحساب';
            if (error.code === 'auth/email-already-in-use') {
                errorMessage = 'هذا البريد الإلكتروني مستخدم بالفعل';
            } else if (error.code === 'auth/weak-password') {
                errorMessage = 'كلمة المرور ضعيفة جداً';
            } else if (error.code === 'auth/invalid-email') {
                errorMessage = 'البريد الإلكتروني غير صالح';
            } else if (error.message) {
                errorMessage = error.message;
            }
            
            notificationManager.show('خطأ في التسجيل', errorMessage, 'error');
        } finally {
            btn.disabled = false;
            btn.innerHTML = originalText;
        }
    }

    async function activateDriverImmediately(uid, initialLocation = null) {
        try {
            const loc = initialLocation || userLatLng || { latitude: 18.0859, longitude: -15.9707 };
            await db.collection('users').doc(uid).update({
                isOnline: true,
                location: {
                    latitude: loc.latitude,
                    longitude: loc.longitude,
                    timestamp: firebase.firestore.FieldValue.serverTimestamp()
                }
            });
        } catch (error) {
            console.error('فشل التفعيل الفوري:', error);
        }
    }

    // ==================== إعدادات التحقق الفوري ====================
    function addRealTimeValidation() {
        const driverFields = ['regDriverName', 'regDriverEmail', 'regDriverPassword', 'regDriverIdCard', 'regDriverPhone'];
        driverFields.forEach(fieldId => {
            const field = document.getElementById(fieldId);
            if (field) {
                field.addEventListener('blur', function() {
                    validateField(fieldId, 'driver');
                });
            }
        });

        const userFields = ['regUserName', 'regUserEmail', 'regUserPassword'];
        userFields.forEach(fieldId => {
            const field = document.getElementById(fieldId);
            if (field) {
                field.addEventListener('blur', function() {
                    validateField(fieldId, 'user');
                });
            }
        });
    }

    function validateField(fieldId, userType) {
        const field = document.getElementById(fieldId);
        const value = field.value.trim();
        let isValid = true;
        let errorMessage = '';

        switch(fieldId) {
            case 'regDriverName':
            case 'regUserName':
                if (value.length < 2) {
                    isValid = false;
                    errorMessage = 'الاسم يجب أن يكون حرفين على الأقل';
                }
                break;
                
            case 'regDriverEmail':
            case 'regUserEmail':
                const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
                if (!emailRegex.test(value)) {
                    isValid = false;
                    errorMessage = 'بريد إلكتروني غير صالح';
                }
                break;
                
            case 'regDriverPassword':
            case 'regUserPassword':
                if (value.length < 6) {
                    isValid = false;
                    errorMessage = 'كلمة المرور يجب أن تكون 6 أحرف على الأقل';
                }
                break;
                
            case 'regDriverIdCard':
                if (value.length < 4) {
                    isValid = false;
                    errorMessage = 'رقم البطاقة يجب أن يكون 4 أحرف على الأقل';
                }
                break;
                
            case 'regDriverPhone':
                const phoneRegex = /^[\d\s\-\+]{8,15}$/;
                if (!phoneRegex.test(value)) {
                    isValid = false;
                    errorMessage = 'رقم هاتف غير صالح';
                }
                break;
        }

        if (isValid) {
            field.style.borderColor = '#4CAF50';
            field.style.boxShadow = '0 0 0 2px rgba(76, 175, 80, 0.2)';
            removeFieldError(fieldId);
        } else {
            field.style.borderColor = '#f44336';
            field.style.boxShadow = '0 0 0 2px rgba(244, 67, 54, 0.2)';
            showFieldError(fieldId, errorMessage);
        }
    }

    function showFieldError(fieldId, message) {
        removeFieldError(fieldId);
        
        const field = document.getElementById(fieldId);
        const errorDiv = document.createElement('div');
        errorDiv.className = 'field-error';
        errorDiv.id = fieldId + '-error';
        errorDiv.innerHTML = `<small style="color: #f44336; font-size: 12px; margin-top: 5px; display: block;">${message}</small>`;
        
        field.parentNode.appendChild(errorDiv);
    }

    function removeFieldError(fieldId) {
        const existingError = document.getElementById(fieldId + '-error');
        if (existingError) {
            existingError.remove();
        }
    }

    // ==================== تهيئة أزرار التسجيل ====================
    function initializeRegistrationEventListeners() {
        console.log('تهيئة أزرار التسجيل...');
        
        const registerDriverBtn = document.getElementById('registerDriverBtn');
        if (registerDriverBtn) {
            registerDriverBtn.addEventListener('click', function(e) {
                e.preventDefault();
                console.log('فتح نافذة تسجيل السائق');
                document.getElementById('registerDriverModal').classList.add('open');
                document.getElementById('overlay').classList.add('active');
                
                setTimeout(() => {
                    document.getElementById('regDriverName').focus();
                }, 300);
            });
        }

        const registerUserBtn = document.getElementById('registerUserBtn');
        if (registerUserBtn) {
            registerUserBtn.addEventListener('click', function(e) {
                e.preventDefault();
                console.log('فتح نافذة تسجيل الزبون');
                document.getElementById('registerUserModal').classList.add('open');
                document.getElementById('overlay').classList.add('active');
                
                setTimeout(() => {
                    document.getElementById('regUserName').focus();
                }, 300);
            });
        }

        const submitDriverBtn = document.getElementById('submitDriverRegister');
        if (submitDriverBtn) {
            submitDriverBtn.addEventListener('click', function(e) {
                e.preventDefault();
                console.log('محاولة تسجيل سائق جديد');
                registerDriver();
            });
        }

        const submitUserBtn = document.getElementById('submitUserRegister');
        if (submitUserBtn) {
            submitUserBtn.addEventListener('click', function(e) {
                e.preventDefault();
                console.log('محاولة تسجيل زبون جديد');
                registerUser();
            });
        }

        const closeDriverModal = document.getElementById('closeRegisterDriverModal');
        if (closeDriverModal) {
            closeDriverModal.addEventListener('click', function() {
                document.getElementById('registerDriverModal').classList.remove('open');
                document.getElementById('overlay').classList.remove('active');
            });
        }

        const closeUserModal = document.getElementById('closeRegisterUserModal');
        if (closeUserModal) {
            closeUserModal.addEventListener('click', function() {
                document.getElementById('registerUserModal').classList.remove('open');
                document.getElementById('overlay').classList.remove('active');
            });
        }

        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                document.getElementById('registerDriverModal').classList.remove('open');
                document.getElementById('registerUserModal').classList.remove('open');
                document.getElementById('overlay').classList.remove('active');
            }
        });

        addRealTimeValidation();
    }

    // ==================== تهيئة زر تفعيل الموقع ====================
    function initializeLocationButton() {
        const allowBtn = document.getElementById('allowBtn');
        if (allowBtn) {
            allowBtn.addEventListener('click', async function() {
                const btn = this;
                const originalHTML = btn.innerHTML;
                
                btn.disabled = true;
                btn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> جاري تفعيل الموقع...';

                try {
                    await enableLocationAndInitMap();
                    notificationManager.show('تم التفعيل', 'تم تفعيل الموقع بنجاح', 'success');
                } catch (error) {
                    console.error('خطأ في تفعيل الموقع:', error);
                    notificationManager.show('خطأ', error.message, 'error');
                    
                    btn.disabled = false;
                    btn.innerHTML = originalHTML;
                }
            });
        }
    }

    // ==================== تهيئة زر طلب التاكسي ====================
    function initializeRequestButton() {
        const requestBtn = document.getElementById('requestBtn');
        if (requestBtn) {
            requestBtn.addEventListener('click', async function() {
                if (!isLocationEnabled) {
                    notificationManager.show('خطأ', 'يجب تفعيل الموقع أولاً لطلب التاكسي', 'error');
                    return;
                }

                if (!map) {
                    try {
                        await enableLocationAndInitMap();
                    } catch (error) {
                        return notificationManager.show('خطأ', 'يجب تفعيل الموقع أولاً', 'error');
                    }
                } else {
                    setTimeout(() => { if (map) map.invalidateSize(); }, 100);
                }
                
                notificationManager.show('طلب تاكسي', 'جارٍ البحث عن أقرب سائق...', 'info');
                
                setTimeout(() => {
                    const drivers = Array.from(userMarkers.values()).filter(marker => {
                        return marker.options.icon?.options?.className?.includes('driver-marker');
                    });
                    
                    if (drivers.length > 0) {
                        notificationManager.show('تم العثور', `عثرنا على ${drivers.length} سائق قريب`, 'success');
                    } else {
                        notificationManager.show('لا سائقين', 'لا توجد سائقين متاحين حالياً', 'warning');
                    }
                }, 2000);
            });
        }
    }

    // ==================== تهيئة معالجات الأحداث الرئيسية ====================
    function initializeEventListeners() {
        console.log('تهيئة معالجات الأحداث الرئيسية...');
        
        // زر القائمة الرئيسية
        const menuToggle = document.getElementById('menuToggle');
        const sidebar = document.getElementById('sidebar');
        const overlay = document.getElementById('overlay');

        if (menuToggle && sidebar && overlay) {
            menuToggle.addEventListener('click', function(e) {
                e.preventDefault();
                e.stopPropagation();
                console.log('النقر على زر القائمة');
                sidebar.classList.toggle('open');
                overlay.classList.toggle('active');
                
                document.getElementById('userInfoCard').style.display = 'none';
            });
        }

        // النقر على الـ overlay لإغلاق القائمة
        if (overlay) {
            overlay.addEventListener('click', function(e) {
                e.preventDefault();
                console.log('النقر على الـ overlay');
                sidebar.classList.remove('open');
                overlay.classList.remove('active');
                document.getElementById('userInfoCard').style.display = 'none';
                
                document.getElementById('registerDriverModal').classList.remove('open');
                document.getElementById('registerUserModal').classList.remove('open');
            });
        }

        // زر تسجيل الدخول
        const loginBtn = document.getElementById('loginBtn');
        if (loginBtn) {
            loginBtn.addEventListener('click', async function(e) {
                e.preventDefault();
                const email = document.getElementById('email').value.trim();
                const password = document.getElementById('password').value;
                
                if (!email || !password) {
                    return notificationManager.show('خطأ', 'أدخل البريد وكلمة المرور', 'error');
                }
                
                loadingManager.show('جاري تسجيل الدخول...');
                
                try {
                    await auth.signInWithEmailAndPassword(email, password);
                    notificationManager.show('مرحباً', 'تم تسجيل الدخول بنجاح', 'success');
                    
                    sidebar.classList.remove('open');
                    overlay.classList.remove('active');
                } catch (error) {
                    let msg = 'فشل الدخول';
                    if (error.code === 'auth/user-not-found') msg = 'الحساب غير موجود';
                    else if (error.code === 'auth/wrong-password') msg = 'كلمة المرور خاطئة';
                    else if (error.code === 'auth/too-many-requests') msg = 'محاولات كثيرة، حاول لاحقاً';
                    else if (error.code === 'auth/invalid-email') msg = 'البريد الإلكتروني غير صالح';
                    notificationManager.show('خطأ', msg, 'error');
                } finally {
                    loadingManager.hide();
                }
            });
        }

        // زر حفظ الإعدادات
        const saveSettingsBtn = document.getElementById('saveSettingsBtn');
        if (saveSettingsBtn) {
            saveSettingsBtn.addEventListener('click', function() {
                privacyManager.saveSettings();
            });
        }

        // زر حفظ الملف الشخصي
        const saveProfileBtn = document.getElementById('saveProfileBtn');
        if (saveProfileBtn) {
            saveProfileBtn.addEventListener('click', async function() {
                const user = auth.currentUser;
                if (!user) return;

                const name = document.getElementById('profileName').value.trim();
                const idCard = document.getElementById('profileIdCard').value.trim();
                const phone = document.getElementById('profilePhone').value.trim();

                if (!name) {
                    return notificationManager.show('خطأ', 'الاسم مطلوب', 'error');
                }

                loadingManager.show('جاري حفظ المعلومات...');

                try {
                    const updateData = { name };
                    
                    if (currentUserRole === 'driver') {
                        if (!idCard) {
                            loadingManager.hide();
                            return notificationManager.show('خطأ', 'رقم البطاقة مطلوب', 'error');
                        }
                        if (!phone) {
                            loadingManager.hide();
                            return notificationManager.show('خطأ', 'رقم الهاتف مطلوب', 'error');
                        }
                        updateData.idCard = idCard;
                        updateData.phone = phone;
                    }

                    await db.collection('users').doc(user.uid).update(updateData);
                    notificationManager.show('تم الحفظ', 'تم تحديث المعلومات بنجاح', 'success');
                } catch (error) {
                    notificationManager.show('خطأ', 'فشل حفظ المعلومات', 'error');
                } finally {
                    loadingManager.hide();
                }
            });
        }

        // زر تفعيل التتبع للسائقين
        const startTrackingBtn = document.getElementById('startTrackingBtn');
        if (startTrackingBtn) {
            startTrackingBtn.addEventListener('click', async function() {
                const user = auth.currentUser;
                if (!user) return notificationManager.show('خطأ', 'يجب تسجيل الدخول أولاً', 'error');
                
                loadingManager.show('جاري التفعيل...');
                
                try {
                    const userData = await checkUserPermission('driver');
                    
                    await db.collection('users').doc(user.uid).update({ 
                        isOnline: true,
                        lastSeen: firebase.firestore.FieldValue.serverTimestamp()
                    });
                    
                    const btn = document.getElementById('startTrackingBtn');
                    btn.textContent = '📍 التحديث مفعل';
                    btn.style.background = '#4CAF50';
                    btn.disabled = true;
                    
                    notificationManager.show('تم التفعيل', 'تم تفعيل تحديث الموقع - أنت الآن ظاهر للزبائن', 'success');
                } catch (error) {
                    notificationManager.show('خطأ', error.message, 'error');
                } finally {
                    loadingManager.hide();
                }
            });
        }

        // إغلاق النوافذ بالضغط على ESC
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                sidebar.classList.remove('open');
                overlay.classList.remove('active');
                document.getElementById('registerDriverModal').classList.remove('open');
                document.getElementById('registerUserModal').classList.remove('open');
                document.getElementById('chatModal').classList.remove('open');
                document.getElementById('userInfoCard').style.display = 'none';
            }
        });

        // منع إغلاق القائمة عند النقر داخلها
        if (sidebar) {
            sidebar.addEventListener('click', function(e) {
                e.stopPropagation();
            });
        }

        // إعدادات الدردشة
        document.getElementById('sendMessageBtn').addEventListener('click', sendMessage);
        
        const messageInput = document.getElementById('messageInput');
        messageInput.addEventListener('keypress', (e) => {
            if (e.key === 'Enter' && !e.shiftKey) { 
                e.preventDefault(); 
                sendMessage(); 
            }
        });

        messageInput.addEventListener('input', debounce(() => {
            if (currentChatRoom && messageInput.value.trim()) {
                chatManager.typingIndicator(currentChatRoom, true);
                
                clearTimeout(typingTimeout);
                typingTimeout = setTimeout(() => {
                    chatManager.typingIndicator(currentChatRoom, false);
                }, 3000);
            }
        }, 500));

        messageInput.addEventListener('blur', () => {
            if (currentChatRoom) {
                chatManager.typingIndicator(currentChatRoom, false);
            }
        });
        
        document.getElementById('closeChat').addEventListener('click', () => {
            document.getElementById('chatModal').classList.remove('open');
            if (chatUnsubscribe) chatUnsubscribe();
            chatUnsubscribe = null; 
            currentChatRoom = null; 
            currentChatPartner = null;
            if (typingTimeout) clearTimeout(typingTimeout);
        });
        
        document.getElementById('chatToggleBtn').addEventListener('click', () => {
            if (currentChatPartner) {
                openChatWithUser(currentChatPartner);
            } else {
                notificationManager.show('فتح الدردشة', 'افتح دردشة من القائمة أو الخريطة', 'info');
            }
        });

        // زر تسجيل الخروج
        const logoutBtn = document.getElementById('logoutBtn');
        if (logoutBtn) {
            logoutBtn.addEventListener('click', async function() {
                try {
                    loadingManager.show('جاري تسجيل الخروج...');
                    
                    if (trackingInterval) {
                        navigator.geolocation.clearWatch(trackingInterval);
                        trackingInterval = null;
                    }
                    
                    const user = auth.currentUser;
                    if (user) {
                        const userDoc = await db.collection('users').doc(user.uid).get();
                        if (userDoc.exists && userDoc.data().role === 'driver') {
                            await db.collection('users').doc(user.uid).update({ 
                                isOnline: false,
                                lastSeen: firebase.firestore.FieldValue.serverTimestamp()
                            });
                        }
                    }
                    
                    await auth.signOut();
                    notificationManager.show('تم الخروج', 'تم تسجيل الخروج بنجاح', 'success');
                } catch (error) {
                    notificationManager.show('خطأ', 'حدث خطأ أثناء تسجيل الخروج', 'error');
                } finally {
                    loadingManager.hide();
                }
            });
        }

        console.log('✅ تم تهيئة جميع معالجات الأحداث');
    }

    // ==================== دوال إضافية ====================
    function addPullToRefresh() {
        let startY = 0;
        
        document.addEventListener('touchstart', e => {
            if (window.scrollY === 0) {
                startY = e.touches[0].clientY;
            }
        });
        
        document.addEventListener('touchmove', e => {
            if (window.scrollY === 0 && e.touches[0].clientY - startY > 100) {
                loadActiveUsersOnMap();
                startY = e.touches[0].clientY;
            }
        });
    }

    function optimizePerformance() {
        if (map) {
            map.options.preferCanvas = true;
        }
    }

    // ==================== التهيئة الرئيسية ====================
    document.addEventListener('DOMContentLoaded', function() {
        console.log('🚖 تهيئة تطبيق تاكسي نواكشوط...');
        
        initializeRegistrationEventListeners();
        initializeLocationButton();
        initializeRequestButton();
        initializeEventListeners();
        
        if ('serviceWorker' in navigator) {
            navigator.serviceWorker.register('/sw.js')
                .then(registration => {
                    console.log('Service Worker مسجل بنجاح');
                })
                .catch(error => {
                    console.log('فشل تسجيل Service Worker:', error);
                });
        }
        
        addPullToRefresh();
        optimizePerformance();

        // مراقبة حالة المصادقة
        auth.onAuthStateChanged(async (user) => {
            const authSec = document.getElementById('authSection');
            const profSec = document.getElementById('userProfileSection');
            const settingsSec = document.getElementById('settingsSection');

            if (user) {
                authSec.style.display = 'none';
                profSec.style.display = 'block';
                settingsSec.style.display = 'block';
                
                try {
                    const userDoc = await db.collection('users').doc(user.uid).get();
                    const userData = userDoc.data();
                    
                    if (!userData) {
                        notificationManager.show('خطأ', 'لم يُعثر على ملفك', 'error');
                        await auth.signOut();
                        return;
                    }
                    
                    updateUIBasedOnRole(userData);
                    privacyManager.init();
                    
                    if (document.getElementById('mapContainer').style.display === 'block') {
                        await loadActiveUsersOnMap();
                    }
                    
                } catch (error) {
                    console.error('خطأ في جلب ملف المستخدم:', error);
                    notificationManager.show('خطأ', 'فشل تحميل ملفك الشخصي', 'error');
                }
            } else {
                authSec.style.display = 'block';
                profSec.style.display = 'none';
                settingsSec.style.display = 'none';
                document.getElementById('chatToggleBtn').style.display = 'none';
                document.getElementById('controlBtns').style.display = 'none';
                
                if (trackingInterval) {
                    navigator.geolocation.clearWatch(trackingInterval);
                    trackingInterval = null;
                }
            }
        });

        // الاستماع للتحديثات في الوقت الحقيقي
        db.collection('users').onSnapshot((snapshot) => {
            if (auth.currentUser && document.getElementById('mapContainer').style.display === 'block') {
                debouncedUpdateMap();
            }
        });

        setTimeout(() => {
            console.log('✅ جميع الأزرار جاهزة للاستخدام');
        }, 1000);

        setTimeout(() => {
            document.body.style.opacity = '1';
        }, 100);
    });

    const debouncedUpdateMap = debounce(() => {
        loadActiveUsersOnMap();
    }, 2000);

  </script>
</body>
</html>

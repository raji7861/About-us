<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Voice AI - دستیار هوشمند صوتی</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;500;600;700&display=swap');
        
        :root {
            --primary: #6D28D9;
            --primary-light: #8B5CF6;
            --primary-dark: #4C1D95;
            --secondary: #F59E0B;
            --accent: #06B6D4;
            --text: #2D3748;
            --light-bg: #F5F3FF;
            --gradient: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
        }
        
        body {
            font-family: 'Noto Naskh Arabic', 'B Nazanin', Arial, sans-serif;
            background-color: #f8f9fa;
            color: var(--text);
            line-height: 1.8;
            margin: 0;
            padding: 0;
            min-height: 100vh;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(109, 40, 217, 0.05) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(6, 182, 212, 0.05) 0%, transparent 20%);
        }
        
        .container {
            max-width: 900px;
            margin: 40px auto;
            padding: 0;
            background-color: white;
            border-radius: 24px;
            box-shadow: 0 25px 50px rgba(109, 5, 134, 0.1);
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(109, 40, 217, 0.1);
        }
        
        .header {
            background: var(--gradient);
            padding: 40px;
            color: white;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: "";
            position: absolute;
            top: -50px;
            right: -50px;
            width: 200px;
            height: 200px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        .header::after {
            content: "";
            position: absolute;
            bottom: -80px;
            left: -80px;
            width: 200px;
            height: 200px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        .logo {
            font-size: 42px;
            font-weight: bold;
            color: white;
            margin-bottom: 15px;
            position: relative;
            z-index: 2;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }
        
        .tagline {
            font-size: 18px;
            opacity: 0.9;
            position: relative;
            z-index: 2;
            margin-bottom: 10px;
        }
        
        .content {
            padding: 40px;
        }
        
        h1 {
            color: var(--primary);
            text-align: center;
            font-size: 32px;
            margin: 0 0 30px 0;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--light-bg);
            font-weight: 700;
            position: relative;
        }
        
        h1::after {
            content: "";
            position: absolute;
            bottom: -2px;
            right: 0;
            width: 150px;
            height: 3px;
            background: var(--secondary);
        }
        
        p {
            font-size: 18px;
            margin-bottom: 25px;
            text-align: justify;
            line-height: 2;
        }
        
        .highlight {
            background-color: var(--light-bg);
            padding: 25px;
            border-radius: 15px;
            margin: 30px 0;
            border-right: 4px solid var(--primary);
            font-size: 18px;
            position: relative;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .highlight:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        .highlight::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 60px;
            height: 60px;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="%236D28D9" opacity="0.1"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/></svg>') no-repeat;
            background-size: contain;
        }
        
        .features {
            margin: 35px 0;
            position: relative;
        }
        
        .features::before {
            content: "ویژگی‌های کلیدی";
            display: block;
            font-size: 24px;
            color: var(--primary);
            margin-bottom: 20px;
            font-weight: 600;
            padding-right: 15px;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .feature-card {
            background: white;
            border-radius: 12px;
            padding: 25px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border: 1px solid rgba(109, 40, 217, 0.1);
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        .feature-card::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 4px;
            background: var(--gradient);
        }
        
        .feature-icon {
            font-size: 32px;
            color: var(--primary);
            margin-bottom: 15px;
            display: inline-block;
        }
        
        .feature-title {
            font-weight: 600;
            font-size: 18px;
            margin-bottom: 10px;
            color: var(--primary-dark);
        }
        
        .feature-desc {
            font-size: 16px;
            color: var(--text);
            line-height: 1.8;
        }
        
        .contact {
            background: var(--gradient);
            color: white;
            padding: 30px;
            border-radius: 15px;
            margin-top: 40px;
            text-align: center;
            font-size: 18px;
            box-shadow: 0 10px 30px rgba(109, 40, 217, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .contact::before {
            content: "";
            position: absolute;
            top: -20px;
            right: -20px;
            width: 100px;
            height: 100px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        .contact h2 {
            color: white;
            margin-top: 0;
            font-size: 24px;
            margin-bottom: 20px;
            position: relative;
            z-index: 2;
        }
        
        .contact-links {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            position: relative;
            z-index: 2;
        }
        
        .contact-link {
            color: white;
            text-decoration: none;
            font-weight: 600;
            font-size: 18px;
            padding: 12px 25px;
            border-radius: 8px;
            background-color: rgba(255, 255, 255, 0.15);
            transition: all 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }
        
        .contact-link:hover {
            background-color: rgba(255, 255, 255, 0.25);
            transform: translateY(-3px);
        }
        
        .footer {
            text-align: center;
            margin-top: 40px;
            font-size: 16px;
            color: var(--primary);
            font-weight: 600;
            position: relative;
            padding-top: 20px;
        }
        
        .footer::before {
            content: "";
            position: absolute;
            top: 0;
            right: calc(50% - 50px);
            width: 100px;
            height: 3px;
            background: var(--gradient);
        }
        
        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent 0%, var(--primary) 50%, transparent 100%);
            margin: 40px 0;
            border: none;
        }
        
        .multi-purpose {
            background-color: #FEF3C7;
            padding: 25px;
            border-radius: 15px;
            margin: 30px 0;
            border-right: 4px solid var(--secondary);
            font-size: 18px;
            position: relative;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .multi-purpose::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 60px;
            height: 60px;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="%23F59E0B" opacity="0.1"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8zm-1-13h2v6h-2zm0 8h2v2h-2z"/></svg>') no-repeat;
            background-size: contain;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 0;
                margin: 20px 15px;
                border-radius: 16px;
            }
            
            .header, .content {
                padding: 30px 20px;
            }
            
            h1 {
                font-size: 28px;
            }
            
            .logo {
                font-size: 36px;
            }
            
            .contact-links {
                flex-direction: column;
            }
            
            .contact-link {
                justify-content: center;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo">VOICE AI</div>
            <div class="tagline">دستیار هوشمند تبدیل متن به گفتار با فناوری پیشرفته</div>
        </div>
        
        <div class="content">
            <h1>درباره ما</h1>
            
            <div class="highlight">
                <p>دستیار هوشمند صوتی (Voice AI) نرم‌افزاری کاربردی است که با بهره‌گیری از فناوری‌های پیشرفته، امکان تبدیل متن به گفتار طبیعی و استخراج متن از تصاویر را فراهم می‌کند. این برنامه با طراحی رابط کاربری بصری و امکاناتی نظیر اعمال تنظیمات بر صدای خروجی، تجربه‌ای بهینه و منعطف را در بهره‌گیری از فناوری صوتی برای کاربران فراهم می‌سازد.</p>
            </div>
            
            <div class="divider"></div>
            
            <div class="features">
                <div class="features-grid">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-microphone-alt"></i>
                        </div>
                        <h3 class="feature-title">تبدیل متن به گفتار طبیعی</h3>
                        <p class="feature-desc">تبدیل متن به گفتار با صدای طبیعی با استفاده از فناوری TTS پیشرفته</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-camera"></i>
                        </div>
                        <h3 class="feature-title">شناسایی متن از تصویر</h3>
                        <p class="feature-desc">استخراج متن از تصاویر با دقت بالا با استفاده از فناوری OCR پیشرفته</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-language"></i>
                        </div>
                        <h3 class="feature-title">پشتیبانی چندزبانه</h3>
                        <p class="feature-desc">پشتیبانی کامل از زبان‌های فارسی و انگلیسی با تلفظ طبیعی</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-sliders-h"></i>
                        </div>
                        <h3 class="feature-title">تنظیمات پیشرفته صدا</h3>
                        <p class="feature-desc">امکان تنظیم سرعت، تاخیر بین هر کلمه و سایر پارامترهای خروجی صوتی</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-user-friends"></i>
                        </div>
                        <h3 class="feature-title">رابط کاربری ساده</h3>
                        <p class="feature-desc">رابط کاربری زیبا و کاملاً فارسی‌سازی شده برای تجربه کاربری بهتر</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-file-audio"></i>
                        </div>
                        <h3 class="feature-title">ذخیره فایل صوتی</h3>
                        <p class="feature-desc">ذخیره‌سازی خروجی صوتی با فرمت MP3 با کیفیت بالا</p>
                    </div>
                </div>
            </div>
            
            <div class="multi-purpose">
                <p>🔸 Voice AI تنها یک ابزار تبدیل متن به گفتار نیست، بلکه یک دستیار هوشمند و چندمنظوره است که در زمینه‌های متنوعی مانند آموزش، یادگیری، ارتباطات، تولید محتوا، تقویت مهارت‌های زبانی و بسیاری کاربردهای دیگر، بسته به خلاقیت و نیاز کاربر، قابل استفاده است.</p>
            </div>
            
            <div class="contact">
                <h2>راه‌های ارتباط با ما</h2>
                <div class="contact-links">
                    <a href="mailto:raji.tech.ai.101@gmail.com" class="contact-link">
                        <i class="fas fa-envelope"></i>
                        ایمیل: raji.tech.ai.101@gmail.com
                    </a>
                    <a href="tel:+989183094275" class="contact-link">
                        <i class="fas fa-phone"></i>
                        تلفن: 09183094275
                    </a>
                </div>
            </div>
            
            <div class="footer">
                طراح:محمدرضا راجی
            </div>
        </div>
    </div>
</body>
</html>

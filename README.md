<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>شهرستان دورود - قلب لرستان</title>
    <meta name="description" content="شهرستان دورود در قلب لرستان - مرکز گردشگری، فرهنگ و تاریخ">
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/sahel-font@v3.4.0/dist/font-face.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Vazirmatn', 'Sahel', 'Inter', 'Tahoma', sans-serif;
            background: #f5f5f5;
            overflow-x: hidden;
            line-height: 1.7;
            box-sizing: border-box;
            font-feature-settings: "kern" 1, "liga" 1;
            text-rendering: optimizeLegibility;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            font-weight: 400;
        }

        /* Animated Background */
        .animated-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: linear-gradient(-45deg, #f5f5f5, #e8e8e8, #f0f0f0, #eeeeee);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Glass Effect Widgets */
        .glass-widget {
            background: rgba(255, 255, 255, 0.25);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 30px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.23, 1, 0.320, 1);
        }

        .glass-widget::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            transition: left 0.8s ease;
        }

        .glass-widget:hover::before {
            left: 100%;
        }

        .glass-widget:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        }

        /* Navigation */
        .navbar {
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            padding: 1rem 2rem;
            transition: all 0.4s ease;
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(25px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .navbar.scrolled {
            background: rgba(255, 255, 255, 0.25);
            backdrop-filter: blur(30px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1400px;
            margin: 0 auto;
        }

        .logo {
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            font-size: 2rem;
            font-weight: 800;
            color: #333;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            cursor: pointer;
            transition: all 0.3s ease;
            letter-spacing: -0.5px;
        }

        .logo:hover {
            transform: scale(1.05);
            color: #555;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 0.5rem;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 30px;
            padding: 0.5rem;
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .nav-item a {
            color: #333;
            text-decoration: none;
            font-weight: 600;
            padding: 0.8rem 1.5rem;
            border-radius: 25px;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            white-space: nowrap;
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            letter-spacing: -0.2px;
        }

        .nav-item a:hover,
        .nav-item.active a {
            background: rgba(255, 255, 255, 0.4);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .mobile-menu-btn {
            display: none;
            background: rgba(255, 255, 255, 0.3);
            border: none;
            color: #333;
            padding: 0.8rem;
            border-radius: 15px;
            cursor: pointer;
            backdrop-filter: blur(20px);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
            padding: 0 2rem;
        }

        .hero-content {
            max-width: 800px;
            color: #333;
            z-index: 2;
        }

        .hero h1 {
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            font-size: 4rem;
            font-weight: 900;
            margin-bottom: 1.5rem;
            animation: fadeInUp 1s ease-out;
            background: linear-gradient(45deg, #333, #666, #999);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            letter-spacing: -1px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.8;
            animation: fadeInUp 1s ease-out 0.3s both;
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .cta-button {
            display: inline-block;
            padding: 1rem 2rem;
            background: rgba(255, 255, 255, 0.3);
            color: #333;
            text-decoration: none;
            border-radius: 30px;
            font-weight: 600;
            transition: all 0.3s ease;
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.4);
            animation: fadeInUp 1s ease-out 0.6s both;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            background: rgba(255, 255, 255, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        /* Floating Elements */
        .floating-element {
            position: absolute;
            opacity: 0.1;
            pointer-events: none;
            animation: float 6s ease-in-out infinite;
        }

        .floating-element:nth-child(1) { top: 20%; left: 10%; animation-delay: 0s; }
        .floating-element:nth-child(2) { top: 60%; right: 15%; animation-delay: -2s; }
        .floating-element:nth-child(3) { bottom: 30%; left: 20%; animation-delay: -4s; }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(5deg); }
        }

        /* Main Content */
        .main-content {
            padding: 4rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .page {
            display: none;
            min-height: 100vh;
            padding-top: 100px;
        }

        .page.active {
            display: block;
            animation: pageSlideIn 0.6s ease-out;
        }

        @keyframes pageSlideIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .section-title {
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            text-align: center;
            font-size: 2.5rem;
            font-weight: 800;
            color: #333;
            margin-bottom: 3rem;
            position: relative;
            letter-spacing: -0.5px;
            text-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: linear-gradient(45deg, #666, #999);
            border-radius: 2px;
        }

        /* Grid Layouts */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }

        .card {
            padding: 2rem;
            text-align: center;
            color: #333;
            min-height: 350px;
            display: flex;
            flex-direction: column;
            align-items: center;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .card::after {
            content: '🔍 کلیک برای اطلاعات بیشتر';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(135deg, rgba(100, 150, 255, 0.9), rgba(150, 100, 255, 0.9));
            color: white;
            padding: 0.8rem;
            transform: translateY(100%);
            transition: transform 0.3s ease;
            font-size: 0.85rem;
            font-weight: 600;
            backdrop-filter: blur(10px);
        }

        .card:hover::after {
            transform: translateY(0);
        }

        .card-icon {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            display: block;
            animation: iconBounce 2s ease-in-out infinite;
        }

        @keyframes iconBounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }

        .card h3 {
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: #444;
            letter-spacing: -0.3px;
        }

        .card p {
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            opacity: 0.85;
            line-height: 1.7;
            flex: 1;
            font-size: 0.95rem;
            font-weight: 400;
        }



        /* Map Section */
        .map-section {
            margin: 3rem 0;
            padding: 2rem;
            text-align: center;
        }

        .map-container {
            width: 100%;
            height: 400px;
            border-radius: 30px;
            overflow: hidden;
            position: relative;
            cursor: pointer;
            transition: all 0.3s ease;
            background: linear-gradient(135deg, #e8e8e8, #f0f0f0);
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
        }

        .map-container:hover {
            transform: scale(1.02);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .map-placeholder {
            font-size: 4rem;
            margin-bottom: 1rem;
            opacity: 0.6;
        }

        .map-text {
            font-size: 1.2rem;
            color: #666;
            font-weight: 600;
        }

        /* Gallery Grid */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .gallery-item {
            height: 200px;
            border-radius: 30px;
            overflow: hidden;
            position: relative;
            cursor: pointer;
            transition: all 0.4s ease;
            background: linear-gradient(45deg, #e8e8e8, #f0f0f0, #f5f5f5);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            color: #999;
        }

        .gallery-item:hover {
            transform: scale(1.05) rotate(2deg);
        }

        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0,0,0,0.8));
            color: white;
            padding: 0.8rem;
            transform: translateY(100%);
            transition: transform 0.3s ease;
            font-family: 'Vazir', sans-serif;
        }

        .gallery-overlay h4 {
            font-size: 0.9rem;
            font-weight: 600;
            margin: 0 0 0.3rem 0;
            color: white;
        }

        .gallery-overlay p {
            font-size: 0.75rem;
            margin: 0 0 0.5rem 0;
            opacity: 0.9;
            line-height: 1.3;
        }

        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }

        /* Events Timeline */
        .events-timeline {
            position: relative;
            margin: 3rem 0;
            padding: 0 1rem;
        }

        .timeline-line {
            position: absolute;
            left: 50%;
            top: 0;
            bottom: 0;
            width: 3px;
            background: linear-gradient(to bottom, #ddd, #aaa, #ddd);
            transform: translateX(-50%);
            border-radius: 2px;
        }

        .event-item {
            display: flex;
            align-items: center;
            margin-bottom: 3rem;
            position: relative;
            min-height: 120px;
        }

        .event-item:nth-child(even) {
            flex-direction: row-reverse;
        }

        .event-content {
            width: 45%;
            padding: 1.8rem;
            border-radius: 25px;
            position: relative;
            background: rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.4);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .event-content:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.15);
        }

        .event-content h3 {
            font-family: 'Yekan Bakh', 'Estedad', 'Vazir', sans-serif;
            font-size: 1.1rem;
            font-weight: 700;
            color: #333;
            margin-bottom: 0.8rem;
            letter-spacing: -0.2px;
        }

        .event-content p {
            font-family: 'Estedad', 'Yekan Bakh', 'Vazir', sans-serif;
            font-size: 0.9rem;
            line-height: 1.7;
            color: #555;
            text-align: justify;
            font-weight: 400;
        }

        .event-date {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(100, 150, 255, 0.2);
            padding: 0.6rem 1.2rem;
            border-radius: 25px;
            font-weight: 700;
            color: #333;
            backdrop-filter: blur(20px);
            border: 2px solid rgba(100, 150, 255, 0.3);
            font-family: 'Yekan Bakh', 'Estedad', 'Vazir', sans-serif;
            font-size: 0.85rem;
            white-space: nowrap;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            letter-spacing: -0.2px;
        }

        /* Contact Form */
        .contact-form {
            max-width: 600px;
            margin: 2rem auto;
            padding: 2rem;
            border-radius: 30px;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #555;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 1rem;
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(20px);
            color: #333;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: rgba(255, 255, 255, 0.5);
            background: rgba(255, 255, 255, 0.3);
        }

        .submit-btn {
            width: 100%;
            padding: 1rem;
            background: rgba(255, 255, 255, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.4);
            border-radius: 25px;
            color: #333;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(20px);
        }

        .submit-btn:hover {
            background: rgba(255, 255, 255, 0.4);
            transform: translateY(-2px);
        }

        /* Statistics */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin: 3rem 0;
        }

        .stat-item {
            text-align: center;
            padding: 2rem;
            border-radius: 30px;
            color: #333;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: #555;
            display: block;
            margin-bottom: 0.5rem;
            animation: countUp 2s ease-out;
        }

        @keyframes countUp {
            from { opacity: 0; transform: scale(0.5); }
            to { opacity: 1; transform: scale(1); }
        }

        .stat-label {
            font-size: 1rem;
            opacity: 0.8;
        }

        /* Scroll to Top */
        .scroll-to-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 50px;
            height: 50px;
            background: rgba(255, 255, 255, 0.3);
            border: none;
            border-radius: 50%;
            color: #333;
            font-size: 1.2rem;
            cursor: pointer;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.4);
        }

        .scroll-to-top.show {
            opacity: 1;
            visibility: visible;
        }

        .scroll-to-top:hover {
            transform: translateY(-3px);
            background: rgba(255, 255, 255, 0.4);
        }

        /* Font Size Scaling for Better Typography */
        .text-xs { font-size: 0.75rem; font-weight: 400; }
        .text-sm { font-size: 0.875rem; font-weight: 400; }
        .text-base { font-size: 1rem; font-weight: 400; }
        .text-lg { font-size: 1.125rem; font-weight: 500; }
        .text-xl { font-size: 1.25rem; font-weight: 600; }
        .text-2xl { font-size: 1.5rem; font-weight: 700; }
        .text-3xl { font-size: 1.875rem; font-weight: 700; }
        .text-4xl { font-size: 2.25rem; font-weight: 800; }
        .text-5xl { font-size: 3rem; font-weight: 900; }
        .text-6xl { font-size: 3.75rem; font-weight: 900; }

        /* Enhanced Mobile Responsiveness */
        @media (max-width: 768px) {
            .navbar {
                padding: 0.8rem 1rem;
            }

            .nav-container {
                position: relative;
            }

            .logo {
                font-size: 1.5rem;
            }

            .nav-menu {
                display: none;
                position: absolute;
                top: calc(100% + 15px);
                left: 0;
                right: 0;
                background: rgba(255, 255, 255, 0.98);
                backdrop-filter: blur(35px);
                flex-direction: column;
                padding: 1.5rem;
                border-radius: 25px;
                border: 1px solid rgba(255, 255, 255, 0.4);
                box-shadow: 0 20px 40px rgba(0, 0, 0, 0.25);
                z-index: 1001;
                animation: slideDown 0.3s ease-out;
                max-height: 70vh;
                overflow-y: auto;
                overflow-x: hidden;
            }

            /* Custom scrollbar for mobile menu */
            .nav-menu::-webkit-scrollbar {
                width: 6px;
            }

            .nav-menu::-webkit-scrollbar-track {
                background: rgba(255, 255, 255, 0.1);
                border-radius: 10px;
            }

            .nav-menu::-webkit-scrollbar-thumb {
                background: rgba(255, 255, 255, 0.3);
                border-radius: 10px;
            }

            .nav-menu::-webkit-scrollbar-thumb:hover {
                background: rgba(255, 255, 255, 0.5);
            }

            @keyframes slideDown {
                from { opacity: 0; transform: translateY(-10px); }
                to { opacity: 1; transform: translateY(0); }
            }

            .nav-menu.active {
                display: flex;
            }

            .nav-item {
                margin: 0.3rem 0;
            }

            .nav-item a {
                padding: 1rem;
                font-size: 1.1rem;
                justify-content: center;
                border-radius: 20px;
            }

            .mobile-menu-btn {
                display: block;
                font-size: 1.2rem;
                padding: 0.6rem;
            }

            /* Events Timeline Mobile Responsiveness */
            .events-timeline {
                padding: 0 0.5rem;
                margin: 2rem 0;
            }

            .timeline-line {
                left: 20px;
                width: 2px;
            }

            .event-item {
                flex-direction: row !important;
                padding-left: 3.5rem;
                margin-bottom: 2.5rem;
                min-height: auto;
            }

            .event-content {
                width: 100%;
                padding: 1.2rem;
                border-radius: 20px;
            }

            .event-content h3 {
                font-size: 1rem;
                margin-bottom: 0.6rem;
            }

            .event-content p {
                font-size: 0.85rem;
                line-height: 1.5;
            }

            .event-date {
                left: 20px;
                transform: translateX(-50%);
                font-size: 0.75rem;
                padding: 0.4rem 0.8rem;
                border-radius: 20px;
            }

            .hero {
                height: 90vh;
                padding: 0 1rem;
            }

            .hero h1 {
                font-size: 2.2rem;
                line-height: 1.2;
                margin-bottom: 1rem;
            }

            .hero p {
                font-size: 1rem;
                margin-bottom: 1.5rem;
                line-height: 1.5;
            }

            .cta-button {
                padding: 0.8rem 1.5rem;
                font-size: 0.9rem;
            }

            .main-content {
                padding: 2rem 1rem;
            }

            .section-title {
                font-size: 2rem;
                margin-bottom: 2rem;
            }

            .cards-grid {
                grid-template-columns: 1fr;
                gap: 1.2rem;
            }

            .card {
                min-height: 280px;
                padding: 1.5rem;
                text-align: center;
            }

            .card-icon {
                font-size: 2.8rem;
            }

            .card h3 {
                font-size: 1.3rem;
            }

            .card p {
                font-size: 0.95rem;
            }

            .weather-widget {
                position: static;
                width: calc(100% - 2rem);
                margin: 1.5rem 1rem;
                padding: 1.2rem;
            }

            .weather-temp {
                font-size: 1.8rem;
            }

            .weather-details {
                gap: 0.8rem;
            }

            .weather-item {
                padding: 0.8rem 0.5rem;
            }

            .stats-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 1rem;
            }

            .stat-item {
                padding: 1.5rem 1rem;
            }

            .stat-number {
                font-size: 2rem;
            }

            .events-timeline {
                padding: 0 0.5rem;
            }

            .timeline-line {
                left: 20px;
                width: 2px;
            }

            .event-item {
                flex-direction: row !important;
                padding-left: 3.5rem;
                margin-bottom: 2.5rem;
                min-height: auto;
            }

            .event-content {
                width: 100%;
                padding: 1.2rem;
                border-radius: 20px;
            }

            .event-content h3 {
                font-size: 1rem;
                margin-bottom: 0.6rem;
            }

            .event-content p {
                font-size: 0.85rem;
                line-height: 1.5;
            }

            .event-date {
                left: 20px;
                transform: translateX(-50%);
                font-size: 0.75rem;
                padding: 0.4rem 0.8rem;
                border-radius: 20px;
            }

            .gallery-categories {
                gap: 0.5rem;
                margin-bottom: 1.5rem;
            }

            .gallery-cat-btn {
                padding: 0.5rem 1.2rem;
                font-size: 0.8rem;
                border-radius: 40px;
            }

            .gallery-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 1rem;
            }

            .gallery-item {
                height: 150px;
                font-size: 2.5rem;
            }

            .modal-content {
                width: 98%;
                max-height: 95vh;
                border-radius: 20px;
            }

            .modal-header {
                padding: 1rem;
            }

            .modal-header h3 {
                font-size: 1rem;
            }

            .modal-body {
                flex-direction: column;
                padding: 1rem;
                gap: 1rem;
            }

            .modal-image {
                font-size: 4rem;
                min-height: 180px;
                padding: 1.5rem;
            }

            .modal-info {
                padding-right: 0;
            }

            .modal-info p {
                font-size: 0.9rem;
                margin-bottom: 1rem;
            }

            .modal-actions {
                justify-content: center;
            }

            .action-btn {
                font-size: 0.8rem;
                padding: 0.6rem 1rem;
            }

            .contact-form {
                padding: 1.5rem;
                margin: 1.5rem 0;
            }

            .form-group input,
            .form-group textarea,
            .form-group select {
                padding: 0.8rem;
                font-size: 1rem;
            }

            .map-container {
                height: 250px;
            }

            .map-placeholder {
                font-size: 3rem;
            }

            .floating-element {
                display: none;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 1.8rem;
            }

            .hero p {
                font-size: 0.9rem;
            }

            .section-title {
                font-size: 1.6rem;
            }

            .card {
                min-height: 250px;
                padding: 1.2rem;
            }

            .card-icon {
                font-size: 2.5rem;
            }

            .card h3 {
                font-size: 1.2rem;
            }

            .stats-grid {
                grid-template-columns: 1fr;
                gap: 1rem;
            }

            .stat-number {
                font-size: 1.8rem;
            }

            .weather-widget {
                margin: 1rem 0.5rem;
                padding: 1rem;
            }

            .gallery-categories {
                gap: 0.3rem;
                margin-bottom: 1rem;
            }

            .gallery-cat-btn {
                padding: 0.4rem 1rem;
                font-size: 0.75rem;
                border-radius: 35px;
            }

            .gallery-grid {
                grid-template-columns: 1fr;
                gap: 1rem;
            }

            .gallery-item {
                height: 180px;
            }

            .modal-content {
                width: 100%;
                max-height: 98vh;
                border-radius: 15px;
            }

            .modal-header {
                padding: 0.8rem;
            }

            .modal-header h3 {
                font-size: 0.9rem;
            }

            .modal-close {
                width: 30px;
                height: 30px;
                font-size: 1rem;
            }

            .modal-body {
                padding: 0.8rem;
            }

            .modal-image {
                font-size: 3rem;
                min-height: 150px;
                padding: 1rem;
            }

            .modal-info p {
                font-size: 0.85rem;
            }

            .action-btn {
                font-size: 0.75rem;
                padding: 0.5rem 0.8rem;
                margin: 0.1rem;
            }

            /* Enhanced Events Timeline Mobile */
            .events-timeline {
                padding: 0 0.3rem;
                margin: 1.5rem 0;
            }

            .timeline-line {
                left: 15px;
                width: 2px;
            }

            .event-item {
                padding-left: 2.5rem;
                margin-bottom: 2rem;
                min-height: auto;
            }

            .event-content {
                padding: 1rem;
                border-radius: 15px;
                width: 100%;
            }

            .event-content h3 {
                font-size: 0.9rem;
                margin-bottom: 0.5rem;
                line-height: 1.3;
            }

            .event-content p {
                font-size: 0.8rem;
                line-height: 1.4;
                text-align: justify;
            }

            .event-date {
                left: 15px;
                font-size: 0.7rem;
                padding: 0.3rem 0.6rem;
                border-radius: 15px;
                white-space: nowrap;
            }

            .contact-form {
                padding: 1rem;
            }

            .nav-menu {
                left: 0.5rem;
                right: 0.5rem;
                padding: 1rem;
            }

            .dialog-content {
                width: 95%;
                max-height: 90vh;
                border-radius: 20px;
            }

            .dialog-header {
                padding: 1rem 1.5rem;
            }

            .dialog-icon {
                font-size: 2rem;
                margin-left: 0.5rem;
            }

            .dialog-title {
                font-size: 1.2rem;
            }

            .dialog-close {
                width: 35px;
                height: 35px;
                font-size: 1rem;
            }

            .dialog-body {
                padding: 1.5rem;
            }

            .dialog-description {
                font-size: 0.9rem;
                margin-bottom: 1.5rem;
            }

            .dialog-features {
                grid-template-columns: 1fr;
                gap: 0.8rem;
                margin-bottom: 1.5rem;
            }

            .feature-item {
                padding: 0.8rem;
            }

            .feature-icon {
                font-size: 1.3rem;
            }

            .feature-title {
                font-size: 0.85rem;
            }

            .feature-desc {
                font-size: 0.75rem;
            }

            .dialog-actions {
                gap: 0.5rem;
            }

            .dialog-btn {
                padding: 0.6rem 1.2rem;
                font-size: 0.8rem;
            }
        }

        @media (max-width: 360px) {
            .hero h1 {
                font-size: 1.6rem;
            }

            .main-content {
                padding: 1.5rem 0.8rem;
            }

            .card {
                padding: 1rem;
                min-height: 220px;
            }

            .weather-widget {
                margin: 1rem 0.3rem;
            }
        }

        /* Loading Animation */
        .loading {
            display: inline-block;
            width: 20px;
            height: 20px;
            border: 3px solid rgba(0,0,0,.1);
            border-radius: 50%;
            border-top-color: #333;
            animation: spin 1s ease-in-out infinite;
        }

        @keyframes spin {
            to { transform: rotate(360deg); }
        }

        /* Gallery Categories */
        .gallery-categories {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-bottom: 2rem;
            flex-wrap: wrap;
        }

        .gallery-cat-btn {
            background: rgba(255, 255, 255, 0.25);
            border: 1px solid rgba(255, 255, 255, 0.4);
            border-radius: 50px;
            padding: 0.7rem 1.8rem;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(15px);
            color: #333;
            font-weight: 600;
            font-family: 'Yekan Bakh', 'Estedad', 'Vazir', sans-serif;
            font-size: 0.9rem;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            letter-spacing: -0.2px;
        }

        .gallery-cat-btn.active,
        .gallery-cat-btn:hover {
            background: rgba(255, 255, 255, 0.4);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .view-btn {
            background: rgba(255, 255, 255, 0.9);
            border: none;
            border-radius: 15px;
            padding: 0.4rem 0.8rem;
            margin-top: 0.3rem;
            cursor: pointer;
            transition: all 0.3s ease;
            color: #333;
            font-size: 0.7rem;
            font-family: 'Vazir', sans-serif;
            font-weight: 500;
        }

        .view-btn:hover {
            background: rgba(255, 255, 255, 1);
            transform: scale(1.05);
        }

        /* Image Modal */
        .image-modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 2000;
            display: none;
            align-items: center;
            justify-content: center;
            animation: modalFadeIn 0.3s ease-out;
        }

        .image-modal.active {
            display: flex;
        }

        @keyframes modalFadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .modal-content {
            width: 95%;
            max-width: 900px;
            max-height: 90vh;
            overflow-y: auto;
            animation: modalSlideUp 0.4s ease-out;
            border-radius: 25px;
            backdrop-filter: blur(25px);
            background: rgba(255, 255, 255, 0.95);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        @keyframes modalSlideUp {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 1.5rem;
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
            background: rgba(255, 255, 255, 0.1);
            border-radius: 25px 25px 0 0;
        }

        .modal-header h3 {
            margin: 0;
            color: #333;
            font-size: 1.2rem;
            font-family: 'Yekan Bakh', 'Estedad', 'Vazir', sans-serif;
            font-weight: 700;
            letter-spacing: -0.3px;
        }

        .modal-close {
            background: rgba(255, 0, 0, 0.1);
            border: none;
            border-radius: 50%;
            width: 35px;
            height: 35px;
            cursor: pointer;
            color: #d32f2f;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }

        .modal-close:hover {
            background: rgba(255, 0, 0, 0.2);
            transform: scale(1.1);
        }

        .modal-body {
            padding: 1.5rem;
            display: flex;
            gap: 1.5rem;
            align-items: flex-start;
        }

        .modal-image {
            font-size: 6rem;
            text-align: center;
            flex: 1;
            background: rgba(0, 0, 0, 0.05);
            border-radius: 20px;
            padding: 2rem;
            min-height: 250px;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 2px solid rgba(0, 0, 0, 0.1);
        }

        .modal-info {
            flex: 1;
            padding-right: 1rem;
        }

        .modal-info p {
            color: #444;
            line-height: 1.8;
            margin-bottom: 1.5rem;
            font-family: 'Estedad', 'Yekan Bakh', 'Vazir', sans-serif;
            font-size: 0.95rem;
            text-align: justify;
            font-weight: 400;
        }

        .modal-actions {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .action-btn {
            background: rgba(100, 150, 255, 0.1);
            border: 1px solid rgba(100, 150, 255, 0.3);
            border-radius: 25px;
            padding: 0.7rem 1.2rem;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            color: #333;
            font-size: 0.85rem;
            font-family: 'Yekan Bakh', 'Estedad', 'Vazir', sans-serif;
            font-weight: 600;
            margin: 0.2rem;
            letter-spacing: -0.2px;
        }

        .action-btn:hover {
            background: rgba(255, 255, 255, 0.4);
            transform: translateY(-2px);
        }

        /* Chatbot Widget */
        .chatbot-widget {
            position: fixed;
            bottom: 100px;
            right: 20px;
            width: 350px;
            max-height: 500px;
            z-index: 1000;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.23, 1, 0.320, 1);
        }

        .chatbot-header {
            padding: 1rem;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: space-between;
            background: rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(25px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .chatbot-title {
            font-weight: 700;
            color: #333;
            font-size: 0.9rem;
            font-family: 'Yekan Bakh', 'Estedad', sans-serif;
            letter-spacing: -0.2px;
        }

        .chatbot-toggle {
            font-size: 1.2rem;
            transition: transform 0.3s ease;
        }

        .chatbot-body {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease;
        }

        .chatbot-widget.open .chatbot-body {
            max-height: 400px;
        }

        .chatbot-widget.open .chatbot-toggle {
            transform: rotate(180deg);
        }

        .chat-messages {
            height: 250px;
            overflow-y: auto;
            padding: 1rem;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .bot-message, .user-message {
            display: flex;
            align-items: flex-start;
            gap: 0.5rem;
            animation: messageSlide 0.3s ease-out;
        }

        .user-message {
            flex-direction: row-reverse;
        }

        @keyframes messageSlide {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .message-avatar {
            font-size: 1.5rem;
            flex-shrink: 0;
        }

        .message-content {
            background: rgba(255, 255, 255, 0.2);
            padding: 0.8rem;
            border-radius: 15px;
            font-size: 0.9rem;
            line-height: 1.4;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .user-message .message-content {
            background: rgba(100, 150, 255, 0.2);
        }

        .quick-actions {
            display: flex;
            gap: 0.5rem;
            padding: 0 1rem;
            flex-wrap: wrap;
        }

        .quick-btn {
            background: rgba(255, 255, 255, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 20px;
            padding: 0.5rem 0.8rem;
            font-size: 0.8rem;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            color: #333;
        }

        .quick-btn:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-2px);
        }

        .chat-input {
            display: flex;
            padding: 1rem;
            gap: 0.5rem;
        }

        .chat-input input {
            flex: 1;
            padding: 0.8rem;
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            color: #333;
            font-size: 0.9rem;
        }

        .send-btn {
            background: rgba(255, 255, 255, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.4);
            border-radius: 50%;
            width: 40px;
            height: 40px;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .send-btn:hover {
            background: rgba(255, 255, 255, 0.4);
            transform: scale(1.1);
        }

        /* Weather Station */
        .weather-station {
            position: fixed;
            top: 120px;
            left: 20px;
            width: 300px;
            z-index: 999;
            padding: 1.5rem;
            animation: slideInLeft 1s ease-out;
        }

        @keyframes slideInLeft {
            from { transform: translateX(-100%); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }

        .station-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1rem;
        }

        .station-header h4 {
            color: #333;
            font-size: 1rem;
            margin: 0;
        }

        .live-indicator {
            font-size: 0.8rem;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }

        .weather-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 0.8rem;
            margin-bottom: 1rem;
        }

        .weather-card {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.8rem;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .weather-icon {
            font-size: 1.5rem;
        }

        .weather-data {
            display: flex;
            flex-direction: column;
        }

        .weather-value {
            font-weight: 600;
            color: #333;
            font-size: 0.9rem;
        }

        .weather-label {
            font-size: 0.7rem;
            opacity: 0.7;
            color: #555;
        }

        .weather-forecast {
            background: rgba(255, 255, 255, 0.15);
            border-radius: 15px;
            padding: 1rem;
            backdrop-filter: blur(10px);
        }

        .weather-forecast h5 {
            margin: 0 0 0.8rem 0;
            color: #333;
            font-size: 0.9rem;
        }

        .forecast-items {
            display: flex;
            flex-direction: column;
            gap: 0.5rem;
        }

        .forecast-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 0.8rem;
            color: #555;
        }

        /* VR Tour Widget */
        .vr-tour-widget {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80vw;
            max-width: 600px;
            height: 70vh;
            z-index: 1001;
            display: none;
            animation: modalSlideIn 0.4s ease-out;
        }

        .vr-tour-widget.active {
            display: block;
        }

        @keyframes modalSlideIn {
            from { opacity: 0; transform: translate(-50%, -50%) scale(0.8); }
            to { opacity: 1; transform: translate(-50%, -50%) scale(1); }
        }

        .vr-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .vr-header h4 {
            margin: 0;
            color: #333;
        }

        .vr-close {
            background: rgba(255, 255, 255, 0.3);
            border: none;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            cursor: pointer;
            color: #333;
        }

        .vr-content {
            padding: 1rem;
            height: calc(100% - 80px);
            display: flex;
            flex-direction: column;
        }

        .vr-viewer {
            flex: 1;
            background: linear-gradient(135deg, #87CEEB, #98FB98);
            border-radius: 20px;
            position: relative;
            overflow: hidden;
            margin-bottom: 1rem;
        }

        .vr-scene {
            display: none;
            width: 100%;
            height: 100%;
            position: relative;
        }

        .vr-scene.active {
            display: block;
        }

        .vr-panorama {
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 8rem;
            animation: vrRotate 20s linear infinite;
        }

        @keyframes vrRotate {
            from { transform: rotateY(0deg); }
            to { transform: rotateY(360deg); }
        }

        .vr-hotspots {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .hotspot {
            position: absolute;
            width: 30px;
            height: 30px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            animation: hotspotPulse 2s infinite;
        }

        @keyframes hotspotPulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }

        .vr-controls {
            display: flex;
            gap: 0.5rem;
            justify-content: center;
        }

        .vr-btn {
            background: rgba(255, 255, 255, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 20px;
            padding: 0.8rem 1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            color: #333;
            font-size: 0.9rem;
        }

        .vr-btn.active,
        .vr-btn:hover {
            background: rgba(255, 255, 255, 0.4);
            transform: translateY(-2px);
        }

        /* Live Info Widget */
        .live-info-widget {
            position: fixed;
            bottom: 20px;
            left: 20px;
            width: 320px;
            z-index: 999;
            animation: slideInUp 1s ease-out;
        }

        @keyframes slideInUp {
            from { transform: translateY(100%); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        .live-tabs {
            display: flex;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 25px 25px 0 0;
            overflow: hidden;
        }

        .tab-btn {
            flex: 1;
            background: transparent;
            border: none;
            padding: 1rem 0.5rem;
            cursor: pointer;
            transition: all 0.3s ease;
            color: #333;
            font-size: 0.8rem;
        }

        .tab-btn.active,
        .tab-btn:hover {
            background: rgba(255, 255, 255, 0.3);
        }

        .live-content {
            background: rgba(255, 255, 255, 0.25);
            backdrop-filter: blur(20px);
            border-radius: 0 0 25px 25px;
            padding: 1rem;
            max-height: 200px;
            overflow-y: auto;
        }

        .live-tab {
            display: none;
        }

        .live-tab.active {
            display: block;
        }

        .traffic-item,
        .event-item,
        .news-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.8rem 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
            font-size: 0.9rem;
            color: #333;
        }

        .traffic-item:last-child,
        .event-item:last-child,
        .news-item:last-child {
            border-bottom: none;
        }

        .traffic-status {
            font-size: 0.8rem;
        }

        .traffic-time,
        .event-time,
        .news-time {
            font-size: 0.8rem;
            opacity: 0.7;
        }

        /* Audio Player */
        .audio-player {
            position: fixed;
            top: 50%;
            right: 20px;
            transform: translateY(-50%);
            width: 280px;
            z-index: 999;
            animation: slideInRight 1s ease-out;
        }

        .audio-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem;
            cursor: pointer;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .audio-header h4 {
            margin: 0;
            color: #333;
            font-size: 0.9rem;
        }

        .audio-toggle {
            background: rgba(255, 255, 255, 0.3);
            border: none;
            border-radius: 50%;
            width: 35px;
            height: 35px;
            cursor: pointer;
            font-size: 1rem;
        }

        .audio-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease;
        }

        .audio-player.open .audio-content {
            max-height: 300px;
        }

        .audio-track {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0.8rem 1rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }

        .audio-track:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .audio-track.active {
            background: rgba(255, 255, 255, 0.2);
        }

        .track-name {
            font-size: 0.9rem;
            color: #333;
            margin-left: 0.5rem;
        }

        .play-btn {
            background: rgba(255, 255, 255, 0.3);
            border: none;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            cursor: pointer;
            font-size: 0.8rem;
        }

        .audio-controls {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 1rem;
            background: rgba(255, 255, 255, 0.1);
        }

        .volume-slider {
            flex: 1;
            height: 5px;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 5px;
            outline: none;
        }

        /* Card Dialog Modal */
        .card-dialog {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 2000;
            display: none;
            align-items: center;
            justify-content: center;
            animation: modalFadeIn 0.3s ease-out;
            backdrop-filter: blur(5px);
        }

        .card-dialog.active {
            display: flex;
        }

        .dialog-content {
            width: 90%;
            max-width: 600px;
            max-height: 85vh;
            overflow-y: auto;
            animation: dialogSlideUp 0.4s ease-out;
            border-radius: 30px;
            backdrop-filter: blur(25px);
            background: rgba(255, 255, 255, 0.95);
            border: 1px solid rgba(255, 255, 255, 0.3);
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            position: relative;
        }

        @keyframes dialogSlideUp {
            from { transform: translateY(50px) scale(0.9); opacity: 0; }
            to { transform: translateY(0) scale(1); opacity: 1; }
        }

        .dialog-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 2rem;
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
            background: linear-gradient(135deg, rgba(100, 150, 255, 0.1), rgba(150, 100, 255, 0.1));
            border-radius: 30px 30px 0 0;
        }

        .dialog-icon {
            font-size: 2.5rem;
            margin-left: 1rem;
        }

        .dialog-title {
            flex: 1;
            margin: 0;
            color: #333;
            font-size: 1.4rem;
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            font-weight: 700;
            letter-spacing: -0.3px;
        }

        .dialog-close {
            background: rgba(255, 0, 0, 0.1);
            border: none;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            cursor: pointer;
            color: #d32f2f;
            font-size: 1.2rem;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .dialog-close:hover {
            background: rgba(255, 0, 0, 0.2);
            transform: scale(1.1);
        }

        .dialog-body {
            padding: 2rem;
        }

        .dialog-description {
            color: #444;
            line-height: 1.8;
            margin-bottom: 2rem;
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            font-size: 1rem;
            text-align: justify;
            font-weight: 400;
        }

        .dialog-features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .feature-item {
            background: rgba(255, 255, 255, 0.3);
            padding: 1rem;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.4);
            transition: all 0.3s ease;
        }

        .feature-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .feature-icon {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
            display: block;
        }

        .feature-title {
            font-weight: 600;
            color: #333;
            margin-bottom: 0.3rem;
            font-size: 0.9rem;
        }

        .feature-desc {
            font-size: 0.8rem;
            color: #666;
            line-height: 1.4;
        }

        .dialog-actions {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
            justify-content: center;
            padding-top: 1rem;
            border-top: 1px solid rgba(0, 0, 0, 0.1);
        }

        .dialog-btn {
            background: linear-gradient(135deg, rgba(100, 150, 255, 0.2), rgba(150, 100, 255, 0.2));
            border: 1px solid rgba(100, 150, 255, 0.3);
            border-radius: 25px;
            padding: 0.8rem 1.5rem;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            color: #333;
            font-size: 0.9rem;
            font-family: 'Vazirmatn', 'Sahel', 'Inter', sans-serif;
            font-weight: 600;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .dialog-btn:hover {
            background: linear-gradient(135deg, rgba(100, 150, 255, 0.3), rgba(150, 100, 255, 0.3));
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .dialog-btn.primary {
            background: linear-gradient(135deg, rgba(100, 150, 255, 0.8), rgba(150, 100, 255, 0.8));
            color: white;
        }

        .dialog-btn.primary:hover {
            background: linear-gradient(135deg, rgba(100, 150, 255, 0.9), rgba(150, 100, 255, 0.9));
        }

        /* Enhanced Mobile Responsiveness for New Widgets */
        @media (max-width: 768px) {
            #floatingChatbot {
                width: 280px !important;
                right: 10px !important;
                bottom: 70px !important;
            }
            
            .chatbot-header {
                padding: 0.8rem;
            }
            
            .chatbot-title {
                font-size: 0.8rem;
            }
            
            .chat-messages {
                height: 200px;
                padding: 0.8rem;
            }
            
            .message-content {
                padding: 0.6rem;
                font-size: 0.85rem;
            }
            
            .quick-actions {
                padding: 0 0.8rem;
                gap: 0.3rem;
            }
            
            .quick-btn {
                padding: 0.4rem 0.6rem;
                font-size: 0.75rem;
            }
            
            .chat-input {
                padding: 0.8rem;
                gap: 0.3rem;
            }
            
            .chat-input input {
                padding: 0.6rem;
                font-size: 0.85rem;
            }
            
            .send-btn {
                width: 35px;
                height: 35px;
                font-size: 0.8rem;
            }

            .weather-station {
                position: static;
                width: calc(100% - 2rem);
                margin: 1rem;
                order: -1;
            }

            .live-info-widget {
                position: static;
                width: calc(100% - 2rem);
                margin: 1rem;
            }

            .audio-player {
                position: static;
                width: calc(100% - 2rem);
                margin: 1rem;
                transform: none;
            }

            .vr-tour-widget {
                width: 95vw;
                height: 80vh;
            }

            .vr-panorama {
                font-size: 4rem;
            }

            .vr-controls {
                flex-wrap: wrap;
            }

            .vr-btn {
                font-size: 0.8rem;
                padding: 0.6rem 0.8rem;
            }
        }

        @media (max-width: 480px) {
            #floatingChatbot {
                width: 260px !important;
                right: 5px !important;
                bottom: 60px !important;
            }
            
            .chatbot-header {
                padding: 0.6rem;
            }
            
            .chatbot-title {
                font-size: 0.75rem;
            }
            
            .chat-messages {
                height: 180px;
                padding: 0.6rem;
            }
            
            .message-content {
                padding: 0.5rem;
                font-size: 0.8rem;
            }
            
            .quick-btn {
                padding: 0.3rem 0.5rem;
                font-size: 0.7rem;
            }
            
            .chat-input {
                padding: 0.6rem;
            }
            
            .chat-input input {
                padding: 0.5rem;
                font-size: 0.8rem;
            }
            
            .send-btn {
                width: 30px;
                height: 30px;
                font-size: 0.7rem;
            }

            .weather-station,
            .live-info-widget,
            .audio-player {
                width: calc(100% - 1rem);
                margin: 0.5rem;
            }

            .weather-grid {
                grid-template-columns: 1fr;
            }

            .vr-panorama {
                font-size: 3rem;
            }

            .forecast-items {
                gap: 0.3rem;
            }

            .forecast-item {
                font-size: 0.7rem;
            }
        }
    </style>
</head>
<body>
    <div class="animated-bg"></div>

    <!-- Navigation -->
    <nav class="navbar" id="navbar">
        <div class="nav-container">
            <div class="logo" onclick="showPage('home')">
                🏔️ دورود لرستان
            </div>
            <ul class="nav-menu" id="navMenu">
                <li class="nav-item active" id="nav-home">
                    <a href="#" onclick="showPage('home')">🏠 خانه</a>
                </li>
                <li class="nav-item" id="nav-culture">
                    <a href="#" onclick="showPage('culture')">🎭 فرهنگ</a>
                </li>
                <li class="nav-item" id="nav-history">
                    <a href="#" onclick="showPage('history')">📜 تاریخچه</a>
                </li>
                <li class="nav-item" id="nav-tourism">
                    <a href="#" onclick="showPage('tourism')">🗻 گردشگری</a>
                </li>
                <li class="nav-item" id="nav-villages">
                    <a href="#" onclick="showPage('villages')">🏘️ روستاها</a>
                </li>
                <li class="nav-item" id="nav-gallery">
                    <a href="#" onclick="showPage('gallery')">📸 گالری</a>
                </li>
                <li class="nav-item" id="nav-events">
                    <a href="#" onclick="showPage('events')">📅 رویدادها</a>
                </li>
                <li class="nav-item" id="nav-ecotourism">
                    <a href="#" onclick="showPage('ecotourism')">🌿 اکوتوریسم</a>
                </li>
                <li class="nav-item" id="nav-contact">
                    <a href="#" onclick="showPage('contact')">📞 تماس</a>
                </li>
            </ul>
            <button class="mobile-menu-btn" onclick="toggleMobileMenu()">☰</button>
        </div>
    </nav>



    <!-- Home Page -->
    <div id="home" class="page active">
        <section class="hero">
            <div class="floating-element">🏔️</div>
            <div class="floating-element">🌲</div>
            <div class="floating-element">🦅</div>
            
            <div class="hero-content">
                <h1>شهرستان دورود</h1>
                <p>قلب طبیعت لرستان - سرزمین کوه‌های بلند، جنگل‌های سرسبز و چشمه‌های زلال</p>
                <div style="display: flex; gap: 1rem; flex-wrap: wrap; justify-content: center;">
                    <a href="#" class="cta-button" onclick="showPage('tourism')">
                        🌿 کشف جاذبه‌های گردشگری
                    </a>
                    <a href="#" class="cta-button" onclick="openVRTour()">
                        🥽 تور مجازی 360°
                    </a>
                </div>
            </div>
        </section>

        <div class="main-content">
            <!-- Statistics -->
            <div class="stats-grid">
                <div class="stat-item glass-widget">
                    <span class="stat-number">1,200</span>
                    <div class="stat-label">متر ارتفاع از سطح دریا</div>
                </div>
                <div class="stat-item glass-widget">
                    <span class="stat-number">85,000</span>
                    <div class="stat-label">نفر جمعیت</div>
                </div>
                <div class="stat-item glass-widget">
                    <span class="stat-number">2,400</span>
                    <div class="stat-label">کیلومتر مربع مساحت</div>
                </div>
                <div class="stat-item glass-widget">
                    <span class="stat-number">150+</span>
                    <div class="stat-label">جاذبه گردشگری</div>
                </div>
            </div>

            <!-- Features -->
            <h2 class="section-title">ویژگی‌های منحصربه‌فرد دورود</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openCardDialog('zagros', '🏔️', 'کوه‌های زاگرس')">
                    <span class="card-icon">🏔️</span>
                    <h3>کوه‌های زاگرس</h3>
                    <p>رشته کوه‌های مرتفع زاگرس با قله‌های برفی و مناظر خیره‌کننده که محل زندگی گونه‌های کمیاب حیوانات و گیاهان است.</p>
                </div>
                <div class="card glass-widget" onclick="openCardDialog('forests', '🌲', 'جنگل‌های انبوه')">
                    <span class="card-icon">🌲</span>
                    <h3>جنگل‌های انبوه</h3>
                    <p>جنگل‌های بلوط و بادام کوهی که در فصل پاییز رنگ‌های طلایی و قرمز زیبایی خلق می‌کنند.</p>
                </div>
                <div class="card glass-widget" onclick="openCardDialog('springs', '💧', 'چشمه‌های زلال')">
                    <span class="card-icon">💧</span>
                    <h3>چشمه‌های زلال</h3>
                    <p>آب‌های خنک و شفاف که از دل کوه‌های زاگرس جاری می‌شوند و خواص درمانی دارند.</p>
                </div>
                <div class="card glass-widget" onclick="openCardDialog('heritage', '🏛️', 'میراث تاریخی')">
                    <span class="card-icon">🏛️</span>
                    <h3>میراث تاریخی</h3>
                    <p>آثار باستانی و تاریخی که نشان‌دهنده تمدن کهن این سرزمین و فرهنگ غنی مردم لرستان است.</p>
                </div>
            </div>

            <!-- Weather Section -->
            <h2 class="section-title">آب و هوای دورود</h2>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌡️</span>
                    <h3>دمای فعلی</h3>
                    <p><span id="temperature" style="font-size: 2rem; font-weight: 700; color: #555;">22°C</span><br>
                    آفتابی و دلپذیر</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">💨</span>
                    <h3>وضعیت باد</h3>
                    <p><span style="font-size: 1.5rem; font-weight: 600; color: #555;">12 km/h</span><br>
                    باد ملایم از شمال غرب</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">💧</span>
                    <h3>رطوبت هوا</h3>
                    <p><span style="font-size: 1.5rem; font-weight: 600; color: #555;">65%</span><br>
                    رطوبت مناسب و طبیعی</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌅</span>
                    <h3>طلوع و غروب</h3>
                    <p><span style="font-size: 1.2rem; font-weight: 600; color: #555;">06:30 - 18:45</span><br>
                    ساعات روشنایی: 12 ساعت و 15 دقیقه</p>
                </div>
            </div>

            <!-- Technology & Innovation Section -->
            <h2 class="section-title">تکنولوژی و نوآوری</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openSmartGuide()">
                    <span class="card-icon">📱</span>
                    <h3>اپلیکیشن موبایل دورود</h3>
                    <p>اپلیکیشن هوشمند با نقشه آفلاین، راهنمای صوتی، پیش‌بینی آب و هوا و رزرو آنلاین هتل‌ها و تورها.</p>
                </div>
                <div class="card glass-widget" onclick="openQRTour()">
                    <span class="card-icon">📷</span>
                    <h3>تور QR کد</h3>
                    <p>کدهای QR در تمام جاذبه‌ها برای دریافت اطلاعات فوری، تصاویر تاریخی و راهنمای صوتی به زبان‌های مختلف.</p>
                </div>
                <div class="card glass-widget" onclick="openDroneView()">
                    <span class="card-icon">🚁</span>
                    <h3>نمای پهپادی زنده</h3>
                    <p>تصاویر زنده از پهپاد از جاذبه‌های اصلی، وضعیت ترافیک جاده‌ها و شرایط آب و هوایی کوهستان.</p>
                </div>
                <div class="card glass-widget" onclick="openAIPlanner()">
                    <span class="card-icon">🧠</span>
                    <h3>برنامه‌ریز هوشمند سفر</h3>
                    <p>هوش مصنوعی که بر اساس علایق، بودجه و زمان شما بهترین برنامه سفر را طراحی می‌کند.</p>
                </div>
            </div>

            <!-- Interactive Features Section -->
            <h2 class="section-title">امکانات تعاملی</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openVRTour()">
                    <span class="card-icon">🥽</span>
                    <h3>تور مجازی 360°</h3>
                    <p>بازدید مجازی از جاذبه‌های دورود با تکنولوژی واقعیت مجازی. کوهستان، جنگل، آبشار و غار را از نزدیک ببینید.</p>
                </div>
                <div class="card glass-widget" onclick="toggleChatbot()">
                    <span class="card-icon">🤖</span>
                    <h3>راهنمای هوشمند</h3>
                    <p>چت‌بات هوشمند برای پاسخ به سوالات شما درباره دورود. اطلاعات گردشگری، اقامت، غذا و جاذبه‌ها.</p>
                </div>
                <div class="card glass-widget" onclick="toggleAudioPlayer()">
                    <span class="card-icon">🎵</span>
                    <h3>صداهای طبیعت</h3>
                    <p>گوش دادن به صداهای آرامش‌بخش طبیعت دورود: آبشار، پرندگان، جنگل و باد کوهستان.</p>
                </div>
                <div class="card glass-widget" onclick="showLiveInfo()">
                    <span class="card-icon">📊</span>
                    <h3>اطلاعات زنده</h3>
                    <p>وضعیت ترافیک جاده‌ها، رویدادهای روز، آخرین اخبار منطقه و اطلاعات به‌روز گردشگری.</p>
                </div>
            </div>

            <!-- Eco-Tourism Section -->
            <h2 class="section-title">اکوتوریسم و حفاظت از طبیعت</h2>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌱</span>
                    <h3>گردشگری پایدار</h3>
                    <p>برنامه‌های گردشگری سازگار با محیط زیست که به حفظ طبیعت کمک می‌کند و درآمد پایدار برای مردم محلی ایجاد می‌کند.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">♻️</span>
                    <h3>صفر ضایعات</h3>
                    <p>سیستم مدیریت زباله و بازیافت در تمام جاذبه‌های گردشگری. استفاده از ظروف قابل تجدید و کاهش پلاستیک.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🦋</span>
                    <h3>حفاظت از حیات وحش</h3>
                    <p>برنامه‌های حفاظت از گونه‌های در معرض خطر، ایجاد کریدورهای حیات وحش و نظارت بر اکوسیستم کوهستانی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">💧</span>
                    <h3>مدیریت منابع آب</h3>
                    <p>حفاظت از چشمه‌ها و آبشارها، سیستم‌های آبیاری قطره‌ای و استفاده بهینه از منابع آبی کوهستان.</p>
                </div>
            </div>

            <!-- Online Shop Section -->
            <h2 class="section-title">فروشگاه آنلاین دورود</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openOnlineShop('souvenirs')">
                    <span class="card-icon">🛍️</span>
                    <h3>سوغات و صنایع دستی</h3>
                    <p>گلیم‌های دست‌باف، سفال‌های سنتی، چوب‌تراشی‌های زیبا و صنایع دستی اصیل لرستان را آنلاین سفارش دهید.</p>
                </div>
                <div class="card glass-widget" onclick="openOnlineShop('organic')">
                    <span class="card-icon">🌾</span>
                    <h3>محصولات ارگانیک</h3>
                    <p>گردو، بادام، انجیر، عسل طبیعی، پنیر و کشک محلی مستقیم از تولیدکنندگان روستایی.</p>
                </div>
                <div class="card glass-widget" onclick="openOnlineShop('books')">
                    <span class="card-icon">📚</span>
                    <h3>کتاب و نقشه</h3>
                    <p>راهنمای گردشگری، نقشه‌های کوهنوردی، کتاب‌های فرهنگ لری و مجموعه عکس‌های دورود.</p>
                </div>
                <div class="card glass-widget" onclick="openOnlineShop('clothing')">
                    <span class="card-icon">👕</span>
                    <h3>پوشاک محلی</h3>
                    <p>لباس‌های سنتی لری، کلاه‌های محلی، شال و روسری‌های دست‌باف و تی‌شرت‌های یادگاری.</p>
                </div>
            </div>

            <!-- Educational Center Section -->
            <h2 class="section-title">مرکز آموزش و یادگیری</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openEducationCenter('mountaineering')">
                    <span class="card-icon">🧗</span>
                    <h3>دوره‌های کوهنوردی</h3>
                    <p>آموزش کوهنوردی از مبتدی تا حرفه‌ای، تکنیک‌های صخره‌نوردی، ایمنی کوهستان و استفاده از تجهیزات.</p>
                </div>
                <div class="card glass-widget" onclick="openEducationCenter('photography')">
                    <span class="card-icon">📸</span>
                    <h3>عکاسی طبیعت</h3>
                    <p>کلاس‌های عکاسی منظره، عکاسی حیات وحش، تکنیک‌های نوردهی و ترکیب‌بندی در طبیعت.</p>
                </div>
                <div class="card glass-widget" onclick="openEducationCenter('crafts')">
                    <span class="card-icon">🎨</span>
                    <h3>صنایع دستی</h3>
                    <p>آموزش گلیم‌بافی، سفالگری، چوب‌تراشی و سایر هنرهای سنتی توسط استادکاران محلی.</p>
                </div>
                <div class="card glass-widget" onclick="openEducationCenter('language')">
                    <span class="card-icon">🗣️</span>
                    <h3>زبان و فرهنگ لری</h3>
                    <p>آموزش زبان لری، آشنایی با فرهنگ و آداب محلی، ضرب‌المثل‌ها و داستان‌های عامیانه.</p>
                </div>
            </div>

            <!-- Health Services Section -->
            <h2 class="section-title">خدمات سلامت و درمان</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openHealthServices('medical')">
                    <span class="card-icon">🏥</span>
                    <h3>مراکز درمانی</h3>
                    <p>بیمارستان دورود، درمانگاه‌های تخصصی، داروخانه‌ها و مراکز اورژانس با آدرس و شماره تماس.</p>
                </div>
                <div class="card glass-widget" onclick="openHealthServices('traditional')">
                    <span class="card-icon">🌿</span>
                    <h3>طب سنتی</h3>
                    <p>مراکز طب سنتی، گیاه‌درمانی، حجامت، ماساژ درمانی و روش‌های طبیعی درمان بیماری‌ها.</p>
                </div>
                <div class="card glass-widget" onclick="openHealthServices('emergency')">
                    <span class="card-icon">🚑</span>
                    <h3>خدمات اورژانس</h3>
                    <p>اورژانس کوهستان، امداد و نجات، هلال احمر، آتش‌نشانی و شماره‌های ضروری منطقه.</p>
                </div>
                <div class="card glass-widget" onclick="openHealthServices('wellness')">
                    <span class="card-icon">🧘</span>
                    <h3>مراکز تندرستی</h3>
                    <p>مراکز یوگا، مدیتیشن، ماساژ درمانی، آب‌درمانی و برنامه‌های سلامت جسم و روح.</p>
                </div>
            </div>

            <!-- Transportation Section -->
            <h2 class="section-title">حمل‌ونقل و دسترسی</h2>
            <div class="cards-grid">
                <div class="card glass-widget" onclick="openTransportation('rental')">
                    <span class="card-icon">🚗</span>
                    <h3>اجاره خودرو</h3>
                    <p>اجاره انواع خودرو از اقتصادی تا شاسی‌بلند، موتورسیکلت کوهستان و دوچرخه برای گردش در طبیعت.</p>
                </div>
                <div class="card glass-widget" onclick="openTransportation('taxi')">
                    <span class="card-icon">🚕</span>
                    <h3>تاکسی‌های محلی</h3>
                    <p>تاکسی‌های شهری، تاکسی‌های بین‌شهری، سرویس‌های ویژه گردشگری و راننده‌های آشنا به منطقه.</p>
                </div>
                <div class="card glass-widget" onclick="openTransportation('routes')">
                    <span class="card-icon">🗺️</span>
                    <h3>راهنمای مسیرها</h3>
                    <p>نقشه جاده‌ها، مسیرهای دسترسی به جاذبه‌ها، وضعیت ترافیک و بهترین زمان‌های سفر.</p>
                </div>
                <div class="card glass-widget" onclick="openTransportation('parking')">
                    <span class="card-icon">🅿️</span>
                    <h3>پارکینگ و توقف</h3>
                    <p>پارکینگ‌های عمومی، محل‌های مجاز توقف در جاذبه‌ها، پارکینگ‌های امن و نگهبانی‌دار.</p>
                </div>
            </div>

            <!-- Map Section -->
            <div class="map-section glass-widget">
                <h2 class="section-title">موقعیت جغرافیایی دورود</h2>
                <div class="map-container" onclick="openMap()">
                    <div class="map-placeholder">🗺️</div>
                    <div class="map-text">کلیک کنید تا نقشه را مشاهده کنید</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Culture Page -->
    <div id="culture" class="page">
        <div class="main-content">
            <h2 class="section-title">فرهنگ و سنت‌های دورود</h2>
            
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🎵</span>
                    <h3>موسیقی محلی</h3>
                    <p>موسیقی اصیل لری با سازهای سنتی مثل دف، نی و کمانچه که روح و جان مردم این سرزمین را نمایان می‌سازد.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🍲</span>
                    <h3>غذاهای محلی</h3>
                    <p>آشپزی سنتی با استفاده از گیاهان کوهی، شیر و پنیر طبیعی و گوشت دام‌های محلی که طعم‌های بی‌نظیری دارد.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🧵</span>
                    <h3>صنایع دستی</h3>
                    <p>گلیم‌بافی، سفالگری، چوب‌تراشی و سایر هنرهای سنتی که از نسلی به نسل دیگر منتقل شده‌اند.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🎭</span>
                    <h3>جشن‌ها و مراسم</h3>
                    <p>جشن‌های سنتی مثل جشن برداشت، نوروز کوهستانی و مراسم عروسی با آداب و رسوم خاص منطقه.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">👥</span>
                    <h3>مهمان‌نوازی</h3>
                    <p>فرهنگ گرم و صمیمی مردم لر که مهمان‌نوازی و کمک به همدیگر از ارزش‌های اصلی آن‌هاست.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">📚</span>
                    <h3>ادبیات شفاهی</h3>
                    <p>قصه‌ها، ضرب‌المثل‌ها و شعرهای محلی که حکمت و تجربه اجداد را در خود جای داده‌اند.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- History Page -->
    <div id="history" class="page">
        <div class="main-content">
            <h2 class="section-title">تاریخچه دورود</h2>
            
            <div class="events-timeline">
                <div class="timeline-line"></div>
                
                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>دوران باستان</h3>
                        <p>اولین سکونتگاه‌های انسانی در منطقه دورود به دوران پارینه سنگی برمی‌گردد. غارهای متعددی در این منطقه وجود دارد که نشان‌دهنده حضور انسان‌های اولیه است.</p>
                    </div>
                    <div class="event-date">10000 سال پیش</div>
                </div>

                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>تمدن عیلام</h3>
                        <p>دورود در دوران تمدن عیلام به عنوان یکی از مراکز مهم تجاری و فرهنگی شناخته می‌شد. آثار متعددی از این دوران در منطقه کشف شده است.</p>
                    </div>
                    <div class="event-date">3200 ق.م</div>
                </div>

                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>دوران ساسانی</h3>
                        <p>در دوران ساسانی، دورود به عنوان یکی از شهرهای مهم استان لرستان شناخته می‌شد و پل‌ها و راه‌های مهمی در آن ساخته شد.</p>
                    </div>
                    <div class="event-date">224-651 م</div>
                </div>

                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>دوران اسلامی</h3>
                        <p>با ورود اسلام، دورود همچنان به عنوان مرکز مهم منطقه باقی ماند و مساجد و مدارس متعددی در آن ساخته شد.</p>
                    </div>
                    <div class="event-date">651 م</div>
                </div>

                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>دوران معاصر</h3>
                        <p>در دوران معاصر، دورود به عنوان یکی از شهرستان‌های مهم لرستان شناخته می‌شود و مرکز صنعتی و گردشگری مهمی محسوب می‌شود.</p>
                    </div>
                    <div class="event-date">1900 تاکنون</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Tourism Page -->
    <div id="tourism" class="page">
        <div class="main-content">
            <h2 class="section-title">جاذبه‌های گردشگری دورود</h2>
            
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🏔️</span>
                    <h3>قله اشترانکوه</h3>
                    <p>بلندترین قله منطقه با ارتفاع 4050 متر که مقصد محبوب کوهنوردان و طبیعت‌دوستان است.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">💧</span>
                    <h3>آبشار بیشه‌لو</h3>
                    <p>یکی از زیباترین آبشارهای ایران با ارتفاع 48 متر که در فصل بهار و تابستان منظره‌ای خیره‌کننده دارد.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🕳️</span>
                    <h3>غار علیصدر</h3>
                    <p>بزرگترین غار آبی جهان که با قایق‌های کوچک قابل بازدید است و از عجایب طبیعی ایران محسوب می‌شود.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌊</span>
                    <h3>چشمه گرماب</h3>
                    <p>چشمه آب گرم طبیعی با خواص درمانی که برای درمان بیماری‌های پوستی و مفصلی استفاده می‌شود.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌲</span>
                    <h3>جنگل‌های زاگرس</h3>
                    <p>جنگل‌های انبوه بلوط که در پاییز رنگ‌های زیبایی به خود می‌گیرند و محل زندگی حیوانات کمیاب هستند.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏛️</span>
                    <h3>پل کشکان</h3>
                    <p>پل تاریخی ساسانی که یکی از شاهکارهای معماری ایران باستان محسوب می‌شود.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🕳️</span>
                    <h3>چاه تیان</h3>
                    <p>چاه عمیق و اسرارآمیز در انتهای روستای تیان، در میان کوه‌های زاگرس و نزدیک تپه‌های اشترانکوه که داستان‌ها و افسانه‌های محلی زیادی دارد.</p>
                </div>
            </div>

            <!-- Adventure Tourism Section -->
            <h3 class="section-title" style="margin-top: 4rem;">ماجراجویی و فعالیت‌های هیجان‌انگیز</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🧗</span>
                    <h3>کوهنوردی و صخره‌نوردی</h3>
                    <p>قله‌های چالش‌برانگیز زاگرس برای کوهنوردان حرفه‌ای و مبتدی. مسیرهای مختلف با درجات سختی متفاوت و راهنمایان مجرب.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🚵</span>
                    <h3>دوچرخه‌سواری کوهستان</h3>
                    <p>مسیرهای هیجان‌انگیز دوچرخه‌سواری در طبیعت بکر دورود. از مسیرهای آسان خانوادگی تا مسیرهای اکستریم برای حرفه‌ای‌ها.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏕️</span>
                    <h3>کمپینگ و بوشکرافت</h3>
                    <p>تجربه زندگی در طبیعت با کمپینگ در بهترین نقاط دورود. آموزش مهارت‌های بقا و زندگی در طبیعت.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🎣</span>
                    <h3>ماهیگیری ورزشی</h3>
                    <p>ماهیگیری در رودخانه‌ها و چشمه‌های زلال دورود. ماهی‌های قزل‌آلا و کپور در آب‌های خنک کوهستانی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🪂</span>
                    <h3>پاراگلایدر و هوابازی</h3>
                    <p>پرواز بر فراز کوه‌های زیبای دورود با پاراگلایدر. مناظر خیره‌کننده از ارتفاع و تجربه‌ای فراموش‌نشدنی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏃</span>
                    <h3>دوی کوهستان و تریل رانینگ</h3>
                    <p>مسابقات و تمرینات دوی کوهستان در مسیرهای طبیعی. از دویدن آرام تا مسابقات حرفه‌ای تریل رانینگ.</p>
                </div>
            </div>

            <!-- Wellness Tourism Section -->
            <h3 class="section-title" style="margin-top: 4rem;">سلامت و آرامش</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">♨️</span>
                    <h3>آب‌درمانی طبیعی</h3>
                    <p>چشمه‌های آب گرم با خواص درمانی برای درمان بیماری‌های مفصلی، پوستی و استرس. آب‌های معدنی با ترکیبات مفید.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🧘</span>
                    <h3>یوگا و مدیتیشن</h3>
                    <p>کلاس‌های یوگا و مدیتیشن در طبیعت بکر. آرامش ذهن و جسم در محیطی آرام و دور از آلودگی شهری.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌿</span>
                    <h3>طب سنتی و گیاه‌درمانی</h3>
                    <p>استفاده از گیاهان دارویی محلی برای درمان‌های طبیعی. مشاوره با طبیبان سنتی و تهیه داروهای گیاهی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🍃</span>
                    <h3>هوای پاک کوهستان</h3>
                    <p>تنفس هوای پاک و غنی از اکسیژن کوهستان. مفید برای بیماری‌های تنفسی و تقویت سیستم ایمنی بدن.</p>
                </div>
            </div>
        </div>
    </div>



    <!-- Villages Page -->
    <div id="villages" class="page">
        <div class="main-content">
            <h2 class="section-title">روستاهای زیبای دورود</h2>
            
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌅</span>
                    <h3>روستای بر افتاب</h3>
                    <p>روستایی زیبا در دامنه کوه‌های زاگرس که نام آن از موقعیت خاصش در برابر نور خورشید گرفته شده. مشهور به باغ‌های میوه و چشمه‌های زلال.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🚪</span>
                    <h3>روستای دربند</h3>
                    <p>روستای کوهستانی با معماری سنتی و خانه‌های پلکانی. دارای آب و هوای خنک و طبیعت بکر که مقصد مناسبی برای استراحت و آرامش است.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🕌</span>
                    <h3>روستای پیر عبدالله</h3>
                    <p>روستای تاریخی با بقعه مقدس پیر عبدالله که مرکز زیارت و معنویت منطقه محسوب می‌شود. دارای جاذبه‌های مذهبی و فرهنگی فراوان.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🕳️</span>
                    <h3>روستای تیان و چاه تیان</h3>
                    <p>روستای کوهستانی تیان با چاه اسرارآمیز و عمیق در انتهای روستا که در میان کوه‌های زاگرس و نزدیک اشترانکوه قرار دارد. محل افسانه‌ها و داستان‌های محلی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏘️</span>
                    <h3>سایر روستاها</h3>
                    <p>دهه‌ها روستای دیگر با ویژگی‌های منحصربه‌فرد: چم‌آسمان، سراب دوره، کاکارضا، گل‌تپه و بسیاری روستاهای زیبای دیگر.</p>
                </div>
            </div>

            <!-- Village Features -->
            <h3 class="section-title" style="margin-top: 4rem;">ویژگی‌های روستاهای دورود</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🏠</span>
                    <h3>معماری سنتی</h3>
                    <p>خانه‌های سنگی و گلی با سقف‌های شیبدار که با اقلیم کوهستانی منطقه سازگار هستند و زیبایی خاصی دارند.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌾</span>
                    <h3>کشاورزی ارگانیک</h3>
                    <p>تولید محصولات کشاورزی طبیعی و ارگانیک مثل گردو، بادام، انجیر و انواع سبزیجات کوهستانی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🐑</span>
                    <h3>دامداری سنتی</h3>
                    <p>پرورش گوسفند، بز و گاو در مراتع طبیعی که تولید شیر، پنیر و کشک با کیفیت بالا را به همراه دارد.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🎨</span>
                    <h3>صنایع دستی</h3>
                    <p>تولید گلیم، جاجیم، سفال، چوب‌تراشی و سایر صنایع دستی که هنر و مهارت مردم محلی را نشان می‌دهد.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏕️</span>
                    <h3>بوم‌گردی</h3>
                    <p>امکان اقامت در خانه‌های روستایی، تجربه زندگی محلی، شرکت در فعالیت‌های کشاورزی و لذت بردن از طبیعت.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🥾</span>
                    <h3>مسیرهای پیاده‌روی</h3>
                    <p>مسیرهای طبیعی و زیبا برای پیاده‌روی و کوهنوردی که از روستا شروع شده و به نقاط دیدنی منتهی می‌شوند.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Gallery Page -->
    <div id="gallery" class="page">
        <div class="main-content">
            <h2 class="section-title">گالری تصاویر دورود</h2>
            
            <!-- Gallery Categories -->
            <div class="gallery-categories">
                <button class="gallery-cat-btn active" onclick="showGalleryCategory('all')">🖼️ همه</button>
                <button class="gallery-cat-btn" onclick="showGalleryCategory('nature')">🌿 طبیعت</button>
                <button class="gallery-cat-btn" onclick="showGalleryCategory('villages')">🏘️ روستاها</button>
                <button class="gallery-cat-btn" onclick="showGalleryCategory('culture')">🎭 فرهنگ</button>
                <button class="gallery-cat-btn" onclick="showGalleryCategory('history')">🏛️ تاریخ</button>
            </div>
            
            <div class="gallery-grid" id="galleryGrid">
                <!-- Nature Category -->
                <div class="gallery-item glass-widget" data-category="nature">
                    🏔️
                    <div class="gallery-overlay">
                        <h4>کوه‌های زاگرس</h4>
                        <p>مناظر خیره‌کننده قله‌های برفی</p>
                        <button onclick="openImageModal('کوه‌های زاگرس', '🏔️')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="nature">
                    💧
                    <div class="gallery-overlay">
                        <h4>آبشار بیشه‌لو</h4>
                        <p>آبشار زیبا در دل طبیعت</p>
                        <button onclick="openImageModal('آبشار بیشه‌لو', '💧')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="nature">
                    🌲
                    <div class="gallery-overlay">
                        <h4>جنگل‌های پاییزی</h4>
                        <p>رنگ‌های طلایی پاییز</p>
                        <button onclick="openImageModal('جنگل‌های پاییزی', '🌲')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="nature">
                    🕳️
                    <div class="gallery-overlay">
                        <h4>غار علیصدر</h4>
                        <p>بزرگترین غار آبی جهان</p>
                        <button onclick="openImageModal('غار علیصدر', '🕳️')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="nature">
                    🌊
                    <div class="gallery-overlay">
                        <h4>چشمه گرماب</h4>
                        <p>آب‌های گرم درمانی</p>
                        <button onclick="openImageModal('چشمه گرماب', '🌊')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="nature">
                    🌸
                    <div class="gallery-overlay">
                        <h4>بهار کوهستان</h4>
                        <p>شکوفه‌های بهاری</p>
                        <button onclick="openImageModal('بهار کوهستان', '🌸')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>

                <!-- Villages Category -->
                <div class="gallery-item glass-widget" data-category="villages">
                    🌅
                    <div class="gallery-overlay">
                        <h4>روستای بر افتاب</h4>
                        <p>روستای زیبا در برابر خورشید</p>
                        <button onclick="openImageModal('روستای بر افتاب', '🌅')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="villages">
                    🚪
                    <div class="gallery-overlay">
                        <h4>روستای دربند</h4>
                        <p>معماری سنتی کوهستانی</p>
                        <button onclick="openImageModal('روستای دربند', '🚪')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="villages">
                    🕌
                    <div class="gallery-overlay">
                        <h4>روستای پیر عبدالله</h4>
                        <p>مرکز معنویت و زیارت</p>
                        <button onclick="openImageModal('روستای پیر عبدالله', '🕌')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>

                <!-- Culture Category -->
                <div class="gallery-item glass-widget" data-category="culture">
                    🎵
                    <div class="gallery-overlay">
                        <h4>موسیقی محلی</h4>
                        <p>سازهای سنتی لری</p>
                        <button onclick="openImageModal('موسیقی محلی', '🎵')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="culture">
                    🧵
                    <div class="gallery-overlay">
                        <h4>صنایع دستی</h4>
                        <p>گلیم‌بافی و سفالگری</p>
                        <button onclick="openImageModal('صنایع دستی', '🧵')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="culture">
                    🍲
                    <div class="gallery-overlay">
                        <h4>غذاهای محلی</h4>
                        <p>آشپزی سنتی لرستان</p>
                        <button onclick="openImageModal('غذاهای محلی', '🍲')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>

                <!-- History Category -->
                <div class="gallery-item glass-widget" data-category="history">
                    🏛️
                    <div class="gallery-overlay">
                        <h4>پل کشکان</h4>
                        <p>معماری ساسانی</p>
                        <button onclick="openImageModal('پل کشکان', '🏛️')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="history">
                    🏺
                    <div class="gallery-overlay">
                        <h4>آثار باستانی</h4>
                        <p>میراث تاریخی دورود</p>
                        <button onclick="openImageModal('آثار باستانی', '🏺')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
                <div class="gallery-item glass-widget" data-category="nature">
                    🦅
                    <div class="gallery-overlay">
                        <h4>حیات وحش</h4>
                        <p>پرندگان کمیاب منطقه</p>
                        <button onclick="openImageModal('حیات وحش', '🦅')" class="view-btn">👁️ مشاهده</button>
                    </div>
                </div>
            </div>

            <!-- Image Modal -->
            <div class="image-modal" id="imageModal">
                <div class="modal-content glass-widget">
                    <div class="modal-header">
                        <h3 id="modalTitle">عنوان تصویر</h3>
                        <button onclick="closeImageModal()" class="modal-close">✕</button>
                    </div>
                    <div class="modal-body">
                        <div class="modal-image" id="modalImage">🖼️</div>
                        <div class="modal-info">
                            <p id="modalDescription">توضیحات تصویر در اینجا نمایش داده می‌شود.</p>
                            <div class="modal-actions">
                                <button onclick="shareImage()" class="action-btn">📤 اشتراک‌گذاری</button>
                                <button onclick="downloadImage()" class="action-btn">💾 دانلود</button>
                                <button onclick="setWallpaper()" class="action-btn">🖼️ تصویر زمینه</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Events Page -->
    <div id="events" class="page">
        <div class="main-content">
            <h2 class="section-title">رویدادها و جشنواره‌ها</h2>
            
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌸</span>
                    <h3>جشنواره بهار کوهستان</h3>
                    <p>جشنواره سالانه که در فروردین ماه برگزار می‌شود و شامل نمایشگاه صنایع دستی، موسیقی محلی و غذاهای سنتی است.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🍂</span>
                    <h3>جشن برداشت پاییز</h3>
                    <p>جشن سنتی برداشت محصولات کشاورزی که در مهر ماه برگزار شده و نمایانگر فرهنگ کشاورزی منطقه است.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏔️</span>
                    <h3>مسابقات کوهنوردی</h3>
                    <p>مسابقات سالانه کوهنوردی که در تابستان برگزار می‌شود و کوهنوردان از سراسر کشور در آن شرکت می‌کنند.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🎭</span>
                    <h3>جشنواره فرهنگ لری</h3>
                    <p>نمایش فرهنگ و سنت‌های اصیل مردم لر شامل موسیقی، رقص، شعر و ادبیات محلی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">📸</span>
                    <h3>مسابقه عکاسی طبیعت</h3>
                    <p>مسابقه سالانه عکاسی از طبیعت و مناظر زیبای دورود که در فصل پاییز برگزار می‌شود.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏃</span>
                    <h3>دوی کوهستان</h3>
                    <p>مسابقات دوی کوهستان که در مسیرهای طبیعی و چالش‌برانگیز دورود برگزار می‌شود.</p>
                </div>
            </div>

            <!-- Upcoming Events -->
            <h3 class="section-title" style="margin-top: 4rem;">رویدادهای پیش رو</h3>
            <div class="events-timeline">
                <div class="timeline-line"></div>
                
                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>جشنواره زمستان کوهستان</h3>
                        <p>جشنواره‌ای ویژه فصل زمستان با فعالیت‌های برفی، اسکی و ورزش‌های زمستانی در کوه‌های دورود.</p>
                    </div>
                    <div class="event-date">دی 1404</div>
                </div>

                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>نمایشگاه صنایع دستی</h3>
                        <p>نمایشگاه بزرگ صنایع دستی و سوغات محلی با حضور هنرمندان و صنعتگران منطقه.</p>
                    </div>
                    <div class="event-date">بهمن 1404</div>
                </div>

                <div class="event-item">
                    <div class="event-content glass-widget">
                        <h3>جشن نوروز کوهستانی</h3>
                        <p>جشن سنتی نوروز با آداب و رسوم خاص مردم کوهستان و برگزاری مراسم‌های محلی.</p>
                    </div>
                    <div class="event-date">فروردین 1405</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Ecotourism Page -->
    <div id="ecotourism" class="page">
        <div class="main-content">
            <h2 class="section-title">اکوتوریسم دورود - گردشگری پایدار</h2>
            
            <!-- Introduction Section -->
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌍</span>
                    <h3>گردشگری مسئولانه</h3>
                    <p>اکوتوریسم دورود بر حفظ طبیعت، احترام به فرهنگ محلی و ایجاد درآمد پایدار برای جوامع روستایی تأکید دارد.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🦋</span>
                    <h3>حفاظت از تنوع زیستی</h3>
                    <p>کوه‌های زاگرس خانه گونه‌های کمیاب گیاهی و جانوری است که با اکوتوریسم از آن‌ها محافظت می‌کنیم.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">👥</span>
                    <h3>توسعه جوامع محلی</h3>
                    <p>اکوتوریسم فرصت‌های شغلی برای مردم محلی ایجاد کرده و از فرهنگ و سنت‌های آن‌ها حمایت می‌کند.</p>
                </div>
            </div>

            <!-- Eco-Activities Section -->
            <h3 class="section-title" style="margin-top: 4rem;">فعالیت‌های اکوتوریستی</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🥾</span>
                    <h3>پیاده‌روی اکولوژیک</h3>
                    <p>مسیرهای پیاده‌روی طراحی‌شده برای کمترین تأثیر بر محیط زیست. راهنمایان محلی اکوسیستم را معرفی می‌کنند.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🦅</span>
                    <h3>پرنده‌نگری</h3>
                    <p>مشاهده پرندگان کمیاب زاگرس در زیستگاه طبیعی‌شان. بهترین زمان: صبح زود و غروب آفتاب.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌿</span>
                    <h3>گیاه‌شناسی کاربردی</h3>
                    <p>آشنایی با گیاهان دارویی و خوراکی منطقه. یادگیری استفاده سنتی از گیاهان توسط مردم محلی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">📸</span>
                    <h3>عکاسی طبیعت</h3>
                    <p>عکاسی مسئولانه از طبیعت بدون مزاحمت برای حیوانات. کارگاه‌های عکاسی با متخصصان.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏕️</span>
                    <h3>کمپینگ سبز</h3>
                    <p>کمپینگ با رعایت اصول Leave No Trace. استفاده از تجهیزات سازگار با محیط زیست.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌊</span>
                    <h3>حفاظت از آب</h3>
                    <p>آشنایی با چرخه آب در کوهستان، حفاظت از چشمه‌ها و رودخانه‌ها، و استفاده بهینه از منابع آبی.</p>
                </div>
            </div>

            <!-- Sustainable Accommodation -->
            <h3 class="section-title" style="margin-top: 4rem;">اقامتگاه‌های پایدار</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🏠</span>
                    <h3>بوم‌گردی روستایی</h3>
                    <p>اقامت در خانه‌های سنتی روستایی با معماری محلی. تجربه زندگی اصیل کوهنشینان و مشارکت در فعالیت‌های روزانه.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">⚡</span>
                    <h3>انرژی تجدیدپذیر</h3>
                    <p>اقامتگاه‌هایی که از انرژی خورشیدی و بادی استفاده می‌کنند. سیستم‌های گرمایش طبیعی و صرفه‌جویی در انرژی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">♻️</span>
                    <h3>مدیریت زباله</h3>
                    <p>سیستم تفکیک و بازیافت زباله در اقامتگاه‌ها. کمپوست‌سازی از مواد آلی و کاهش تولید زباله.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🥬</span>
                    <h3>غذای ارگانیک محلی</h3>
                    <p>استفاده از محصولات ارگانیک تولیدی روستاییان. باغ‌های سبزیجات طبیعی و دام‌های بومی منطقه.</p>
                </div>
            </div>

            <!-- Conservation Programs -->
            <h3 class="section-title" style="margin-top: 4rem;">برنامه‌های حفاظتی</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌳</span>
                    <h3>جنگل‌کاری مشارکتی</h3>
                    <p>برنامه کاشت درخت با مشارکت گردشگران. هر بازدیدکننده می‌تواند درختی بکارد و از رشد آن مطلع شود.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🐻</span>
                    <h3>حفاظت از حیات وحش</h3>
                    <p>نظارت بر جمعیت حیوانات، ایجاد کریدورهای حیات وحش و جلوگیری از شکار غیرمجاز.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🔬</span>
                    <h3>تحقیقات زیست‌محیطی</h3>
                    <p>مشارکت در پروژه‌های تحقیقاتی دانشگاه‌ها برای مطالعه اکوسیستم کوهستانی و تغییرات اقلیمی.</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">📚</span>
                    <h3>آموزش زیست‌محیطی</h3>
                    <p>کارگاه‌های آموزشی برای کودکان و بزرگسالان درباره اهمیت حفاظت از طبیعت و زندگی پایدار.</p>
                </div>
            </div>

            <!-- Eco-Tourism Guidelines -->
            <h3 class="section-title" style="margin-top: 4rem;">راهنمای اکوتوریست مسئول</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">👣</span>
                    <h3>Leave No Trace</h3>
                    <p>• فقط در مسیرهای تعیین‌شده حرکت کنید<br>• زباله خود را با خود ببرید<br>• از گیاهان و حیوانات فاصله نگه دارید<br>• آتش فقط در محل‌های مجاز روشن کنید</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🤝</span>
                    <h3>احترام به فرهنگ محلی</h3>
                    <p>• از آداب و رسوم محلی پیروی کنید<br>• محصولات محلی خریداری کنید<br>• با مردم محلی مودبانه رفتار کنید<br>• از عکس‌گیری بی‌اجازه خودداری کنید</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">💧</span>
                    <h3>صرفه‌جویی در منابع</h3>
                    <p>• از آب و انرژی صرفه‌جویی کنید<br>• از ظروف قابل استفاده مجدد استفاده کنید<br>• حمل‌ونقل عمومی را ترجیح دهید<br>• در گروه‌های کوچک سفر کنید</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🎓</span>
                    <h3>یادگیری و آگاهی</h3>
                    <p>• درباره اکوسیستم منطقه مطالعه کنید<br>• از راهنمایان محلی استفاده کنید<br>• تجربیات خود را با دیگران به اشتراک بگذارید<br>• در برنامه‌های حفاظتی مشارکت کنید</p>
                </div>
            </div>

            <!-- Eco-Tourism Impact -->
            <h3 class="section-title" style="margin-top: 4rem;">تأثیرات مثبت اکوتوریسم</h3>
            <div class="stats-grid">
                <div class="stat-item glass-widget">
                    <span class="stat-number">85%</span>
                    <div class="stat-label">کاهش مهاجرت روستایی</div>
                </div>
                <div class="stat-item glass-widget">
                    <span class="stat-number">200+</span>
                    <div class="stat-label">شغل ایجادشده</div>
                </div>
                <div class="stat-item glass-widget">
                    <span class="stat-number">15</span>
                    <div class="stat-label">گونه حفاظت‌شده</div>
                </div>
                <div class="stat-item glass-widget">
                    <span class="stat-number">5000</span>
                    <div class="stat-label">درخت کاشته‌شده</div>
                </div>
            </div>

            <!-- Eco-Tourism Packages -->
            <h3 class="section-title" style="margin-top: 4rem;">بسته‌های اکوتوریستی</h3>
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">🌅</span>
                    <h3>تور یک‌روزه طبیعت</h3>
                    <p><strong>مدت:</strong> 8 ساعت<br><strong>شامل:</strong> راهنمای محلی، ناهار ارگانیک، تجهیزات<br><strong>فعالیت‌ها:</strong> پیاده‌روی، پرنده‌نگری، عکاسی<br><strong>قیمت:</strong> 350 هزار تومان</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🏕️</span>
                    <h3>کمپ اکولوژیک 3 روزه</h3>
                    <p><strong>مدت:</strong> 2 شب و 3 روز<br><strong>شامل:</strong> اقامت، غذا، فعالیت‌ها<br><strong>ویژگی:</strong> کمپینگ سبز، کارگاه محیط زیست<br><strong>قیمت:</strong> 850 هزار تومان</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🌿</span>
                    <h3>بوم‌گردی هفتگی</h3>
                    <p><strong>مدت:</strong> 7 روز<br><strong>شامل:</strong> اقامت روستایی، غذای محلی<br><strong>تجربه:</strong> زندگی با خانواده‌های محلی<br><strong>قیمت:</strong> 1.8 میلیون تومان</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">🎓</span>
                    <h3>تور آموزشی دانشجویی</h3>
                    <p><strong>مدت:</strong> 5 روز<br><strong>مخاطب:</strong> دانشجویان و محققان<br><strong>شامل:</strong> کارگاه‌های تخصصی، تحقیق میدانی<br><strong>قیمت:</strong> 1.2 میلیون تومان</p>
                </div>
            </div>

            <!-- Booking Section -->
            <div class="contact-form glass-widget" style="margin-top: 3rem;">
                <h3 style="text-align: center; margin-bottom: 2rem; color: #555;">رزرو تور اکوتوریستی</h3>
                <form onsubmit="submitEcoTourForm(event)">
                    <div class="form-group">
                        <label for="ecoTourType">نوع تور:</label>
                        <select id="ecoTourType" name="tourType" required>
                            <option value="">انتخاب کنید...</option>
                            <option value="oneday">تور یک‌روزه طبیعت</option>
                            <option value="camping">کمپ اکولوژیک 3 روزه</option>
                            <option value="weekly">بوم‌گردی هفتگی</option>
                            <option value="educational">تور آموزشی دانشجویی</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="ecoTourDate">تاریخ مورد نظر:</label>
                        <input type="date" id="ecoTourDate" name="tourDate" required>
                    </div>
                    <div class="form-group">
                        <label for="ecoParticipants">تعداد شرکت‌کنندگان:</label>
                        <select id="ecoParticipants" name="participants" required>
                            <option value="">انتخاب کنید...</option>
                            <option value="1">1 نفر</option>
                            <option value="2">2 نفر</option>
                            <option value="3-5">3-5 نفر</option>
                            <option value="6-10">6-10 نفر</option>
                            <option value="10+">بیش از 10 نفر</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="ecoName">نام و نام خانوادگی:</label>
                        <input type="text" id="ecoName" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="ecoPhone">شماره تماس:</label>
                        <input type="tel" id="ecoPhone" name="phone" required>
                    </div>
                    <div class="form-group">
                        <label for="ecoEmail">ایمیل:</label>
                        <input type="email" id="ecoEmail" name="email">
                    </div>
                    <div class="form-group">
                        <label for="ecoMessage">درخواست‌های خاص:</label>
                        <textarea id="ecoMessage" name="message" rows="3" placeholder="نیازهای غذایی، محدودیت‌های جسمی، علایق خاص و..."></textarea>
                    </div>
                    <button type="submit" class="submit-btn">ارسال درخواست رزرو</button>
                </form>
            </div>
        </div>
    </div>

    <!-- Contact Page -->
    <div id="contact" class="page">
        <div class="main-content">
            <h2 class="section-title">تماس با ما</h2>
            
            <div class="cards-grid">
                <div class="card glass-widget">
                    <span class="card-icon">📍</span>
                    <h3>آدرس</h3>
                    <p>استان لرستان، شهرستان دورود<br>
                    میدان مرکزی، ساختمان شهرداری<br>
                    کد پستی: 6815613453</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">📞</span>
                    <h3>تلفن</h3>
                    <p>دفتر مرکزی: 066-52224455<br>
                    اطلاعات گردشگری: 066-52224466<br>
                    اورژانس: 110</p>
                </div>
                <div class="card glass-widget">
                    <span class="card-icon">✉️</span>
                    <h3>ایمیل</h3>
                    <p>info@dorud-lorestan.ir<br>
                    tourism@dorud-lorestan.ir<br>
                    contact@dorud-lorestan.ir</p>
                </div>
            </div>

            <!-- Contact Form -->
            <div class="contact-form glass-widget">
                <h3 style="text-align: center; margin-bottom: 2rem; color: #555;">فرم تماس</h3>
                <form onsubmit="submitForm(event)">
                    <div class="form-group">
                        <label for="name">نام و نام خانوادگی:</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">ایمیل:</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="phone">شماره تماس:</label>
                        <input type="tel" id="phone" name="phone">
                    </div>
                    <div class="form-group">
                        <label for="subject">موضوع:</label>
                        <select id="subject" name="subject" required>
                            <option value="">انتخاب کنید...</option>
                            <option value="tourism">اطلاعات گردشگری</option>
                            <option value="culture">فرهنگ و سنت‌ها</option>
                            <option value="events">رویدادها</option>
                            <option value="other">سایر موارد</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">پیام:</label>
                        <textarea id="message" name="message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="submit-btn">ارسال پیام</button>
                </form>
            </div>

            <!-- Developer Info Section -->
            <div class="contact-form glass-widget" style="margin-top: 3rem;">
                <h3 style="text-align: center; margin-bottom: 2rem; color: #555;">🚀 سازنده و توسعه‌دهنده</h3>
                <div style="display: flex; flex-direction: column; align-items: center; gap: 1.5rem;">
                    <div style="text-align: center;">
                        <div style="width: 120px; height: 120px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); border-radius: 50%; display: flex; align-items: center; justify-content: center; margin: 0 auto 1rem; font-size: 3rem; color: white; box-shadow: 0 10px 30px rgba(0,0,0,0.2);">
                            👨‍💻
                        </div>
                        <h4 style="margin: 0 0 0.5rem 0; font-size: 1.5rem; color: #333; font-weight: 700;">حسین گراوند</h4>
                        <p style="margin: 0 0 1rem 0; color: #666; font-size: 1rem;">توسعه‌دهنده فول‌استک • 19 ساله</p>
                        <div style="background: rgba(255,255,255,0.3); padding: 0.5rem 1rem; border-radius: 20px; display: inline-block; backdrop-filter: blur(10px);">
                            <span style="color: #555; font-weight: 600;">🎯 متخصص طراحی وب و تجربه کاربری</span>
                        </div>
                    </div>
                    
                    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem; width: 100%;">
                        <div class="feature-item" style="text-align: center;">
                            <span class="feature-icon">📱</span>
                            <div class="feature-title">تماس مستقیم</div>
                            <div class="feature-desc">
                                <a href="tel:09380856805" style="color: #4CAF50; text-decoration: none; font-weight: 600;">
                                    📞 09380856805
                                </a>
                            </div>
                        </div>
                        
                        <div class="feature-item" style="text-align: center;">
                            <span class="feature-icon">💬</span>
                            <div class="feature-title">تلگرام</div>
                            <div class="feature-desc">
                                <a href="https://t.me/HocenWO" target="_blank" rel="noopener noreferrer" style="color: #0088cc; text-decoration: none; font-weight: 600;">
                                    🔗 @HocenWO
                                </a>
                            </div>
                        </div>
                        
                        <div class="feature-item" style="text-align: center;">
                            <span class="feature-icon">📸</span>
                            <div class="feature-title">اینستاگرام</div>
                            <div class="feature-desc">
                                <a href="https://instagram.com/TraceOS" target="_blank" rel="noopener noreferrer" style="color: #E4405F; text-decoration: none; font-weight: 600;">
                                    🔗 @TraceOS
                                </a>
                            </div>
                        </div>
                    </div>
                    
                    <div style="text-align: center; background: rgba(255,255,255,0.2); padding: 1.5rem; border-radius: 20px; backdrop-filter: blur(10px); width: 100%;">
                        <h5 style="margin: 0 0 1rem 0; color: #333; font-size: 1.1rem;">💡 خدمات ارائه‌شده</h5>
                        <div style="display: flex; flex-wrap: wrap; gap: 0.5rem; justify-content: center;">
                            <span style="background: rgba(100,150,255,0.2); padding: 0.3rem 0.8rem; border-radius: 15px; font-size: 0.8rem; color: #333;">🌐 طراحی وب‌سایت</span>
                            <span style="background: rgba(100,150,255,0.2); padding: 0.3rem 0.8rem; border-radius: 15px; font-size: 0.8rem; color: #333;">📱 اپلیکیشن موبایل</span>
                            <span style="background: rgba(100,150,255,0.2); padding: 0.3rem 0.8rem; border-radius: 15px; font-size: 0.8rem; color: #333;">🎨 UI/UX Design</span>
                            <span style="background: rgba(100,150,255,0.2); padding: 0.3rem 0.8rem; border-radius: 15px; font-size: 0.8rem; color: #333;">⚡ بهینه‌سازی</span>
                            <span style="background: rgba(100,150,255,0.2); padding: 0.3rem 0.8rem; border-radius: 15px; font-size: 0.8rem; color: #333;">🔧 پشتیبانی فنی</span>
                        </div>
                        <p style="margin: 1rem 0 0 0; color: #666; font-size: 0.9rem; font-style: italic;">
                            "با تجربه در ساخت وب‌سایت‌های مدرن و کاربرپسند، آماده همکاری در پروژه‌های جدید هستم! 🚀"
                        </p>
                    </div>
                </div>
            </div>

            <!-- Map Section -->
            <div class="map-section glass-widget" style="margin-top: 3rem;">
                <h3 style="text-align: center; margin-bottom: 2rem; color: #555;">موقعیت جغرافیایی</h3>
                <div class="map-container" onclick="openMap()">
                    <div class="map-placeholder">🗺️</div>
                    <div class="map-text">دورود، لرستان - کلیک برای مشاهده در نقشه</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Interactive Widgets Section (Hidden by default, shown when needed) -->
    <div id="interactiveWidgets" style="display: none;">
        <!-- AI Chatbot Widget -->
        <div class="chatbot-widget glass-widget" id="chatbot">
            <div class="chatbot-header" onclick="toggleChatbot()">
                <span class="chatbot-icon">🤖</span>
                <span class="chatbot-title">راهنمای هوشمند دورود</span>
                <span class="chatbot-toggle" id="chatToggle">💬</span>
            </div>
            <div class="chatbot-body" id="chatbotBody">
                <div class="chat-messages" id="chatMessages">
                    <div class="bot-message">
                        <span class="message-avatar">🤖</span>
                        <div class="message-content">
                            سلام! من راهنمای هوشمند دورود هستم. چطور می‌تونم کمکتون کنم؟
                        </div>
                    </div>
                </div>
                <div class="quick-actions">
                    <button onclick="askBot('جاذبه‌های گردشگری')" class="quick-btn">🗻 جاذبه‌ها</button>
                    <button onclick="askBot('هتل و اقامت')" class="quick-btn">🏨 اقامت</button>
                    <button onclick="askBot('آب و هوا')" class="quick-btn">🌤️ آب و هوا</button>
                    <button onclick="askBot('غذاهای محلی')" class="quick-btn">🍲 غذا</button>
                </div>
                <div class="chat-input">
                    <input type="text" id="chatInput" placeholder="سوال خود را بپرسید..." onkeypress="handleChatEnter(event)">
                    <button onclick="sendMessage()" class="send-btn">📤</button>
                </div>
            </div>
        </div>

        <!-- Virtual Tour Widget -->
        <div class="vr-tour-widget glass-widget" id="vrTour">
            <div class="vr-header">
                <h4>🥽 تور مجازی 360°</h4>
                <button class="vr-close" onclick="closeVRTour()">✕</button>
            </div>
            <div class="vr-content">
                <div class="vr-viewer" id="vrViewer">
                    <div class="vr-scene active" data-scene="mountain">
                        <div class="vr-panorama">🏔️</div>
                        <div class="vr-hotspots">
                            <div class="hotspot" style="top: 30%; left: 20%;" onclick="showHotspotInfo('قله اشترانکوه')">📍</div>
                            <div class="hotspot" style="top: 60%; left: 70%;" onclick="showHotspotInfo('جنگل بلوط')">📍</div>
                        </div>
                    </div>
                </div>
                <div class="vr-controls">
                    <button onclick="changeVRScene('mountain')" class="vr-btn active">🏔️ کوهستان</button>
                    <button onclick="changeVRScene('forest')" class="vr-btn">🌲 جنگل</button>
                    <button onclick="changeVRScene('waterfall')" class="vr-btn">💧 آبشار</button>
                    <button onclick="changeVRScene('cave')" class="vr-btn">🕳️ غار</button>
                </div>
            </div>
        </div>

        <!-- Live Info Widget -->
        <div class="live-info-widget glass-widget" id="liveInfo">
            <div class="live-tabs">
                <button class="tab-btn active" onclick="showLiveTab('traffic')">🚗 ترافیک</button>
                <button class="tab-btn" onclick="showLiveTab('events')">📅 رویدادها</button>
                <button class="tab-btn" onclick="showLiveTab('news')">📰 اخبار</button>
            </div>
            <div class="live-content">
                <div class="live-tab active" id="traffic">
                    <div class="traffic-item">
                        <span class="traffic-status green">🟢</span>
                        <span>جاده دورود - خرم‌آباد</span>
                        <span class="traffic-time">روان</span>
                    </div>
                    <div class="traffic-item">
                        <span class="traffic-status yellow">🟡</span>
                        <span>جاده دورود - بروجرد</span>
                        <span class="traffic-time">نیمه‌سنگین</span>
                    </div>
                    <div class="traffic-item">
                        <span class="traffic-status green">🟢</span>
                        <span>جاده دورود - اراک</span>
                        <span class="traffic-time">روان</span>
                    </div>
                </div>
                <div class="live-tab" id="events">
                    <div class="event-item">
                        <span class="event-date">امروز</span>
                        <span>نمایشگاه صنایع دستی</span>
                        <span class="event-time">14:00</span>
                    </div>
                    <div class="event-item">
                        <span class="event-date">فردا</span>
                        <span>کنسرت موسیقی محلی</span>
                        <span class="event-time">19:30</span>
                    </div>
                </div>
                <div class="live-tab" id="news">
                    <div class="news-item">
                        <span class="news-time">2 ساعت پیش</span>
                        <span>افتتاح مسیر جدید کوهنوردی</span>
                    </div>
                    <div class="news-item">
                        <span class="news-time">5 ساعت پیش</span>
                        <span>جشنواره عکاسی طبیعت آغاز شد</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- Audio Player for Nature Sounds -->
        <div class="audio-player glass-widget" id="audioPlayer">
            <div class="audio-header">
                <h4>🎵 صداهای طبیعت دورود</h4>
                <button class="audio-toggle" onclick="toggleAudioPlayer()">🎧</button>
            </div>
            <div class="audio-content" id="audioContent">
                <div class="audio-track active">
                    <span class="track-icon">🌊</span>
                    <span class="track-name">صدای آبشار</span>
                    <button class="play-btn" onclick="playTrack('waterfall')">▶️</button>
                </div>
                <div class="audio-track">
                    <span class="track-icon">🦅</span>
                    <span class="track-name">آواز پرندگان</span>
                    <button class="play-btn" onclick="playTrack('birds')">▶️</button>
                </div>
                <div class="audio-track">
                    <span class="track-icon">🌲</span>
                    <span class="track-name">صدای جنگل</span>
                    <button class="play-btn" onclick="playTrack('forest')">▶️</button>
                </div>
                <div class="audio-track">
                    <span class="track-icon">💨</span>
                    <span class="track-name">صدای باد کوهستان</span>
                    <button class="play-btn" onclick="playTrack('wind')">▶️</button>
                </div>
                <div class="audio-controls">
                    <button onclick="stopAllTracks()">⏹️ توقف</button>
                    <input type="range" class="volume-slider" min="0" max="100" value="50" onchange="setVolume(this.value)">
                    <span>🔊</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Floating Chatbot Widget -->
    <div class="chatbot-widget glass-widget" id="floatingChatbot" style="position: fixed; bottom: 20px; right: 20px; width: 350px; z-index: 1000; display: block;">
        <div class="chatbot-header" onclick="toggleFloatingChatbot()">
            <span class="chatbot-icon">🤖</span>
            <span class="chatbot-title">راهنمای هوشمند دورود</span>
            <span class="chatbot-toggle" id="floatingChatToggle">💬</span>
        </div>
        <div class="chatbot-body" id="floatingChatbotBody">
            <div class="chat-messages" id="floatingChatMessages">
                <div class="bot-message">
                    <span class="message-avatar">🤖</span>
                    <div class="message-content">
                        سلام! من راهنمای هوشمند دورود هستم. چطور می‌تونم کمکتون کنم؟
                    </div>
                </div>
            </div>
            <div class="quick-actions">
                <button onclick="askFloatingBot('جاذبه‌های گردشگری')" class="quick-btn">🗻 جاذبه‌ها</button>
                <button onclick="askFloatingBot('هتل و اقامت')" class="quick-btn">🏨 اقامت</button>
                <button onclick="askFloatingBot('آب و هوا')" class="quick-btn">🌤️ آب و هوا</button>
                <button onclick="askFloatingBot('غذاهای محلی')" class="quick-btn">🍲 غذا</button>
            </div>
            <div class="chat-input">
                <input type="text" id="floatingChatInput" placeholder="سوال خود را بپرسید..." onkeypress="handleFloatingChatEnter(event)">
                <button onclick="sendFloatingMessage()" class="send-btn">📤</button>
            </div>
        </div>
    </div>

    <!-- Card Dialog Modal -->
    <div class="card-dialog" id="cardDialog">
        <div class="dialog-content">
            <div class="dialog-header">
                <span class="dialog-icon" id="dialogIcon">🏔️</span>
                <h3 class="dialog-title" id="dialogTitle">عنوان کارت</h3>
                <button class="dialog-close" onclick="closeCardDialog()">✕</button>
            </div>
            <div class="dialog-body">
                <div class="dialog-description" id="dialogDescription">
                    توضیحات تفصیلی در اینجا نمایش داده می‌شود.
                </div>
                <div class="dialog-features" id="dialogFeatures">
                    <!-- Features will be populated by JavaScript -->
                </div>
                <div class="dialog-actions" id="dialogActions">
                    <!-- Action buttons will be populated by JavaScript -->
                </div>
            </div>
        </div>
    </div>

    <!-- Scroll to Top Button -->
    <button class="scroll-to-top" id="scrollToTop" onclick="scrollToTop()">↑</button>

    <script>
        // Navigation functionality
        function showPage(pageId) {
            // Hide all pages
            const pages = document.querySelectorAll('.page');
            pages.forEach(page => page.classList.remove('active'));
            
            // Show selected page
            document.getElementById(pageId).classList.add('active');
            
            // Update navigation
            const navItems = document.querySelectorAll('.nav-item');
            navItems.forEach(item => item.classList.remove('active'));
            document.getElementById(`nav-${pageId}`).classList.add('active');
            
            // Close mobile menu
            document.getElementById('navMenu').classList.remove('active');
            
            // Scroll to top
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function toggleMobileMenu() {
            const navMenu = document.getElementById('navMenu');
            navMenu.classList.toggle('active');
        }

        // Navbar scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            const scrollToTop = document.getElementById('scrollToTop');
            
            if (window.scrollY > 100) {
                navbar.classList.add('scrolled');
                scrollToTop.classList.add('show');
            } else {
                navbar.classList.remove('scrolled');
                scrollToTop.classList.remove('show');
            }
        });

        // Scroll to top function
        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Weather widget animation
        function updateWeather() {
            const temps = [18, 19, 20, 21, 22, 23, 24, 25];
            const temp = temps[Math.floor(Math.random() * temps.length)];
            document.getElementById('temperature').textContent = temp + '°C';
        }

        // Update weather every 30 seconds
        setInterval(updateWeather, 30000);

        // Map function
        function openMap() {
            const url = 'https://www.google.com/maps/place/Dorud,+Lorestan+Province,+Iran/@33.4969,49.0519,12z';
            window.open(url, '_blank', 'noopener,noreferrer');
        }

        // Form submission
        function submitForm(event) {
            event.preventDefault();
            
            const submitBtn = event.target.querySelector('.submit-btn');
            const originalText = submitBtn.textContent;
            
            submitBtn.innerHTML = '<span class="loading"></span> در حال ارسال...';
            submitBtn.disabled = true;
            
            // Simulate form submission
            setTimeout(() => {
                alert('پیام شما با موفقیت ارسال شد. به زودی با شما تماس خواهیم گرفت.');
                event.target.reset();
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            }, 2000);
        }

        // Eco-tourism form submission
        function submitEcoTourForm(event) {
            event.preventDefault();
            
            const submitBtn = event.target.querySelector('.submit-btn');
            const originalText = submitBtn.textContent;
            const tourType = document.getElementById('ecoTourType').value;
            const tourDate = document.getElementById('ecoTourDate').value;
            const participants = document.getElementById('ecoParticipants').value;
            
            submitBtn.innerHTML = '<span class="loading"></span> در حال ارسال درخواست...';
            submitBtn.disabled = true;
            
            // Simulate form submission
            setTimeout(() => {
                const tourNames = {
                    'oneday': 'تور یک‌روزه طبیعت',
                    'camping': 'کمپ اکولوژیک 3 روزه',
                    'weekly': 'بوم‌گردی هفتگی',
                    'educational': 'تور آموزشی دانشجویی'
                };
                
                alert(`🌿 درخواست رزرو شما ثبت شد!\n\n📋 جزئیات:\n• تور: ${tourNames[tourType]}\n• تاریخ: ${tourDate}\n• تعداد: ${participants}\n\n✅ کارشناسان اکوتوریسم دورود تا 24 ساعت آینده با شما تماس خواهند گرفت.\n\n🙏 از انتخاب گردشگری پایدار متشکریم!`);
                event.target.reset();
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            }, 2500);
        }

        // Animate statistics on scroll
        function animateStats() {
            const stats = document.querySelectorAll('.stat-number');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        const target = entry.target;
                        const finalValue = target.textContent;
                        const numericValue = parseInt(finalValue.replace(/[^\d]/g, ''));
                        
                        if (numericValue) {
                            let current = 0;
                            const increment = numericValue / 50;
                            const timer = setInterval(() => {
                                current += increment;
                                if (current >= numericValue) {
                                    target.textContent = finalValue;
                                    clearInterval(timer);
                                } else {
                                    target.textContent = Math.floor(current).toLocaleString();
                                }
                            }, 30);
                        }
                        
                        observer.unobserve(target);
                    }
                });
            });
            
            stats.forEach(stat => observer.observe(stat));
        }

        // Initialize animations when page loads
        document.addEventListener('DOMContentLoaded', function() {
            animateStats();
            
            // Add click handlers for gallery items
            const galleryItems = document.querySelectorAll('.gallery-item');
            galleryItems.forEach(item => {
                item.addEventListener('click', function() {
                    this.style.transform = 'scale(1.1) rotate(5deg)';
                    setTimeout(() => {
                        this.style.transform = '';
                    }, 300);
                });
            });
        });

        // Close mobile menu when clicking outside
        document.addEventListener('click', function(event) {
            const navMenu = document.getElementById('navMenu');
            const mobileBtn = document.querySelector('.mobile-menu-btn');
            
            if (!navMenu.contains(event.target) && !mobileBtn.contains(event.target)) {
                navMenu.classList.remove('active');
            }
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add loading animation to buttons
        document.querySelectorAll('button, .cta-button').forEach(btn => {
            btn.addEventListener('click', function() {
                if (!this.classList.contains('loading')) {
                    this.style.transform = 'scale(0.95)';
                    setTimeout(() => {
                        this.style.transform = '';
                    }, 150);
                }
            });
        });

        // Floating Chatbot functionality
        let floatingChatbotOpen = false;
        
        function toggleFloatingChatbot() {
            const chatbot = document.getElementById('floatingChatbot');
            floatingChatbotOpen = !floatingChatbotOpen;
            
            if (floatingChatbotOpen) {
                chatbot.classList.add('open');
                document.getElementById('floatingChatToggle').textContent = '🔽';
            } else {
                chatbot.classList.remove('open');
                document.getElementById('floatingChatToggle').textContent = '💬';
            }
        }

        function askFloatingBot(question) {
            addFloatingUserMessage(question);
            
            setTimeout(() => {
                let response = '';
                switch(question) {
                    case 'جاذبه‌های گردشگری':
                        response = 'دورود دارای جاذبه‌های فوق‌العاده‌ای مثل قله اشترانکوه، آبشار بیشه‌لو، غار علیصدر و جنگل‌های زاگرس است. کدام یک را می‌خواهید بیشتر بدانید؟';
                        break;
                    case 'هتل و اقامت':
                        response = 'در دورود اقامتگاه‌های بوم‌گردی، هتل‌های محلی و کمپینگ‌های طبیعی وجود دارد. بهترین زمان رزرو فصل بهار و تابستان است.';
                        break;
                    case 'آب و هوا':
                        response = 'آب و هوای دورود کوهستانی و معتدل است. بهار و تابستان بهترین فصل برای سفر، زمستان برفی و سرد است.';
                        break;
                    case 'غذاهای محلی':
                        response = 'غذاهای محلی دورود شامل کباب کوبیده لری، آش دوغ، کشک و بادمجان، و انواع نان‌های سنتی است. حتماً امتحان کنید!';
                        break;
                    default:
                        response = 'سوال جالبی پرسیدید! برای اطلاعات دقیق‌تر می‌تونید با اداره گردشگری دورود تماس بگیرید یا از منوهای سایت استفاده کنید.';
                }
                addFloatingBotMessage(response);
            }, 1000);
        }

        function sendFloatingMessage() {
            const input = document.getElementById('floatingChatInput');
            const message = input.value.trim();
            
            if (message) {
                addFloatingUserMessage(message);
                input.value = '';
                
                setTimeout(() => {
                    // Simple keyword-based responses
                    let response = '';
                    const lowerMessage = message.toLowerCase();
                    
                    if (lowerMessage.includes('هتل') || lowerMessage.includes('اقامت')) {
                        response = '🏨 برای رزرو هتل، بودجه و تاریخ سفرتون رو بگید تا بهترین گزینه‌ها رو معرفی کنم!';
                    } else if (lowerMessage.includes('غذا') || lowerMessage.includes('رستوران')) {
                        response = '🍲 رستوران‌های محلی دورود غذاهای فوق‌العاده‌ای دارن! کباب لری و آش دوغ حتماً امتحان کنید!';
                    } else if (lowerMessage.includes('قیمت') || lowerMessage.includes('هزینه')) {
                        response = '💰 هزینه‌های سفر به دورود معقول هستند. اقامت از 500 هزار تومان شروع می‌شود.';
                    } else if (lowerMessage.includes('زمان') || lowerMessage.includes('فصل')) {
                        response = '🌸 بهترین زمان سفر به دورود بهار و تابستانه! هوا معتدل و طبیعت سرسبزه.';
                    } else {
                        response = '😊 ممنون از پیامتون! برای پاسخ بهتر از دکمه‌های بالا استفاده کنید یا سوال مشخص‌تری بپرسید.';
                    }
                    
                    addFloatingBotMessage(response);
                }, 1500);
            }
        }

        function handleFloatingChatEnter(event) {
            if (event.key === 'Enter') {
                sendFloatingMessage();
            }
        }

        function addFloatingUserMessage(message) {
            const chatMessages = document.getElementById('floatingChatMessages');
            const messageDiv = document.createElement('div');
            messageDiv.className = 'user-message';
            messageDiv.innerHTML = `
                <span class="message-avatar">👤</span>
                <div class="message-content">${message}</div>
            `;
            chatMessages.appendChild(messageDiv);
            chatMessages.scrollTop = chatMessages.scrollHeight;
        }

        function addFloatingBotMessage(message) {
            const chatMessages = document.getElementById('floatingChatMessages');
            const messageDiv = document.createElement('div');
            messageDiv.className = 'bot-message';
            messageDiv.innerHTML = `
                <span class="message-avatar">🤖</span>
                <div class="message-content">${message}</div>
            `;
            chatMessages.appendChild(messageDiv);
            chatMessages.scrollTop = chatMessages.scrollHeight;
        }

        // VR Tour functionality
        function openVRTour() {
            document.getElementById('vrTour').classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeVRTour() {
            document.getElementById('vrTour').classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        function changeVRScene(scene) {
            // Remove active class from all scenes and buttons
            document.querySelectorAll('.vr-scene').forEach(s => s.classList.remove('active'));
            document.querySelectorAll('.vr-btn').forEach(b => b.classList.remove('active'));
            
            // Add active class to selected scene and button
            document.querySelector(`[data-scene="${scene}"]`).classList.add('active');
            event.target.classList.add('active');
            
            // Update panorama content based on scene
            const panorama = document.querySelector('.vr-scene.active .vr-panorama');
            const hotspots = document.querySelector('.vr-scene.active .vr-hotspots');
            
            switch(scene) {
                case 'mountain':
                    panorama.textContent = '🏔️';
                    hotspots.innerHTML = `
                        <div class="hotspot" style="top: 30%; left: 20%;" onclick="showHotspotInfo('قله اشترانکوه')">📍</div>
                        <div class="hotspot" style="top: 60%; left: 70%;" onclick="showHotspotInfo('جنگل بلوط')">📍</div>
                    `;
                    break;
                case 'forest':
                    panorama.textContent = '🌲';
                    hotspots.innerHTML = `
                        <div class="hotspot" style="top: 40%; left: 30%;" onclick="showHotspotInfo('درختان بلوط')">📍</div>
                        <div class="hotspot" style="top: 70%; left: 60%;" onclick="showHotspotInfo('چشمه جنگلی')">📍</div>
                    `;
                    break;
                case 'waterfall':
                    panorama.textContent = '💧';
                    hotspots.innerHTML = `
                        <div class="hotspot" style="top: 25%; left: 50%;" onclick="showHotspotInfo('آبشار بیشه‌لو')">📍</div>
                        <div class="hotspot" style="top: 80%; left: 40%;" onclick="showHotspotInfo('استخر طبیعی')">📍</div>
                    `;
                    break;
                case 'cave':
                    panorama.textContent = '🕳️';
                    hotspots.innerHTML = `
                        <div class="hotspot" style="top: 35%; left: 45%;" onclick="showHotspotInfo('غار علیصدر')">📍</div>
                        <div class="hotspot" style="top: 65%; left: 25%;" onclick="showHotspotInfo('دریاچه زیرزمینی')">📍</div>
                    `;
                    break;
            }
        }

        function showHotspotInfo(location) {
            alert(`📍 ${location}\n\nاطلاعات تفصیلی درباره این مکان در نسخه کامل تور مجازی موجود است.`);
        }

        // Live Info Widget functionality
        function showLiveTab(tabName) {
            // Remove active class from all tabs and buttons
            document.querySelectorAll('.live-tab').forEach(tab => tab.classList.remove('active'));
            document.querySelectorAll('.tab-btn').forEach(btn => btn.classList.remove('active'));
            
            // Add active class to selected tab and button
            document.getElementById(tabName).classList.add('active');
            event.target.classList.add('active');
        }

        // Audio Player functionality
        let audioPlayerOpen = false;
        let currentTrack = null;
        
        function toggleAudioPlayer() {
            const audioPlayer = document.getElementById('audioPlayer');
            audioPlayerOpen = !audioPlayerOpen;
            
            if (audioPlayerOpen) {
                audioPlayer.classList.add('open');
            } else {
                audioPlayer.classList.remove('open');
            }
        }

        function playTrack(trackName) {
            // Remove active class from all tracks
            document.querySelectorAll('.audio-track').forEach(track => track.classList.remove('active'));
            
            // Add active class to selected track
            event.target.closest('.audio-track').classList.add('active');
            
            // Update play buttons
            document.querySelectorAll('.play-btn').forEach(btn => btn.textContent = '▶️');
            event.target.textContent = '⏸️';
            
            currentTrack = trackName;
            
            // Show playing message
            setTimeout(() => {
                alert(`🎵 در حال پخش: ${getTrackName(trackName)}\n\nنوت: در نسخه کامل، صداهای واقعی طبیعت پخش خواهد شد.`);
            }, 500);
        }

        function stopAllTracks() {
            document.querySelectorAll('.audio-track').forEach(track => track.classList.remove('active'));
            document.querySelectorAll('.play-btn').forEach(btn => btn.textContent = '▶️');
            currentTrack = null;
        }

        function setVolume(value) {
            // In a real implementation, this would control actual audio volume
            console.log(`Volume set to: ${value}%`);
        }

        function getTrackName(trackName) {
            const trackNames = {
                'waterfall': 'صدای آبشار',
                'birds': 'آواز پرندگان',
                'forest': 'صدای جنگل',
                'wind': 'صدای باد کوهستان'
            };
            return trackNames[trackName] || trackName;
        }

        // Enhanced weather updates
        function updateLiveWeather() {
            const temps = [18, 19, 20, 21, 22, 23, 24, 25];
            const winds = ['10 km/h', '12 km/h', '8 km/h', '15 km/h', '11 km/h'];
            const humidity = [60, 62, 65, 68, 70, 72, 75];
            const visibility = ['12 km', '15 km', '18 km', '20 km', '10 km'];
            
            document.getElementById('liveTemp').textContent = temps[Math.floor(Math.random() * temps.length)] + '°C';
            document.getElementById('liveWind').textContent = winds[Math.floor(Math.random() * winds.length)];
            document.getElementById('liveHumidity').textContent = humidity[Math.floor(Math.random() * humidity.length)] + '%';
            document.getElementById('liveVisibility').textContent = visibility[Math.floor(Math.random() * visibility.length)];
        }

        // Update live weather every 45 seconds
        setInterval(updateLiveWeather, 45000);

        // Gallery functionality
        function showGalleryCategory(category) {
            // Remove active class from all buttons
            document.querySelectorAll('.gallery-cat-btn').forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');
            
            // Show/hide gallery items based on category
            const galleryItems = document.querySelectorAll('.gallery-item');
            galleryItems.forEach(item => {
                if (category === 'all' || item.dataset.category === category) {
                    item.style.display = 'flex';
                    item.style.animation = 'fadeInUp 0.5s ease-out';
                } else {
                    item.style.display = 'none';
                }
            });
        }

        function openImageModal(title, emoji) {
            const modal = document.getElementById('imageModal');
            const modalTitle = document.getElementById('modalTitle');
            const modalImage = document.getElementById('modalImage');
            const modalDescription = document.getElementById('modalDescription');
            
            modalTitle.textContent = title;
            modalImage.textContent = emoji;
            
            // Set description based on title
            const descriptions = {
                'کوه‌های زاگرس': 'رشته کوه‌های مرتفع زاگرس با قله‌های برفی و مناظر خیره‌کننده که محل زندگی گونه‌های کمیاب حیوانات و گیاهان است.',
                'آبشار بیشه‌لو': 'یکی از زیباترین آبشارهای ایران با ارتفاع 48 متر که در فصل بهار و تابستان منظره‌ای خیره‌کننده دارد.',
                'جنگل‌های پاییزی': 'جنگل‌های بلوط که در پاییز رنگ‌های طلایی و قرمز زیبایی خلق می‌کنند.',
                'غار علیصدر': 'بزرگترین غار آبی جهان که با قایق‌های کوچک قابل بازدید است و از عجایب طبیعی ایران محسوب می‌شود.',
                'چشمه گرماب': 'چشمه آب گرم طبیعی با خواص درمانی که برای درمان بیماری‌های پوستی و مفصلی استفاده می‌شود.',
                'بهار کوهستان': 'شکوفه‌های بهاری که کوهستان‌های دورود را به باغی از رنگ‌ها و عطرها تبدیل می‌کنند.',
                'روستای بر افتاب': 'روستایی زیبا در دامنه کوه‌های زاگرس که نام آن از موقعیت خاصش در برابر نور خورشید گرفته شده.',
                'روستای دربند': 'روستای کوهستانی با معماری سنتی و خانه‌های پلکانی که آب و هوای خنک و طبیعت بکر دارد.',
                'روستای پیر عبدالله': 'روستای تاریخی با بقعه مقدس پیر عبدالله که مرکز زیارت و معنویت منطقه محسوب می‌شود.'
            };
            
            modalDescription.textContent = descriptions[title] || 'توضیحات تفصیلی درباره این تصویر زیبا از دورود.';
            
            modal.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeImageModal() {
            const modal = document.getElementById('imageModal');
            modal.classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        function shareImage() {
            const title = document.getElementById('modalTitle').textContent;
            if (navigator.share) {
                navigator.share({
                    title: `${title} - دورود لرستان`,
                    text: `تصویر زیبای ${title} از شهرستان دورود`,
                    url: window.location.href
                });
            } else {
                // Fallback for browsers that don't support Web Share API
                const url = window.location.href;
                navigator.clipboard.writeText(`${title} - دورود لرستان: ${url}`);
                alert('لینک کپی شد! می‌توانید آن را در شبکه‌های اجتماعی به اشتراک بگذارید.');
            }
        }

        function downloadImage() {
            alert('در نسخه کامل، امکان دانلود تصاویر با کیفیت بالا فراهم خواهد بود.');
        }

        function setWallpaper() {
            alert('این تصویر زیبا می‌تواند تصویر زمینه عالی برای دستگاه شما باشد!');
        }

        // New Technology Functions
        function openSmartGuide() {
            alert('📱 اپلیکیشن موبایل دورود\n\n• نقشه آفلاین کامل منطقه\n• راهنمای صوتی به 5 زبان\n• رزرو آنلاین هتل و تور\n• پیش‌بینی آب و هوا\n• کامپاس و GPS کوهستان\n• اطلاعات اضطراری\n\nبه زودی در App Store و Google Play!');
        }

        function openQRTour() {
            alert('📷 تور QR کد\n\n• اسکن کد در هر جاذبه\n• اطلاعات فوری و تصاویر\n• راهنمای صوتی\n• نقشه مسیر\n• تاریخچه و داستان‌ها\n• امکان اشتراک‌گذاری\n\nکدهای QR در تمام نقاط نصب شده!');
        }

        function openDroneView() {
            alert('🚁 نمای پهپادی زنده\n\n• تصاویر زنده از قله اشترانکوه\n• وضعیت ترافیک جاده‌ها\n• شرایط آب و هوایی\n• نظارت بر حیات وحش\n• کنترل آتش‌سوزی جنگل\n\nدوربین‌های 4K با پخش زنده!');
        }

        function openAIPlanner() {
            alert('🧠 برنامه‌ریز هوشمند\n\n• تحلیل علایق شخصی\n• بهینه‌سازی مسیر\n• پیشنهاد بودجه\n• رزرو خودکار\n• هشدارهای هوشمند\n• تطبیق با آب و هوا\n\nهوش مصنوعی پیشرفته برای بهترین تجربه!');
        }

        // Widget management functions
        function showLiveInfo() {
            const widgetsContainer = document.getElementById('interactiveWidgets');
            const liveInfoWidget = document.getElementById('liveInfo');
            
            widgetsContainer.style.display = 'block';
            liveInfoWidget.style.position = 'fixed';
            liveInfoWidget.style.bottom = '20px';
            liveInfoWidget.style.left = '20px';
            liveInfoWidget.style.zIndex = '1000';
            liveInfoWidget.style.display = 'block';
        }



        function toggleAudioPlayer() {
            const widgetsContainer = document.getElementById('interactiveWidgets');
            const audioPlayer = document.getElementById('audioPlayer');
            
            widgetsContainer.style.display = 'block';
            audioPlayer.style.position = 'fixed';
            audioPlayer.style.top = '50%';
            audioPlayer.style.right = '20px';
            audioPlayer.style.transform = 'translateY(-50%)';
            audioPlayer.style.zIndex = '1000';
            audioPlayer.style.display = 'block';
            
            audioPlayerOpen = !audioPlayerOpen;
            
            if (audioPlayerOpen) {
                audioPlayer.classList.add('open');
            } else {
                audioPlayer.classList.remove('open');
            }
        }

        function openVRTour() {
            const widgetsContainer = document.getElementById('interactiveWidgets');
            const vrTour = document.getElementById('vrTour');
            
            widgetsContainer.style.display = 'block';
            vrTour.style.position = 'fixed';
            vrTour.style.top = '50%';
            vrTour.style.left = '50%';
            vrTour.style.transform = 'translate(-50%, -50%)';
            vrTour.style.zIndex = '1001';
            vrTour.style.display = 'block';
            vrTour.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        // Chatbot Page Functions
        function sendQuickMessage(message) {
            addChatbotUserMessage(message);
            
            setTimeout(() => {
                let response = '';
                switch(message) {
                    case 'جاذبه‌های گردشگری دورود':
                        response = '🗻 <strong>جاذبه‌های برتر دورود:</strong><br><br>• قله اشترانکوه (4050 متر) - کوهنوردی<br>• آبشار بیشه‌لو (48 متر) - طبیعت‌گردی<br>• غار علیصدر - بزرگترین غار آبی جهان<br>• چشمه گرماب - آب‌درمانی<br>• جنگل‌های زاگرس - پیاده‌روی<br>• پل کشکان - میراث تاریخی<br><br>کدام یک را بیشتر می‌خواهید بدانید؟ 😊';
                        break;
                    case 'هتل‌های دورود':
                        response = '🏨 <strong>اقامتگاه‌های دورود:</strong><br><br>• هتل کوهستان - 4 ستاره، مرکز شهر<br>• اقامتگاه بوم‌گردی بر افتاب - تجربه روستایی<br>• کمپینگ طبیعت - زیر ستاره‌ها<br>• هتل آپارتمان زاگرس - خانوادگی<br>• اقامتگاه سنتی دربند - معماری محلی<br><br>بودجه و تاریخ سفرتون چیه تا بهترین گزینه رو پیشنهاد بدم؟ 🏠';
                        break;
                    case 'غذاهای محلی':
                        response = '🍲 <strong>غذاهای اصیل دورود:</strong><br><br>• کباب کوبیده لری - با گوشت محلی<br>• آش دوغ - سوپ سنتی<br>• کشک و بادمجان - پیش‌غذای محبوب<br>• نان تنوری - تازه از تنور<br>• پنیر و کشک محلی - از شیر طبیعی<br>• دمی گوشت کوهی - غذای اصیل<br><br>کدوم رستوران رو می‌خواید معرفی کنم؟ 😋';
                        break;
                    case 'آب و هوای دورود':
                        response = '🌤️ <strong>آب و هوای دورود:</strong><br><br>• بهار: 15-25°C - بهترین فصل سفر 🌸<br>• تابستان: 20-30°C - مناسب کوهنوردی ☀️<br>• پاییز: 10-20°C - رنگ‌های زیبا 🍂<br>• زمستان: -5 تا 10°C - برفی و سرد ❄️<br><br>الان دمای هوا 22 درجه و آفتابیه! بهترین زمان برای بازدید از جاذبه‌هاست. 😊';
                        break;
                    case 'برنامه سفر 3 روزه':
                        response = '📅 <strong>برنامه سفر 3 روزه:</strong><br><br><strong>روز اول:</strong><br>• صبح: ورود و اسکان در هتل<br>• ظهر: بازدید از مرکز شهر و بازار<br>• عصر: آبشار بیشه‌لو<br><br><strong>روز دوم:</strong><br>• صبح: صعود به قله اشترانکوه<br>• ظهر: ناهار در طبیعت<br>• عصر: بازدید از روستای بر افتاب<br><br><strong>روز سوم:</strong><br>• صبح: غار علیصدر<br>• ظهر: چشمه گرماب<br>• عصر: خرید سوغات و بازگشت<br><br>نیاز به جزئیات بیشتر دارید؟ 🗺️';
                        break;
                    case 'مسیر به دورود':
                        response = '🗺️ <strong>مسیرهای دسترسی:</strong><br><br><strong>از تهران:</strong><br>• جاده: 380 کیلومتر (5 ساعت)<br>• اتوبوس: ترمینال جنوب<br><br><strong>از اصفهان:</strong><br>• جاده: 280 کیلومتر (4 ساعت)<br><br><strong>از خرم‌آباد:</strong><br>• جاده: 120 کیلومتر (2 ساعت)<br><br>بهترین مسیر از کدوم شهر می‌خواید؟ راهنمایی دقیق‌تر می‌دم! 🚗';
                        break;
                    default:
                        response = 'سوال جالبی پرسیدید! 😊 برای اطلاعات دقیق‌تر از دکمه‌های بالا استفاده کنید یا سوال مشخص‌تری بپرسید.';
                }
                addChatbotBotMessage(response);
            }, 1000);
        }

        function sendChatbotMessage() {
            const input = document.getElementById('chatbotInput');
            const message = input.value.trim();
            
            if (message) {
                addChatbotUserMessage(message);
                input.value = '';
                
                setTimeout(() => {
                    // Simple keyword-based responses
                    let response = '';
                    const lowerMessage = message.toLowerCase();
                    
                    if (lowerMessage.includes('هتل') || lowerMessage.includes('اقامت')) {
                        response = '🏨 برای رزرو هتل، بودجه و تاریخ سفرتون رو بگید تا بهترین گزینه‌ها رو معرفی کنم!';
                    } else if (lowerMessage.includes('غذا') || lowerMessage.includes('رستوران')) {
                        response = '🍲 رستوران‌های محلی دورود غذاهای فوق‌العاده‌ای دارن! کباب لری و آش دوغ حتماً امتحان کنید!';
                    } else if (lowerMessage.includes('قیمت') || lowerMessage.includes('هزینه')) {
                        response = '💰 هزینه‌های سفر به دورود:\n• اقامت: 500-2000 هزار تومان\n• غذا: 100-300 هزار تومان\n• جاذبه‌ها: رایگان تا 50 هزار تومان';
                    } else if (lowerMessage.includes('زمان') || lowerMessage.includes('فصل')) {
                        response = '🌸 بهترین زمان سفر به دورود بهار و تابستانه! هوا معتدل و طبیعت سرسبزه.';
                    } else {
                        response = '😊 ممنون از پیامتون! برای پاسخ بهتر از دکمه‌های بالا استفاده کنید یا سوال مشخص‌تری بپرسید.';
                    }
                    
                    addChatbotBotMessage(response);
                }, 1500);
            }
        }

        function handleChatbotEnter(event) {
            if (event.key === 'Enter') {
                sendChatbotMessage();
            }
        }

        function addChatbotUserMessage(message) {
            const chatInterface = document.getElementById('chatInterface');
            const messageDiv = document.createElement('div');
            messageDiv.style.cssText = 'display: flex; align-items: flex-start; gap: 0.5rem; margin-bottom: 1rem; flex-direction: row-reverse;';
            messageDiv.innerHTML = `
                <span style="font-size: 2rem;">👤</span>
                <div style="background: rgba(100,150,255,0.2); padding: 1rem; border-radius: 15px; flex: 1; text-align: right;">
                    ${message}
                </div>
            `;
            chatInterface.appendChild(messageDiv);
            chatInterface.scrollTop = chatInterface.scrollHeight;
        }

        function addChatbotBotMessage(message) {
            const chatInterface = document.getElementById('chatInterface');
            const messageDiv = document.createElement('div');
            messageDiv.style.cssText = 'display: flex; align-items: flex-start; gap: 0.5rem; margin-bottom: 1rem;';
            messageDiv.innerHTML = `
                <span style="font-size: 2rem;">🤖</span>
                <div style="background: rgba(255,255,255,0.2); padding: 1rem; border-radius: 15px; flex: 1;">
                    ${message}
                </div>
            `;
            chatInterface.appendChild(messageDiv);
            chatInterface.scrollTop = chatInterface.scrollHeight;
        }

        // New Section Functions
        function openOnlineShop(category) {
            const categories = {
                'souvenirs': {
                    title: 'سوغات و صنایع دستی',
                    items: '• گلیم دست‌باف - 2.5 میلیون تومان\n• سفال سنتی - 350 هزار تومان\n• چوب‌تراشی - 180 هزار تومان\n• جاجیم محلی - 1.8 میلیون تومان'
                },
                'organic': {
                    title: 'محصولات ارگانیک',
                    items: '• گردو درجه یک - 120 هزار تومان/کیلو\n• عسل طبیعی - 85 هزار تومان/کیلو\n• پنیر محلی - 45 هزار تومان/کیلو\n• کشک خشک - 35 هزار تومان/کیلو'
                },
                'books': {
                    title: 'کتاب و نقشه',
                    items: '• راهنمای گردشگری دورود - 65 هزار تومان\n• نقشه کوهنوردی - 25 هزار تومان\n• کتاب فرهنگ لری - 45 هزار تومان\n• آلبوم عکس - 85 هزار تومان'
                },
                'clothing': {
                    title: 'پوشاک محلی',
                    items: '• لباس سنتی لری - 850 هزار تومان\n• کلاه محلی - 120 هزار تومان\n• شال دست‌باف - 180 هزار تومان\n• تی‌شرت یادگاری - 45 هزار تومان'
                }
            };
            
            const cat = categories[category];
            alert(`🛍️ ${cat.title}\n\n${cat.items}\n\n📦 ارسال رایگان به سراسر کشور\n💳 پرداخت آنلاین امن\n🔄 ضمانت بازگشت کالا\n\n📞 سفارش: 066-52224477`);
        }

        function openEducationCenter(course) {
            const courses = {
                'mountaineering': {
                    title: 'دوره کوهنوردی',
                    details: '📅 مدت: 3 روز\n👥 ظرفیت: 12 نفر\n💰 هزینه: 650 هزار تومان\n📍 محل: پایگاه کوهنوردی اشترانکوه\n\n📋 سرفصل‌ها:\n• ایمنی و تجهیزات\n• تکنیک‌های صعود\n• ناوبری کوهستان\n• امداد اولیه'
                },
                'photography': {
                    title: 'عکاسی طبیعت',
                    details: '📅 مدت: 2 روز\n👥 ظرفیت: 8 نفر\n💰 هزینه: 450 هزار تومان\n📍 محل: جاذبه‌های طبیعی دورود\n\n📋 سرفصل‌ها:\n• تنظیمات دوربین\n• ترکیب‌بندی\n• عکاسی در نور طبیعی\n• ویرایش عکس'
                },
                'crafts': {
                    title: 'صنایع دستی',
                    details: '📅 مدت: 5 روز\n👥 ظرفیت: 10 نفر\n💰 هزینه: 380 هزار تومان\n📍 محل: کارگاه صنایع دستی\n\n📋 سرفصل‌ها:\n• گلیم‌بافی\n• سفالگری\n• چوب‌تراشی\n• رنگ‌رزی طبیعی'
                },
                'language': {
                    title: 'زبان و فرهنگ لری',
                    details: '📅 مدت: 4 روز\n👥 ظرفیت: 15 نفر\n💰 هزینه: 280 هزار تومان\n📍 محل: مرکز فرهنگی دورود\n\n📋 سرفصل‌ها:\n• مکالمات روزمره\n• ضرب‌المثل‌ها\n• داستان‌های عامیانه\n• آداب و رسوم'
                }
            };
            
            const course_info = courses[course];
            alert(`🎓 ${course_info.title}\n\n${course_info.details}\n\n📞 ثبت‌نام: 066-52224488\n📧 education@dorud-lorestan.ir`);
        }

        function openHealthServices(service) {
            const services = {
                'medical': {
                    title: 'مراکز درمانی',
                    info: '🏥 بیمارستان دورود\n📍 خیابان امام، جنب پارک شهر\n📞 066-52223344\n\n🏥 درمانگاه تخصصی\n📍 میدان مرکزی\n📞 066-52223355\n\n💊 داروخانه شبانه‌روزی\n📍 خیابان ولیعصر\n📞 066-52223366'
                },
                'traditional': {
                    title: 'طب سنتی',
                    info: '🌿 مرکز طب سنتی دورود\n📍 کوچه حکیم نظامی\n📞 066-52224499\n\n🌱 کلینیک گیاه‌درمانی\n📍 بازار قدیم\n📞 066-52224488\n\n💆 مرکز حجامت\n📍 خیابان شهید بهشتی\n📞 066-52224477'
                },
                'emergency': {
                    title: 'خدمات اورژانس',
                    info: '🚑 اورژانس: 115\n🚒 آتش‌نشانی: 125\n👮 پلیس: 110\n🆘 امداد جاده‌ای: 141\n⛑️ هلال احمر: 066-52225500\n🏔️ امداد کوهستان: 066-52225511'
                },
                'wellness': {
                    title: 'مراکز تندرستی',
                    info: '🧘 مرکز یوگا کوهستان\n📍 پارک جنگلی\n📞 066-52226600\n\n💆 مرکز ماساژ درمانی\n📍 چشمه گرماب\n📞 066-52226611\n\n🏊 مجموعه آب‌درمانی\n📍 روستای بر افتاب\n📞 066-52226622'
                }
            };
            
            const service_info = services[service];
            alert(`🏥 ${service_info.title}\n\n${service_info.info}`);
        }

        function openTransportation(type) {
            const transport = {
                'rental': {
                    title: 'اجاره خودرو',
                    info: '🚗 اجاره خودرو دورود\n📍 میدان مرکزی\n📞 066-52227700\n💰 از 350 هزار تومان/روز\n\n🏔️ اجاره شاسی‌بلند\n📞 066-52227711\n💰 از 650 هزار تومان/روز\n\n🚲 اجاره دوچرخه\n📞 066-52227722\n💰 از 50 هزار تومان/روز'
                },
                'taxi': {
                    title: 'تاکسی‌های محلی',
                    info: '🚕 تاکسی شهری: 066-52228800\n🚐 تاکسی بین‌شهری: 066-52228811\n🗻 تاکسی گردشگری: 066-52228822\n\n💰 نرخ‌ها:\n• شهری: 15 هزار تومان\n• به جاذبه‌ها: 80-150 هزار تومان\n• روزانه: 800 هزار تومان'
                },
                'routes': {
                    title: 'راهنمای مسیرها',
                    info: '🗺️ مسیرهای اصلی:\n\n🛣️ تهران - دورود: 380 کیلومتر\n⏱️ زمان: 5 ساعت\n\n🛣️ اصفهان - دورود: 280 کیلومتر\n⏱️ زمان: 4 ساعت\n\n🛣️ خرم‌آباد - دورود: 120 کیلومتر\n⏱️ زمان: 2 ساعت\n\n📱 اپلیکیشن نقشه پیشنهادی: Waze, Google Maps'
                },
                'parking': {
                    title: 'پارکینگ و توقف',
                    info: '🅿️ پارکینگ‌های عمومی:\n\n🏛️ پارکینگ شهرداری\n📍 میدان مرکزی\n💰 10 هزار تومان/ساعت\n\n🗻 پارکینگ اشترانکوه\n📍 پایگاه کوهنوردی\n💰 رایگان\n\n💧 پارکینگ آبشار\n📍 بیشه‌لو\n💰 20 هزار تومان/روز'
                }
            };
            
            const transport_info = transport[type];
            alert(`🚗 ${transport_info.title}\n\n${transport_info.info}`);
        }

        // Card Dialog Functions
        function openCardDialog(cardType, icon, title) {
            const dialog = document.getElementById('cardDialog');
            const dialogIcon = document.getElementById('dialogIcon');
            const dialogTitle = document.getElementById('dialogTitle');
            const dialogDescription = document.getElementById('dialogDescription');
            const dialogFeatures = document.getElementById('dialogFeatures');
            const dialogActions = document.getElementById('dialogActions');
            
            // Set basic info
            dialogIcon.textContent = icon;
            dialogTitle.textContent = title;
            
            // Card data
            const cardData = {
                'zagros': {
                    description: 'رشته کوه‌های زاگرس یکی از مهم‌ترین و زیباترین رشته کوه‌های ایران است که از شمال غرب تا جنوب شرق کشور امتداد دارد. این کوه‌ها با قله‌های مرتفع، دره‌های عمیق، و تنوع زیستی فوق‌العاده، منظره‌ای خیره‌کننده از طبیعت بکر ایران ارائه می‌دهند.',
                    features: [
                        { icon: '⛰️', title: 'قله اشترانکوه', desc: 'بلندترین قله منطقه با ارتفاع 4050 متر' },
                        { icon: '🦅', title: 'حیات وحش', desc: 'زیستگاه عقاب طلایی، پلنگ ایرانی و کل وحشی' },
                        { icon: '🌿', title: 'پوشش گیاهی', desc: 'جنگل‌های بلوط، بادام کوهی و گیاهان دارویی' },
                        { icon: '❄️', title: 'اقلیم کوهستانی', desc: 'هوای خنک تابستان و برف زمستان' }
                    ],
                    actions: [
                        { text: '🧗 برنامه کوهنوردی', class: 'primary', action: 'showMountaineeringProgram()' },
                        { text: '📸 گالری تصاویر', class: '', action: 'showPage("gallery")' },
                        { text: '🗺️ نقشه مسیرها', class: '', action: 'openMap()' }
                    ]
                },
                'forests': {
                    description: 'جنگل‌های زاگرس با درختان بلوط، بادام کوهی و انواع گیاهان کوهستانی، اکوسیستمی منحصربه‌فرد را تشکیل می‌دهند. این جنگل‌ها در فصل پاییز با رنگ‌های طلایی، نارنجی و قرمز، یکی از زیباترین مناظر طبیعی ایران را خلق می‌کنند.',
                    features: [
                        { icon: '🌳', title: 'درختان بلوط', desc: 'جنگل‌های انبوه بلوط با قدمت صدها سال' },
                        { icon: '🍂', title: 'پاییز طلایی', desc: 'رنگ‌های خیره‌کننده در فصل پاییز' },
                        { icon: '🐻', title: 'حیوانات جنگلی', desc: 'خرس قهوه‌ای، گراز وحشی و روباه' },
                        { icon: '🌺', title: 'گیاهان دارویی', desc: 'بیش از 200 گونه گیاه دارویی' }
                    ],
                    actions: [
                        { text: '🥾 مسیرهای پیاده‌روی', class: 'primary', action: 'showHikingTrails()' },
                        { text: '🌿 اکوتوریسم', class: '', action: 'showPage("ecotourism")' },
                        { text: '📚 راهنمای گیاهان', class: '', action: 'showPlantGuide()' }
                    ]
                },
                'springs': {
                    description: 'چشمه‌های زلال دورود از دل کوه‌های زاگرس سرچشمه می‌گیرند و آب‌های خنک و شفافی دارند که علاوه بر زیبایی طبیعی، خواص درمانی نیز دارند. این چشمه‌ها منبع اصلی آب شرب منطقه و زیستگاه آبزیان کوهستانی هستند.',
                    features: [
                        { icon: '♨️', title: 'چشمه گرماب', desc: 'آب گرم طبیعی با خواص درمانی' },
                        { icon: '💎', title: 'آب معدنی', desc: 'غنی از مواد معدنی مفید برای سلامت' },
                        { icon: '🐟', title: 'ماهی قزل‌آلا', desc: 'پرورش طبیعی ماهی در آب‌های خنک' },
                        { icon: '🌊', title: 'آبشارها', desc: 'آبشارهای زیبا و طبیعی در مسیر چشمه‌ها' }
                    ],
                    actions: [
                        { text: '♨️ آب‌درمانی', class: 'primary', action: 'showWaterTherapy()' },
                        { text: '🎣 ماهیگیری', class: '', action: 'showFishingSpots()' },
                        { text: '💧 تور چشمه‌ها', class: '', action: 'showSpringsMap()' }
                    ]
                },
                'heritage': {
                    description: 'میراث تاریخی دورود شامل آثار باستانی از دوران‌های مختلف تاریخ ایران است. از پل‌های ساسانی گرفته تا بقاع مقدس و بناهای اسلامی، هر کدام نشان‌دهنده بخشی از تمدن کهن این سرزمین هستند.',
                    features: [
                        { icon: '🌉', title: 'پل کشکان', desc: 'پل تاریخی ساسانی با معماری منحصربه‌فرد' },
                        { icon: '🕌', title: 'بقاع مقدس', desc: 'آرامگاه‌ها و بقاع با اهمیت مذهبی' },
                        { icon: '🏺', title: 'آثار باستانی', desc: 'سفال‌ها و ابزار کشف‌شده از دوران کهن' },
                        { icon: '📜', title: 'کتیبه‌ها', desc: 'نوشته‌های تاریخی به خط‌های مختلف' }
                    ],
                    actions: [
                        { text: '🏛️ تور تاریخی', class: 'primary', action: 'showHistoricalTour()' },
                        { text: '📚 تاریخچه دورود', class: '', action: 'showPage("history")' },
                        { text: '🎭 فرهنگ محلی', class: '', action: 'showPage("culture")' }
                    ]
                }
            };
            
            const data = cardData[cardType];
            if (!data) return;
            
            // Set description
            dialogDescription.textContent = data.description;
            
            // Set features
            dialogFeatures.innerHTML = data.features.map(feature => `
                <div class="feature-item">
                    <span class="feature-icon">${feature.icon}</span>
                    <div class="feature-title">${feature.title}</div>
                    <div class="feature-desc">${feature.desc}</div>
                </div>
            `).join('');
            
            // Set actions
            dialogActions.innerHTML = data.actions.map(action => `
                <button class="dialog-btn ${action.class}" onclick="${action.action}; closeCardDialog();">
                    ${action.text}
                </button>
            `).join('');
            
            // Show dialog
            dialog.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeCardDialog() {
            const dialog = document.getElementById('cardDialog');
            dialog.classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        // Additional functions for dialog actions
        function showMountaineeringProgram() {
            alert('🧗 برنامه کوهنوردی\n\n📅 تورهای هفتگی به قله اشترانکوه\n⏰ مدت: 2 روز و 1 شب\n👥 حداکثر 8 نفر\n💰 هزینه: 850 هزار تومان\n\n📋 شامل:\n• راهنمای مجرب\n• تجهیزات کوهنوردی\n• غذا و اقامت\n• بیمه\n\n📞 رزرو: 066-52224499');
        }

        function showHikingTrails() {
            alert('🥾 مسیرهای پیاده‌روی\n\n🌲 مسیر جنگلی (آسان): 3 کیلومتر\n🏔️ مسیر کوهستانی (متوسط): 7 کیلومتر\n⛰️ مسیر قله (سخت): 12 کیلومتر\n\n✅ همه مسیرها علامت‌گذاری شده\n🗺️ نقشه و GPS موجود\n☎️ اطلاعات: 066-52224488');
        }

        function showWaterTherapy() {
            alert('♨️ آب‌درمانی طبیعی\n\n🌊 چشمه گرماب: 42 درجه سانتیگراد\n💊 خواص درمانی: روماتیسم، آرتریت، بیماری‌های پوستی\n⏰ ساعات کار: 6 صبح تا 10 شب\n💰 ورودی: 50 هزار تومان\n\n🏨 امکانات: رختکن، دوش، کافه\n📞 اطلاعات: 066-52225566');
        }

        function showFishingSpots() {
            alert('🎣 نقاط ماهیگیری\n\n🐟 رودخانه کشکان: ماهی قزل‌آلا\n🏞️ چشمه بیشه‌لو: کپور کوهی\n💧 استخر طبیعی: ماهی سفید\n\n📋 مجوز ماهیگیری لازم\n🎣 اجاره تجهیزات موجود\n📞 اطلاعات: 066-52226677');
        }

        function showSpringsMap() {
            alert('💧 نقشه چشمه‌ها\n\n📍 چشمه گرماب: 5 کیلومتری شهر\n📍 چشمه بیشه‌لو: 12 کیلومتری شهر\n📍 چشمه زلال: 8 کیلومتری شهر\n\n🚗 دسترسی با خودرو\n🥾 مسیر پیاده‌روی\n🗺️ نقشه دیجیتال موجود');
        }

        function showHistoricalTour() {
            alert('🏛️ تور تاریخی دورود\n\n📅 روزهای زوج هفته\n⏰ ساعت 9 صبح\n👥 حداکثر 15 نفر\n💰 هزینه: 120 هزار تومان\n\n📋 مسیر تور:\n• پل کشکان\n• بقعه پیر عبدالله\n• موزه محلی\n• بازار تاریخی\n\n📞 رزرو: 066-52223377');
        }

        function showPlantGuide() {
            alert('📚 راهنمای گیاهان دارویی\n\n🌿 بیش از 200 گونه شناسایی‌شده\n📖 کتابچه راهنما موجود\n👨‍🏫 کارگاه آموزشی ماهانه\n🏪 فروش گیاهان خشک\n\n📞 مرکز گیاهان دارویی: 066-52227788');
        }

        // Initialize widgets on page load
        document.addEventListener('DOMContentLoaded', function() {
            // Initialize gallery
            showGalleryCategory('all');
            
            // Close modal when clicking outside
            document.getElementById('imageModal').addEventListener('click', function(e) {
                if (e.target === this) {
                    closeImageModal();
                }
            });

            // Close card dialog when clicking outside
            document.getElementById('cardDialog').addEventListener('click', function(e) {
                if (e.target === this) {
                    closeCardDialog();
                }
            });
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'986b4eda17fdd375',t:'MTc1OTE0NzA5OS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>

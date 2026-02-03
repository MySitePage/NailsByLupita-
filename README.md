
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nails By Lupita | Luxury Nail, Lash & Piercing Tech</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display+SC:wght@500;600&family=Allura&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            /* NEW COLOR PALETTE - Baby Pink & Dark Grey */
            --baby-pink: #FFD1DC;
            --pink-accent: #FFB6C1;
            --dark-grey: #2C2C2C;
            --medium-grey: #4A4A4A;
            --light-grey: #F5F5F5;
            --text-dark: #333333;
            --text-light: #FFFFFF;
            --soft-white: #FFF8F8;
            
            /* ENHANCED: Added more color variations for depth */
            --pink-light: #FFE4E9;
            --grey-light: #F8F8F8;
            --shadow-color: rgba(44, 44, 44, 0.1);
            --shadow-pink: rgba(255, 182, 193, 0.2);
            
            /* Fonts */
            --heading-font: 'Playfair Display SC', serif;
            --accent-font: 'Allura', cursive;
            --body-font: 'Poppins', sans-serif;
            
            /* Spacing */
            --header-height-desktop: 85px;
            --header-height-mobile: 70px;
            --header-height-tablet: 75px;
            
            /* ENHANCED: Added decorative borders */
            --border-radius: 20px;
            --border-radius-small: 12px;
            --border-thickness: 2px;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: var(--body-font);
            background-color: var(--soft-white);
            color: var(--text-dark);
            line-height: 1.6;
            overflow-x: hidden;
            -webkit-text-size-adjust: 100%;
            /* ENHANCED: Added subtle background pattern */
            background-image: 
                radial-gradient(circle at 25px 25px, var(--pink-light) 2%, transparent 2%),
                radial-gradient(circle at 75px 75px, var(--pink-light) 2%, transparent 2%);
            background-size: 100px 100px;
            background-attachment: fixed;
        }
        
        a {
            text-decoration: none;
            color: inherit;
        }
        
        img {
            max-width: 100%;
            display: block;
            height: auto;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            position: relative;
        }
        
        /* ENHANCED: Decorative corner accents */
        .container::before,
        .container::after {
            content: '';
            position: absolute;
            width: 40px;
            height: 40px;
            border: 2px solid var(--baby-pink);
            opacity: 0.3;
            z-index: -1;
        }
        
        .container::before {
            top: -15px;
            left: -15px;
            border-right: none;
            border-bottom: none;
        }
        
        .container::after {
            bottom: -15px;
            right: -15px;
            border-left: none;
            border-top: none;
        }
        
        /* ENHANCED: Updated button with more depth */
        .btn {
            display: inline-block;
            background-color: var(--pink-accent);
            color: var(--dark-grey);
            font-family: var(--body-font);
            font-weight: 500;
            padding: 14px 32px;
            border-radius: 25px;
            transition: all 0.4s ease;
            border: none;
            cursor: pointer;
            font-size: 16px;
            box-shadow: 
                0 6px 20px rgba(255, 182, 193, 0.4),
                inset 0 1px 0 rgba(255, 255, 255, 0.3);
            position: relative;
            overflow: hidden;
            letter-spacing: 0.5px;
        }
        
        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.7s ease;
        }
        
        .btn:hover {
            background-color: var(--baby-pink);
            transform: translateY(-3px) scale(1.03);
            box-shadow: 
                0 10px 30px rgba(255, 182, 193, 0.5),
                inset 0 1px 0 rgba(255, 255, 255, 0.4);
        }
        
        .btn:hover::before {
            left: 100%;
        }
        
        /* ENHANCED: More decorative section title */
        .section-title {
            font-family: var(--accent-font);
            font-weight: 400;
            color: var(--dark-grey);
            font-size: 3.5rem;
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
            padding: 0 20px;
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .section-title::before,
        .section-title::after {
            content: '✦';
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            color: var(--pink-accent);
            font-size: 1.5rem;
            opacity: 0.8;
        }
        
        .section-title::before {
            left: 0;
        }
        
        .section-title::after {
            right: 0;
        }
        
        .section-title span {
            display: block;
            font-family: var(--body-font);
            font-size: 1rem;
            font-weight: 300;
            color: var(--medium-grey);
            margin-top: 10px;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        
        /* PAGE TRANSITION */
        .page {
            display: none;
            animation: fadeIn 0.5s ease;
        }
        
        .page.active {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        /* ENHANCED: HEADER with more visual details */
        header {
            position: sticky;
            top: 0;
            z-index: 1000;
            background-color: var(--soft-white);
            height: var(--header-height-desktop);
            border-bottom: 2px solid var(--baby-pink);
            box-shadow: 0 4px 20px rgba(44, 44, 44, 0.1);
            transition: all 0.4s ease;
            width: 100%;
            backdrop-filter: blur(10px);
            background-color: rgba(255, 248, 248, 0.95);
        }
        
        .header-transparent {
            background-color: transparent !important;
            border-bottom: 2px solid rgba(255, 255, 255, 0.3);
            box-shadow: none;
            backdrop-filter: none;
        }
        
        .header-transparent .logo,
        .header-transparent .nav-links a,
        .header-transparent .hamburger span {
            color: var(--text-light) !important;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
            padding: 0 30px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        /* ENHANCED: Logo WITHOUT the pink slash background */
        .logo {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: 2.8rem;
            color: var(--dark-grey);
            transition: all 0.3s ease;
            cursor: pointer;
            white-space: nowrap;
            position: relative;
            padding: 5px 15px;
            border-radius: 15px;
            /* REMOVED the pink slash background */
            background: transparent;
        }
        
        .logo:hover {
            opacity: 0.9;
            transform: scale(1.02);
        }
        
        /* ENHANCED: Desktop Navigation with better visual hierarchy */
        .nav-desktop {
            display: flex;
            align-items: center;
            gap: 30px;
        }
        
        .nav-center {
            display: flex;
            align-items: center;
            gap: 30px;
            padding: 10px 20px;
            background: var(--grey-light);
            border-radius: 25px;
            box-shadow: 
                inset 2px 2px 4px rgba(255, 255, 255, 0.8),
                inset -2px -2px 4px rgba(0, 0, 0, 0.05);
        }
        
        .divider {
            width: 1px;
            height: 25px;
            background: linear-gradient(to bottom, transparent, var(--baby-pink), transparent);
        }
        
        .nav-links {
            display: flex;
            gap: 25px;
            list-style: none;
        }
        
        .nav-links a {
            font-family: var(--body-font);
            font-weight: 500;
            color: var(--dark-grey);
            position: relative;
            transition: all 0.3s ease;
            cursor: pointer;
            white-space: nowrap;
            padding: 8px 0;
            font-size: 1.05rem;
        }
        
        .nav-links a.active-page {
            color: var(--pink-accent);
            font-weight: 600;
        }
        
        .nav-links a:hover {
            color: var(--pink-accent);
            transform: translateY(-1px);
        }
        
        .nav-links a:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background: linear-gradient(90deg, var(--baby-pink), var(--pink-accent));
            border-radius: 2px;
            transition: width 0.3s ease;
            box-shadow: 0 2px 4px var(--shadow-pink);
        }
        
        .nav-links a:hover:after,
        .nav-links a.active-page:after {
            width: 100%;
        }
        
        /* ENHANCED: Mobile Navigation */
        .hamburger {
            display: none;
            flex-direction: column;
            gap: 6px;
            background: none;
            border: none;
            cursor: pointer;
            padding: 10px;
            z-index: 1001;
            background: var(--grey-light);
            border-radius: 10px;
            box-shadow: 
                inset 2px 2px 4px rgba(255, 255, 255, 0.8),
                inset -2px -2px 4px rgba(0, 0, 0, 0.05);
        }
        
        .hamburger span {
            display: block;
            width: 25px;
            height: 3px;
            background-color: var(--dark-grey);
            transition: all 0.3s ease;
            border-radius: 3px;
        }
        
        .mobile-menu {
            position: fixed;
            top: var(--header-height-mobile);
            left: 0;
            width: 100%;
            height: calc(100vh - var(--header-height-mobile));
            background: linear-gradient(135deg, var(--soft-white) 0%, var(--grey-light) 100%);
            transform: translateY(-100%);
            opacity: 0;
            transition: all 0.4s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            z-index: 999;
            pointer-events: none;
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
            border-top: 2px solid var(--baby-pink);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        .mobile-menu.active {
            transform: translateY(0);
            opacity: 1;
            pointer-events: all;
        }
        
        .mobile-links {
            list-style: none;
            padding: 40px 20px;
            display: flex;
            flex-direction: column;
            gap: 20px;
            text-align: center;
        }
        
        .mobile-links li {
            position: relative;
            overflow: hidden;
            border-radius: 15px;
            background: rgba(255, 255, 255, 0.5);
            margin: 0 10px;
        }
        
        .mobile-links a {
            font-family: var(--body-font);
            font-size: 1.5rem;
            color: var(--dark-grey);
            display: block;
            padding: 15px 20px;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .mobile-links a.active-page {
            color: var(--pink-accent);
            font-weight: 600;
            background: linear-gradient(90deg, transparent, var(--pink-light), transparent);
        }
        
        .mobile-links a:hover {
            color: var(--pink-accent);
            transform: translateX(5px);
            background: rgba(255, 209, 220, 0.1);
        }
        
        .mobile-menu-btn {
            padding: 30px 20px;
            text-align: center;
            border-top: 2px solid var(--baby-pink);
            background: rgba(255, 255, 255, 0.8);
        }
        
        /* ENHANCED: HOME PAGE STYLES */
        /* ENHANCED: HERO SECTION with more visual elements */
        .hero {
            height: 100vh;
            min-height: 600px;
            max-height: 900px;
            background-image: 
                linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
                url('https://www.dropbox.com/scl/fi/4sqiwrylens0kuxa8uaki/MRSVOLUENTIC_.jpg?rlkey=752pxoorhed2n6vr14qb2r7rp&st=1xsxwk71&raw=1');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            margin-top: calc(-1 * var(--header-height-desktop));
            overflow: hidden;
        }
        
        /* ENHANCED: Animated background particles */
        .hero-particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        
        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: var(--baby-pink);
            border-radius: 50%;
            opacity: 0.3;
            animation: float 15s infinite linear;
        }
        
        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.3;
            }
            90% {
                opacity: 0.3;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .hero-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, rgba(255, 182, 193, 0.1), transparent 30%),
                        linear-gradient(135deg, rgba(255, 209, 220, 0.1), transparent 30%);
        }
        
        .hero-content {
            position: relative;
            z-index: 2;
            text-align: center;
            color: var(--text-light);
            max-width: 800px;
            padding: 0 20px;
            width: 100%;
            animation: contentFadeIn 1s ease-out;
        }
        
        @keyframes contentFadeIn {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .hero-title {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(3.5rem, 9vw, 6rem);
            margin-bottom: 10px;
            color: var(--soft-white);
            text-shadow: 
                0 2px 10px rgba(0, 0, 0, 0.3),
                0 0 30px rgba(255, 182, 193, 0.2);
            line-height: 1.1;
            position: relative;
            display: inline-block;
        }
        
        .hero-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 150px;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), transparent);
            border-radius: 3px;
        }
        
        .hero-subtitle {
            font-family: var(--accent-font);
            font-size: clamp(2rem, 5vw, 3rem);
            margin-bottom: 40px;
            color: var(--baby-pink);
            line-height: 1.2;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            letter-spacing: 1px;
        }
        
        /* ENHANCED: Hero button with shine effect */
        .hero-btn {
            font-size: clamp(1.3rem, 3vw, 1.8rem);
            padding: clamp(15px, 4vw, 20px) clamp(30px, 6vw, 50px);
            margin-top: 30px;
            font-family: var(--accent-font);
            background: linear-gradient(135deg, var(--pink-accent), var(--baby-pink));
            border: 2px solid rgba(255, 255, 255, 0.3);
            border-radius: 35px;
            color: var(--dark-grey);
            transition: all 0.4s ease;
            display: inline-block;
            box-shadow: 
                0 8px 25px rgba(0, 0, 0, 0.3),
                0 0 20px rgba(255, 182, 193, 0.4);
            position: relative;
            overflow: hidden;
        }
        
        .hero-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
            transition: left 0.7s ease;
        }
        
        .hero-btn:hover {
            background: linear-gradient(135deg, var(--baby-pink), var(--pink-accent));
            color: var(--dark-grey);
            transform: translateY(-5px) scale(1.05);
            box-shadow: 
                0 12px 35px rgba(0, 0, 0, 0.4),
                0 0 30px rgba(255, 182, 193, 0.6);
        }
        
        .hero-btn:hover::before {
            left: 100%;
        }
        
        /* ENHANCED: ABOUT SECTION with decorative frame */
        .about {
            padding: clamp(80px, 10vw, 120px) 0;
            background: linear-gradient(135deg, var(--light-grey) 0%, var(--soft-white) 50%, var(--light-grey) 100%);
            position: relative;
            overflow: hidden;
        }
        
        .about::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), transparent);
        }
        
        .about-container {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 60px;
            position: relative;
        }
        
        .about-text {
            flex: 1 1 500px;
            position: relative;
            padding: 30px;
            background: var(--soft-white);
            border-radius: var(--border-radius);
            box-shadow: 
                0 10px 30px rgba(0, 0, 0, 0.08),
                inset 0 0 0 1px rgba(255, 209, 220, 0.3);
            border: 2px solid transparent;
            background-clip: padding-box;
            background-image: 
                linear-gradient(var(--soft-white), var(--soft-white)),
                linear-gradient(135deg, var(--baby-pink), transparent 30%, transparent 70%, var(--baby-pink));
            background-origin: border-box;
        }
        
        .about-title {
            font-family: var(--accent-font);
            font-weight: 400;
            color: var(--dark-grey);
            font-size: clamp(2.8rem, 6vw, 4rem);
            margin-bottom: 25px;
            line-height: 1.2;
            position: relative;
            display: inline-block;
        }
        
        .about-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 80px;
            height: 3px;
            background: linear-gradient(90deg, var(--pink-accent), transparent);
            border-radius: 3px;
        }
        
        .about-description {
            font-size: clamp(1.05rem, 2vw, 1.2rem);
            line-height: 1.8;
            color: var(--text-dark);
            margin-bottom: 25px;
            background-color: var(--grey-light);
            padding: 25px;
            border-radius: var(--border-radius-small);
            border-left: 4px solid var(--pink-accent);
            box-shadow: 
                0 5px 15px rgba(0, 0, 0, 0.05),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
            position: relative;
            transition: transform 0.3s ease;
        }
        
        .about-description:hover {
            transform: translateY(-3px);
            box-shadow: 
                0 8px 20px rgba(0, 0, 0, 0.08),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
        }
        
        .about-description:last-child {
            margin-bottom: 0;
        }
        
        .about-highlight {
            color: var(--pink-accent);
            font-weight: 600;
            position: relative;
            padding: 0 2px;
        }
        
        .about-highlight::before {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background: var(--baby-pink);
            opacity: 0.3;
        }
        
        /* ENHANCED: ABOUT INFO CARD with glass effect */
        .about-info-card {
            flex: 1 1 400px;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.9), rgba(248, 248, 248, 0.9));
            border-radius: var(--border-radius);
            padding: clamp(30px, 5vw, 45px);
            box-shadow: 
                0 15px 35px rgba(0, 0, 0, 0.1),
                0 0 0 1px rgba(255, 209, 220, 0.3);
            border: 2px solid transparent;
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }
        
        .about-info-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255, 209, 220, 0.1), transparent);
            transform: rotate(45deg);
        }
        
        .info-title {
            font-family: var(--accent-font);
            font-weight: 400;
            color: var(--dark-grey);
            font-size: clamp(2.2rem, 5vw, 3rem);
            margin-bottom: 35px;
            text-align: center;
            padding-bottom: 20px;
            line-height: 1.2;
            position: relative;
        }
        
        .info-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, var(--baby-pink), var(--pink-accent), var(--baby-pink));
            border-radius: 3px;
        }
        
        .info-details {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }
        
        .info-item {
            display: flex;
            align-items: flex-start;
            gap: 20px;
            padding: 15px;
            border-radius: var(--border-radius-small);
            background: rgba(255, 255, 255, 0.6);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .info-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 100%;
            background: var(--pink-accent);
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .info-item:hover {
            background: rgba(255, 255, 255, 0.9);
            transform: translateX(5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .info-item:hover::before {
            opacity: 1;
        }
        
        .info-item i {
            color: var(--pink-accent);
            font-size: 1.6rem;
            margin-top: 5px;
            flex-shrink: 0;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 209, 220, 0.2);
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .info-item:hover i {
            background: var(--pink-accent);
            color: var(--soft-white);
            transform: scale(1.1);
        }
        
        .info-content h4 {
            font-family: var(--body-font);
            font-weight: 600;
            color: var(--dark-grey);
            margin-bottom: 8px;
            font-size: 1.1rem;
            letter-spacing: 0.5px;
        }
        
        .info-content p {
            color: var(--medium-grey);
            font-size: 1rem;
            line-height: 1.6;
        }
        
        /* ENHANCED: SERVICES SECTION with floating cards */
        .services {
            padding: clamp(80px, 10vw, 120px) 0;
            background: var(--soft-white);
            position: relative;
        }
        
        .services::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), transparent);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 35px;
            margin-top: 60px;
        }
        
        .service-card {
            background: linear-gradient(135deg, var(--light-grey) 0%, var(--soft-white) 100%);
            border: 2px solid transparent;
            border-radius: var(--border-radius);
            padding: 35px 30px;
            box-shadow: 
                0 10px 25px rgba(0, 0, 0, 0.08),
                0 0 0 1px rgba(255, 209, 220, 0.2);
            transition: all 0.4s ease;
            text-align: center;
            height: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            overflow: hidden;
        }
        
        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--baby-pink), var(--pink-accent), var(--baby-pink));
            transform: translateX(-100%);
            transition: transform 0.4s ease;
        }
        
        .service-card:hover {
            transform: translateY(-12px) scale(1.02);
            box-shadow: 
                0 20px 40px rgba(255, 182, 193, 0.2),
                0 0 0 1px rgba(255, 209, 220, 0.3);
        }
        
        .service-card:hover::before {
            transform: translateX(0);
        }
        
        .service-icon {
            font-size: 3rem;
            color: var(--pink-accent);
            margin-bottom: 25px;
            width: 80px;
            height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 209, 220, 0.2);
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .service-card:hover .service-icon {
            background: var(--pink-accent);
            color: var(--soft-white);
            transform: scale(1.1) rotate(5deg);
        }
        
        .service-title {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(2rem, 4vw, 2.4rem);
            margin-bottom: 20px;
            color: var(--dark-grey);
            line-height: 1.2;
            position: relative;
            padding-bottom: 15px;
        }
        
        .service-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 50px;
            height: 2px;
            background: var(--baby-pink);
            border-radius: 2px;
        }
        
        .service-description {
            color: var(--medium-grey);
            font-size: 1rem;
            line-height: 1.7;
            flex-grow: 1;
        }
        
        /* ENHANCED: GALLERY PREVIEW with improved slider */
        .gallery-preview {
            padding: clamp(80px, 10vw, 120px) 0;
            background: linear-gradient(to bottom, var(--soft-white), var(--light-grey));
            position: relative;
            overflow: hidden;
        }
        
        .gallery-preview::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), transparent);
        }
        
        .gallery-slider-container {
            position: relative;
            width: 100%;
            overflow: hidden;
            margin-top: 60px;
            padding: 20px 0;
        }
        
        .gallery-slider {
            display: flex;
            gap: 25px;
            animation: scroll 40s linear infinite;
            padding: 10px 0;
        }
        
        .gallery-slider:hover {
            animation-play-state: paused;
        }
        
        .gallery-slide {
            flex: 0 0 auto;
            width: 320px;
            height: 320px;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: 
                0 15px 30px rgba(0, 0, 0, 0.15),
                0 0 0 1px rgba(255, 209, 220, 0.3);
            position: relative;
            transition: all 0.3s ease;
        }
        
        .gallery-slide::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to bottom, transparent 60%, rgba(0, 0, 0, 0.5));
            z-index: 1;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .gallery-slide:hover {
            transform: scale(1.05);
            box-shadow: 
                0 25px 50px rgba(0, 0, 0, 0.2),
                0 0 0 2px rgba(255, 209, 220, 0.4);
        }
        
        .gallery-slide:hover::before {
            opacity: 1;
        }
        
        .gallery-slide img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .gallery-slide:hover img {
            transform: scale(1.1);
        }
        
        .gallery-link {
            display: inline-flex;
            align-items: center;
            gap: 15px;
            text-align: center;
            margin-top: 50px;
            font-family: var(--accent-font);
            font-size: clamp(2rem, 5vw, 2.8rem);
            color: var(--dark-grey);
            transition: all 0.3s ease;
            cursor: pointer;
            padding: 15px 30px;
            border-radius: 30px;
            background: rgba(255, 255, 255, 0.8);
            border: 2px solid var(--baby-pink);
            left: 50%;
            position: relative;
            transform: translateX(-50%);
        }
        
        .gallery-link:hover {
            color: var(--pink-accent);
            background: var(--soft-white);
            transform: translateX(-50%) translateY(-3px);
            box-shadow: 0 10px 25px rgba(255, 182, 193, 0.2);
        }
        
        .gallery-link i {
            font-size: 1.8rem;
            transition: transform 0.3s ease;
        }
        
        .gallery-link:hover i {
            transform: translateX(5px);
        }
        
        @keyframes scroll {
            0% {
                transform: translateX(0);
            }
            100% {
                transform: translateX(calc(-320px * 8));
            }
        }
        
        /* ENHANCED: POLICIES SECTION with timeline effect */
        .policies {
            padding: clamp(80px, 10vw, 120px) 0;
            background: linear-gradient(135deg, var(--light-grey) 0%, var(--baby-pink) 100%);
            position: relative;
        }
        
        .policies-container {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
        }
        
        .policies-container::before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: 40px;
            width: 3px;
            background: linear-gradient(to bottom, transparent, var(--pink-accent), transparent);
        }
        
        .policy-item {
            background: var(--soft-white);
            border-radius: var(--border-radius);
            padding: 30px 30px 30px 80px;
            margin-bottom: 30px;
            box-shadow: 
                0 10px 25px rgba(0, 0, 0, 0.08),
                0 0 0 1px rgba(255, 209, 220, 0.3);
            border-left: 5px solid var(--pink-accent);
            position: relative;
            transition: all 0.3s ease;
        }
        
        .policy-item::before {
            content: '';
            position: absolute;
            left: 32px;
            top: 40px;
            width: 20px;
            height: 20px;
            background: var(--pink-accent);
            border-radius: 50%;
            box-shadow: 0 0 0 4px var(--soft-white), 0 0 0 6px var(--pink-accent);
        }
        
        .policy-item:hover {
            transform: translateX(10px);
            box-shadow: 
                0 15px 35px rgba(0, 0, 0, 0.12),
                0 0 0 1px rgba(255, 209, 220, 0.4);
        }
        
        .policy-title {
            font-family: var(--accent-font);
            font-weight: 400;
            color: var(--dark-grey);
            font-size: clamp(1.6rem, 4vw, 2rem);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 15px;
            line-height: 1.3;
        }
        
        .policy-title i {
            font-size: 1.8rem;
            color: var(--pink-accent);
            width: 50px;
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 209, 220, 0.2);
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .policy-item:hover .policy-title i {
            background: var(--pink-accent);
            color: var(--soft-white);
            transform: rotate(15deg);
        }
        
        .policy-text {
            color: var(--text-dark);
            font-size: 1rem;
            line-height: 1.7;
            padding-left: 10px;
            border-left: 2px solid var(--baby-pink);
            margin-left: 15px;
        }
        
        /* ENHANCED: INSTAGRAM PROMO with gradient text */
        .instagram-promo {
            padding: clamp(60px, 8vw, 100px) 0;
            background: var(--dark-grey);
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .instagram-promo::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(circle at 20% 30%, rgba(255, 182, 193, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 70%, rgba(255, 209, 220, 0.1) 0%, transparent 50%);
        }
        
        .instagram-text {
            font-family: var(--accent-font);
            font-size: clamp(2.5rem, 6vw, 3.5rem);
            color: transparent;
            margin-bottom: 20px;
            line-height: 1.2;
            background: linear-gradient(90deg, var(--baby-pink), var(--pink-accent), var(--baby-pink));
            -webkit-background-clip: text;
            background-clip: text;
            background-size: 200% 100%;
            animation: gradientShift 3s ease infinite;
            position: relative;
            display: inline-block;
        }
        
        @keyframes gradientShift {
            0%, 100% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
        }
        
        .instagram-text::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 150px;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), transparent);
        }
        
        .instagram-handle {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(2rem, 4vw, 2.8rem);
            color: var(--soft-white);
            line-height: 1.2;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
            position: relative;
            display: inline-block;
            padding: 15px 30px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 209, 220, 0.2);
        }
        
        /* ENHANCED: GALLERY PAGE with masonry layout */
        .gallery-hero {
            padding: clamp(120px, 15vw, 160px) 0 clamp(60px, 8vw, 80px);
            text-align: center;
            background: linear-gradient(135deg, var(--soft-white) 0%, var(--light-grey) 100%);
            position: relative;
            overflow: hidden;
        }
        
        .gallery-hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), var(--pink-accent), var(--baby-pink), transparent);
        }
        
        .gallery-title {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(3rem, 7vw, 5rem);
            color: var(--dark-grey);
            margin-bottom: 15px;
            line-height: 1.1;
            position: relative;
            display: inline-block;
        }
        
        .gallery-title::before,
        .gallery-title::after {
            content: '✨';
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            font-size: 2rem;
        }
        
        .gallery-title::before {
            left: -40px;
        }
        
        .gallery-title::after {
            right: -40px;
        }
        
        .gallery-subtitle {
            font-family: var(--accent-font);
            font-size: clamp(2rem, 4vw, 3rem);
            color: var(--pink-accent);
            line-height: 1.2;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        
        .gallery-grid {
            padding: clamp(60px, 8vw, 80px) 0 clamp(80px, 10vw, 120px);
        }
        
        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 30px;
        }
        
        .gallery-item {
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: 
                0 15px 35px rgba(0, 0, 0, 0.1),
                0 0 0 1px rgba(255, 209, 220, 0.3);
            transition: all 0.4s ease;
            position: relative;
            height: 350px;
        }
        
        .gallery-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to bottom, transparent 60%, rgba(0, 0, 0, 0.6));
            z-index: 1;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .gallery-item:hover {
            transform: scale(1.05) rotate(1deg);
            box-shadow: 
                0 25px 50px rgba(0, 0, 0, 0.2),
                0 0 0 2px rgba(255, 209, 220, 0.4);
        }
        
        .gallery-item:hover::before {
            opacity: 1;
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.1);
        }
        
        /* ENHANCED: BOOKING PAGE with glass morphism */
        .booking-hero {
            height: auto;
            min-height: 100vh;
            max-height: none;
            background-image: 
                linear-gradient(rgba(0, 0, 0, 0.85), rgba(0, 0, 0, 0.85)),
                url('https://www.dropbox.com/scl/fi/4sqiwrylens0kuxa8uaki/MRSVOLUENTIC_.jpg?rlkey=752pxoorhed2n6vr14qb2r7rp&st=1xsxwk71&raw=1');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            margin-top: calc(-1 * var(--header-height-desktop));
            padding: clamp(100px, 12vw, 140px) 0 clamp(80px, 10vw, 100px);
            overflow: hidden;
        }
        
        .booking-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 30%, rgba(255, 182, 193, 0.1) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(255, 209, 220, 0.1) 0%, transparent 40%);
            backdrop-filter: blur(5px);
        }
        
        .booking-content {
            position: relative;
            z-index: 2;
            text-align: center;
            color: var(--text-light);
            max-width: 900px;
            padding: 0 20px;
            width: 100%;
            animation: contentFadeIn 1s ease-out;
        }
        
        .booking-title {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(3rem, 6vw, 4.5rem);
            margin-bottom: 50px;
            color: var(--baby-pink);
            line-height: 1.2;
            position: relative;
            display: inline-block;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        }
        
        .booking-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 200px;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), transparent);
            border-radius: 3px;
        }
        
        /* ENHANCED: BOOKING FORM with glass effect */
        .booking-form-container {
            background: rgba(255, 255, 255, 0.1);
            border-radius: var(--border-radius);
            padding: clamp(30px, 5vw, 60px);
            margin-top: 30px;
            backdrop-filter: blur(15px);
            text-align: left;
            border: 2px solid rgba(255, 209, 220, 0.3);
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.2),
                inset 0 1px 0 rgba(255, 255, 255, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .booking-form-container::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transform: rotate(45deg);
        }
        
        .form-group {
            margin-bottom: 30px;
            position: relative;
            z-index: 1;
        }
        
        .form-label {
            display: block;
            font-family: var(--body-font);
            font-weight: 500;
            color: var(--baby-pink);
            margin-bottom: 10px;
            font-size: 1.1rem;
            padding-left: 5px;
            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
        }
        
        .form-control {
            width: 100%;
            padding: 16px 20px;
            border: 2px solid rgba(255, 209, 220, 0.5);
            border-radius: var(--border-radius-small);
            background: rgba(255, 255, 255, 0.1);
            color: var(--text-light);
            font-family: var(--body-font);
            font-size: 1rem;
            transition: all 0.3s ease;
            backdrop-filter: blur(5px);
        }
        
        .form-control:focus {
            outline: none;
            border-color: var(--baby-pink);
            background: rgba(255, 255, 255, 0.2);
            box-shadow: 
                0 0 0 3px rgba(255, 209, 220, 0.2),
                inset 0 2px 4px rgba(255, 255, 255, 0.1);
        }
        
        .form-control::placeholder {
            color: rgba(255, 255, 255, 0.6);
            font-style: italic;
        }
        
        select.form-control {
            appearance: none;
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='%23FFD1DC' viewBox='0 0 16 16'%3E%3Cpath d='M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z'/%3E%3C/svg%3E");
            background-repeat: no-repeat;
            background-position: right 20px center;
            background-size: 16px;
            padding-right: 50px;
        }
        
        .form-row {
            display: flex;
            flex-wrap: wrap;
            gap: 25px;
        }
        
        .form-row .form-group {
            flex: 1 1 250px;
        }
        
        .form-submit {
            text-align: center;
            margin-top: 50px;
            position: relative;
            z-index: 1;
        }
        
        .submit-btn {
            background: linear-gradient(135deg, var(--baby-pink), var(--pink-accent));
            color: var(--dark-grey);
            font-family: var(--accent-font);
            font-size: clamp(1.6rem, 4vw, 2rem);
            padding: clamp(15px, 4vw, 20px) clamp(35px, 7vw, 60px);
            border-radius: 35px;
            border: 2px solid rgba(255, 255, 255, 0.3);
            cursor: pointer;
            transition: all 0.4s ease;
            box-shadow: 
                0 10px 30px rgba(0, 0, 0, 0.3),
                0 0 20px rgba(255, 182, 193, 0.4);
            position: relative;
            overflow: hidden;
            letter-spacing: 1px;
        }
        
        .submit-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
            transition: left 0.7s ease;
        }
        
        .submit-btn:hover {
            background: linear-gradient(135deg, var(--pink-accent), var(--baby-pink));
            transform: translateY(-5px) scale(1.05);
            box-shadow: 
                0 15px 40px rgba(0, 0, 0, 0.4),
                0 0 30px rgba(255, 182, 193, 0.6);
        }
        
        .submit-btn:hover::before {
            left: 100%;
        }
        
        .booking-instructions {
            margin-top: 50px;
            padding-top: 40px;
            border-top: 2px solid rgba(255, 209, 220, 0.3);
            color: var(--baby-pink);
            font-size: 1.05rem;
            text-align: center;
            line-height: 1.7;
            position: relative;
            z-index: 1;
        }
        
        .booking-instructions p {
            margin-bottom: 20px;
            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
        }
        
        .booking-contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 25px;
            margin-top: 30px;
        }
        
        .contact-method {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 15px 20px;
            background: rgba(255, 209, 220, 0.2);
            border-radius: var(--border-radius-small);
            border: 1px solid rgba(255, 209, 220, 0.3);
            flex: 1 1 200px;
            justify-content: center;
            transition: all 0.3s ease;
            backdrop-filter: blur(5px);
        }
        
        .contact-method:hover {
            background: rgba(255, 209, 220, 0.3);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .contact-method i {
            color: var(--baby-pink);
            font-size: 1.4rem;
        }
        
        .contact-method span {
            font-family: var(--body-font);
            font-size: 1rem;
            color: var(--text-light);
            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
        }
        
        /* ENHANCED: FOOTER with gradient background */
        footer {
            background: linear-gradient(135deg, var(--dark-grey) 0%, #252525 100%);
            color: var(--text-light);
            padding: clamp(50px, 8vw, 80px) 0 40px;
            position: relative;
            overflow: hidden;
        }
        
        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--baby-pink), var(--pink-accent), var(--baby-pink), transparent);
        }
        
        .footer-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: flex-start;
            gap: 40px;
            position: relative;
            z-index: 1;
        }
        
        .footer-brand {
            flex: 1 1 300px;
        }
        
        .footer-logo {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(2.2rem, 5vw, 3.2rem);
            margin-bottom: 25px;
            color: var(--baby-pink);
            line-height: 1.2;
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .footer-logo::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 80px;
            height: 2px;
            background: var(--pink-accent);
            border-radius: 2px;
        }
        
        .footer-contact {
            flex: 1 1 300px;
        }
        
        .footer-contact h3 {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(1.8rem, 4vw, 2.2rem);
            margin-bottom: 25px;
            color: var(--baby-pink);
            line-height: 1.2;
            position: relative;
            padding-bottom: 15px;
        }
        
        .footer-contact h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 2px;
            background: var(--pink-accent);
            border-radius: 2px;
        }
        
        .contact-info {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 18px;
        }
        
        .contact-info li {
            display: flex;
            align-items: center;
            gap: 15px;
            font-family: var(--body-font);
            padding: 10px 15px;
            border-radius: var(--border-radius-small);
            background: rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
        }
        
        .contact-info li:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateX(5px);
        }
        
        .contact-info i {
            color: var(--pink-accent);
            font-size: 1.2rem;
            width: 35px;
            height: 35px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 209, 220, 0.1);
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .contact-info li:hover i {
            background: var(--pink-accent);
            color: var(--dark-grey);
            transform: scale(1.1);
        }
        
        .footer-social {
            flex: 1 1 300px;
        }
        
        .footer-social h3 {
            font-family: var(--accent-font);
            font-weight: 400;
            font-size: clamp(1.8rem, 4vw, 2.2rem);
            margin-bottom: 25px;
            color: var(--baby-pink);
            line-height: 1.2;
            position: relative;
            padding-bottom: 15px;
        }
        
        .footer-social h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 2px;
            background: var(--pink-accent);
            border-radius: 2px;
        }
        
        .social-icons {
            display: flex;
            gap: 20px;
            margin-bottom: 35px;
        }
        
        .social-icons a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 55px;
            height: 55px;
            background: rgba(255, 255, 255, 0.08);
            border-radius: 50%;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 209, 220, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .social-icons a::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s ease;
        }
        
        .social-icons a:hover {
            background: var(--pink-accent);
            transform: translateY(-5px) scale(1.1);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .social-icons a:hover::before {
            left: 100%;
        }
        
        .social-icons a i {
            font-size: 1.4rem;
            color: var(--baby-pink);
            transition: all 0.3s ease;
        }
        
        .social-icons a:hover i {
            color: var(--dark-grey);
        }
        
        .copyright {
            width: 100%;
            text-align: center;
            margin-top: 60px;
            padding-top: 25px;
            border-top: 1px solid rgba(255, 209, 220, 0.2);
            font-size: 0.95rem;
            color: var(--baby-pink);
            font-family: var(--body-font);
            position: relative;
            z-index: 1;
        }
        
        /* ENHANCED: MODAL STYLES */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 1100;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }
        
        .modal-overlay.active {
            opacity: 1;
            visibility: visible;
        }
        
        .modal-content {
            background: linear-gradient(135deg, var(--soft-white) 0%, var(--grey-light) 100%);
            border-radius: var(--border-radius);
            padding: 50px;
            max-width: 500px;
            width: 90%;
            text-align: center;
            transform: translateY(-30px) scale(0.9);
            transition: all 0.4s ease;
            border: 2px solid transparent;
            background-clip: padding-box;
            background-image: 
                linear-gradient(var(--soft-white), var(--soft-white)),
                linear-gradient(135deg, var(--baby-pink), var(--pink-accent));
            background-origin: border-box;
            box-shadow: 
                0 25px 50px rgba(0, 0, 0, 0.3),
                0 0 0 1px rgba(255, 209, 220, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .modal-overlay.active .modal-content {
            transform: translateY(0) scale(1);
        }
        
        .modal-content::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255, 209, 220, 0.2), transparent);
            transform: rotate(45deg);
        }
        
        .modal-icon {
            font-size: 5rem;
            color: var(--pink-accent);
            margin-bottom: 25px;
            position: relative;
            z-index: 1;
            text-shadow: 0 5px 15px rgba(255, 182, 193, 0.3);
        }
        
        .modal-title {
            font-family: var(--accent-font);
            font-size: 3rem;
            color: var(--dark-grey);
            margin-bottom: 20px;
            position: relative;
            z-index: 1;
        }
        
        .modal-message {
            font-family: var(--body-font);
            color: var(--medium-grey);
            margin-bottom: 35px;
            line-height: 1.6;
            white-space: pre-line;
            position: relative;
            z-index: 1;
            font-size: 1.05rem;
        }
        
        .modal-btn {
            background: linear-gradient(135deg, var(--pink-accent), var(--baby-pink));
            color: var(--dark-grey);
            border: none;
            padding: 15px 40px;
            border-radius: 25px;
            font-family: var(--body-font);
            font-weight: 500;
            cursor: pointer;
            transition: all 0.3s ease;
            font-size: 1.1rem;
            position: relative;
            z-index: 1;
            box-shadow: 0 5px 15px rgba(255, 182, 193, 0.4);
        }
        
        .modal-btn:hover {
            background: linear-gradient(135deg, var(--baby-pink), var(--pink-accent));
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 10px 25px rgba(255, 182, 193, 0.5);
        }
        
        /* ENHANCED: SCROLL TO TOP BUTTON */
        .scroll-top {
            position: fixed;
            bottom: 40px;
            right: 40px;
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, var(--pink-accent), var(--baby-pink));
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            transition: all 0.3s ease;
            opacity: 0;
            visibility: hidden;
            z-index: 100;
            border: 2px solid rgba(255, 255, 255, 0.3);
            box-shadow: 
                0 10px 25px rgba(255, 182, 193, 0.4),
                0 0 0 1px rgba(255, 209, 220, 0.3);
            transform: translateY(20px);
        }
        
        .scroll-top.visible {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
        }
        
        .scroll-top:hover {
            background: linear-gradient(135deg, var(--baby-pink), var(--pink-accent));
            transform: translateY(-5px) scale(1.1);
            box-shadow: 
                0 15px 35px rgba(255, 182, 193, 0.6),
                0 0 0 1px rgba(255, 209, 220, 0.4);
        }
        
        .scroll-top i {
            color: var(--dark-grey);
            font-size: 1.4rem;
            transition: transform 0.3s ease;
        }
        
        .scroll-top:hover i {
            transform: translateY(-2px);
        }
        
        /* ENHANCED: IMAGE LOADING STATE */
        .img-loading {
            background: linear-gradient(90deg, var(--light-grey) 25%, var(--baby-pink) 50%, var(--light-grey) 75%);
            background-size: 200% 100%;
            animation: loading 1.5s infinite;
            border-radius: inherit;
        }
        
        @keyframes loading {
            0% { background-position: 200% 0; }
            100% { background-position: -200% 0; }
        }
        
        /* ENHANCED: FORM VALIDATION */
        .form-control.error {
            border-color: #ff6b6b;
            background: rgba(255, 107, 107, 0.1);
            animation: shake 0.3s ease;
        }
        
        @keyframes shake {
            0%, 100% { transform: translateX(0); }
            25% { transform: translateX(-5px); }
            75% { transform: translateX(5px); }
        }
        
        .error-message {
            color: #ff6b6b;
            font-size: 0.9rem;
            margin-top: 8px;
            display: none;
            padding-left: 5px;
            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
        }
        
        .error-message.show {
            display: block;
            animation: fadeIn 0.3s ease;
        }
        
        /* ENHANCED: GALLERY LOADING */
        .gallery-loading {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, var(--light-grey), var(--soft-white));
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: inherit;
            z-index: 2;
        }
        
        .gallery-loading i {
            color: var(--pink-accent);
            font-size: 2.5rem;
            animation: spin 1s linear infinite;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* RESPONSIVE BREAKPOINTS */
        
        /* Tablet Styles (768px - 1024px) */
        @media screen and (max-width: 1024px) {
            header {
                height: var(--header-height-tablet);
            }
            
            .header-container {
                padding: 0 25px;
            }
            
            .logo {
                font-size: 2.5rem;
            }
            
            .nav-desktop .nav-links {
                gap: 20px;
            }
            
            .nav-desktop .btn {
                padding: 12px 24px;
                font-size: 15px;
            }
            
            .hero {
                min-height: 550px;
            }
            
            .about-container {
                gap: 40px;
            }
            
            .grid-container {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .modal-content {
                padding: 40px;
            }
            
            .scroll-top {
                bottom: 30px;
                right: 30px;
                width: 55px;
                height: 55px;
            }
            
            .container::before,
            .container::after {
                display: none;
            }
        }
        
        /* Mobile Styles (up to 768px) */
        @media screen and (max-width: 768px) {
            header {
                height: var(--header-height-mobile);
            }
            
            .header-container {
                padding: 0 20px;
            }
            
            .nav-desktop {
                display: none;
            }
            
            .hamburger {
                display: flex;
            }
            
            .logo {
                font-size: 2.2rem;
            }
            
            .hero {
                min-height: 500px;
                background-attachment: scroll;
            }
            
            .hero-content {
                margin-top: 40px;
            }
            
            .about-container {
                flex-direction: column;
            }
            
            .about-info-card {
                order: -1;
            }
            
            .grid-container {
                grid-template-columns: 1fr;
            }
            
            .form-row .form-group {
                flex: 1 1 100%;
            }
            
            .booking-contact-info {
                flex-direction: column;
            }
            
            .contact-method {
                flex: 1 1 100%;
            }
            
            .footer-container {
                flex-direction: column;
                gap: 40px;
            }
            
            .gallery-slide {
                width: 280px;
                height: 280px;
            }
            
            .modal-content {
                padding: 30px;
                width: 95%;
            }
            
            .modal-title {
                font-size: 2.5rem;
            }
            
            .modal-icon {
                font-size: 4rem;
            }
            
            .scroll-top {
                bottom: 25px;
                right: 25px;
                width: 50px;
                height: 50px;
            }
            
            @keyframes scroll {
                0% {
                    transform: translateX(0);
                }
                100% {
                    transform: translateX(calc(-280px * 8));
                }
            }
        }
        
        /* Small Mobile Styles (up to 480px) */
        @media screen and (max-width: 480px) {
            .hero {
                min-height: 450px;
            }
            
            .hero-title {
                font-size: 3rem;
            }
            
            .hero-subtitle {
                font-size: 1.8rem;
                margin-bottom: 30px;
            }
            
            .hero-btn {
                padding: 14px 28px;
                font-size: 1.3rem;
            }
            
            .about-description {
                padding: 20px;
            }
            
            .about-info-card {
                padding: 25px;
            }
            
            .info-item {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
            
            .services-grid {
                grid-template-columns: 1fr;
            }
            
            .policy-item {
                padding: 25px 25px 25px 65px;
            }
            
            .policy-item::before {
                left: 22px;
            }
            
            .booking-form-container {
                padding: 25px;
            }
            
            .submit-btn {
                padding: 14px 35px;
                font-size: 1.4rem;
            }
            
            .gallery-slide {
                width: 250px;
                height: 250px;
            }
            
            .modal-content {
                padding: 25px;
            }
            
            .modal-title {
                font-size: 2.2rem;
            }
            
            .modal-btn {
                padding: 12px 35px;
            }
            
            .scroll-top {
                bottom: 20px;
                right: 20px;
                width: 45px;
                height: 45px;
            }
            
            @keyframes scroll {
                0% {
                    transform: translateX(0);
                }
                100% {
                    transform: translateX(calc(-250px * 8));
                }
            }
        }
        
        /* Large Desktop Styles (over 1440px) */
        @media screen and (min-width: 1440px) {
            .container {
                max-width: 1400px;
            }
            
            .hero {
                max-height: 1000px;
            }
            
            .grid-container {
                grid-template-columns: repeat(4, 1fr);
            }
            
            .services-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }
        
        /* Touch device optimizations */
        @media (hover: none) and (pointer: coarse) {
            .service-card:hover {
                transform: none;
            }
            
            .gallery-item:hover {
                transform: none;
            }
            
            .btn:hover, .hero-btn:hover, .submit-btn:hover {
                transform: none;
            }
            
            .nav-links a:hover:after {
                width: 0;
            }
            
            .social-icons a:hover {
                transform: none;
            }
            
            .policy-item:hover {
                transform: none;
            }
            
            .contact-method:hover {
                transform: none;
            }
        }
        
        /* Reduced motion preferences */
        @media (prefers-reduced-motion: reduce) {
            * {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
            }
            
            .gallery-slider {
                animation: none;
            }
            
            .img-loading {
                animation: none;
            }
            
            .hero-particles {
                display: none;
            }
            
            .instagram-text {
                animation: none;
            }
        }
    </style>
</head>
<body>
    <!-- ENHANCED: SCROLL TO TOP BUTTON -->
    <div class="scroll-top" id="scrollTop" aria-label="Scroll to top">
        <i class="fas fa-chevron-up"></i>
    </div>
    
    <!-- HEADER -->
    <header id="main-header">
        <div class="header-container">
            <!-- Logo WITHOUT pink slash background -->
            <div class="logo" data-page="home">Nails By Lupita</div>
            
            <!-- Desktop Navigation -->
            <div class="nav-desktop">
                <div class="nav-center">
                    <nav>
                        <ul class="nav-links">
                            <li><a href="#" class="nav-link active-page" data-page="home">Home</a></li>
                            <li><a href="#" class="nav-link" data-page="gallery">Gallery</a></li>
                            <li><a href="#" class="nav-link" data-page="booking">Booking</a></li>
                        </ul>
                    </nav>
                    <div class="divider"></div>
                    <a href="#" class="btn" data-page="booking">Book Now</a>
                </div>
            </div>
            
            <!-- Mobile Hamburger Menu -->
            <button class="hamburger" id="hamburger" aria-label="Menu">
                <span></span>
                <span></span>
                <span></span>
            </button>
        </div>
        
        <!-- Mobile Menu -->
        <div class="mobile-menu" id="mobile-menu">
            <ul class="mobile-links">
                <li><a href="#" class="nav-link active-page" data-page="home">Home</a></li>
                <li><a href="#" class="nav-link" data-page="gallery">Gallery</a></li>
                <li><a href="#" class="nav-link" data-page="booking">Booking</a></li>
            </ul>
            <div class="mobile-menu-btn">
                <a href="#" class="btn" data-page="booking">Book Now</a>
            </div>
        </div>
    </header>

    <!-- HOME PAGE -->
    <div class="page active" id="home-page">
        <!-- HERO SECTION -->
        <section class="hero" id="home">
            <!-- Animated particles -->
            <div class="hero-particles" id="heroParticles"></div>
            <div class="hero-overlay"></div>
            <div class="hero-content">
                <h1 class="hero-title">Nails By Lupita</h1>
                <p class="hero-subtitle">Book Appointment</p>
                <a href="#" class="btn hero-btn" data-page="booking">Book Appointment</a>
            </div>
        </section>

        <!-- ABOUT SECTION -->
        <section class="about" id="about">
            <div class="container about-container">
                <div class="about-text">
                    <h2 class="about-title">Heyy! I'm Lupita</h2>
                    <p class="about-description">
                        Hope all is well! Welcome to my business page! My name is <span class="about-highlight">Lupita Castillo</span> - I'm a local but private Nail and Toe tech. I also specialize in <span class="about-highlight">piercings and lashes</span>.
                    </p>
                    <p class="about-description">
                        I'm located in <span class="about-highlight">Reidsville, GA</span>. You can contact me through Facebook or here if you want to see more of my work - it's all posted on Instagram. For faster response, contact my business number: <span class="about-highlight">(912-401-3684)</span>.
                    </p>
                    <p class="about-description">
                        I'm here to make sure you get a great experience if you don't want to go to a salon. With that being said, I am a <span class="about-highlight">home-based nail tech</span> - I do nails in my home. If that's something you're interested in, my policies will be strictly enforced.
                    </p>
                    <p class="about-description">
                        Also keep in mind - just because I'm a private at-home nail tech does <span class="about-highlight">NOT</span> mean I'm dirt cheap! My work is <span class="about-highlight">long-lasting, and very affordable</span>, done with care, and my work will not be rushed.
                    </p>
                    <p class="about-description">
                        Thank you so much for reaching out and trusting me. I'll be in contact as soon as possible 💗
                    </p>
                </div>
                
                <!-- INFO CARD (Replacing Image) -->
                <div class="about-info-card">
                    <h3 class="info-title">Contact & Info</h3>
                    <div class="info-details">
                        <div class="info-item">
                            <i class="fas fa-user"></i>
                            <div class="info-content">
                                <h4>Name</h4>
                                <p>Lupita Castillo</p>
                            </div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-map-marker-alt"></i>
                            <div class="info-content">
                                <h4>Location</h4>
                                <p>Reidsville, GA</p>
                            </div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-phone"></i>
                            <div class="info-content">
                                <h4>Business Phone</h4>
                                <p>912-401-3684</p>
                            </div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-envelope"></i>
                            <div class="info-content">
                                <h4>Email</h4>
                                <p>cluptiaskyla@gmail.com</p>
                            </div>
                        </div>
                        <div class="info-item">
                            <i class="fab fa-instagram"></i>
                            <div class="info-content">
                                <h4>Instagram</h4>
                                <p>@nailssbygloxn</p>
                            </div>
                        </div>
                        <div class="info-item">
                            <i class="fab fa-facebook"></i>
                            <div class="info-content">
                                <h4>Facebook</h4>
                                <p>Lupita Castillo</p>
                            </div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-home"></i>
                            <div class="info-content">
                                <h4>Service Type</h4>
                                <p>Home-Based Nail Tech</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SERVICES SECTION -->
        <section class="services" id="services">
            <div class="container">
                <h2 class="section-title">My Services<span>Premium Beauty Services</span></h2>
                <div class="services-grid">
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-gem"></i>
                        </div>
                        <h3 class="service-title">Nail Services</h3>
                        <p class="service-description">Acrylic sets, custom nail art, fills, and removals. Beautiful, durable work done with care.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-spa"></i>
                        </div>
                        <h3 class="service-title">Toe Services</h3>
                        <p class="service-description">Pedicures, toe nail art, and maintenance. Complete foot care with attention to detail.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-eye"></i>
                        </div>
                        <h3 class="service-title">Lash Services</h3>
                        <p class="service-description">Eyelash extensions, fills, and maintenance. Enhance your natural beauty.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-gem"></i>
                        </div>
                        <h3 class="service-title">Piercings</h3>
                        <p class="service-description">Professional piercing services with proper sterilization and aftercare guidance.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- GALLERY PREVIEW -->
        <section class="gallery-preview" id="gallery-preview">
            <div class="container">
                <h2 class="section-title">Recent Work<span>Featured Designs</span></h2>
                <div class="gallery-slider-container">
                    <div class="gallery-slider" id="gallery-slider">
                        <!-- Gallery images will be dynamically loaded -->
                    </div>
                </div>
                <div class="gallery-link" data-page="gallery">
                    View Full Gallery
                    <i class="fas fa-arrow-right"></i>
                </div>
            </div>
        </section>

        <!-- POLICIES SECTION -->
        <section class="policies" id="policies">
            <div class="container policies-container">
                <h2 class="section-title">Booking Policies<span>Important Information</span></h2>
                
                <div class="policy-item">
                    <h3 class="policy-title"><i class="fas fa-calendar-check"></i> Booking Requirements</h3>
                    <p class="policy-text">A deposit is required to secure your appointment. No deposit means no appointment will be scheduled.</p>
                </div>
                
                <div class="policy-item">
                    <h3 class="policy-title"><i class="fas fa-clock"></i> Arrival Time</h3>
                    <p class="policy-text">Please arrive on time for your appointment. There is a 10-minute grace period. After 10 minutes, a $10 late fee will apply.</p>
                </div>
                
                <div class="policy-item">
                    <h3 class="policy-title"><i class="fas fa-calendar-plus"></i> Sneeze-In Appointments</h3>
                    <p class="policy-text">Sneeze-in appointments (marked in black on the calendar) are available with an additional $15 fee.</p>
                </div>
                
                <div class="policy-item">
                    <h3 class="policy-title"><i class="fas fa-ban"></i> Deposit Policy</h3>
                    <p class="policy-text">Deposits are non-refundable unless I am unable to take you as a client. Rescheduling requires 24-hour notice.</p>
                </div>
                
                .policy-item {
                    <h3 class="policy-title"><i class="fas fa-home"></i> Home-Based Service</h3>
                    <p class="policy-text">I am a home-based nail tech operating in Reidsville, GA. My services are professional, clean, and private.</p>
                </div>
            </div>
        </section>

        <!-- INSTAGRAM PROMO -->
        <section class="instagram-promo">
            <div class="container">
                <p class="instagram-text">Post your nails & tag @nailssbygloxn</p>
                <p class="instagram-handle">Get $5 off your next set!</p>
            </div>
        </section>
    </div>

    <!-- GALLERY PAGE -->
    <div class="page" id="gallery-page">
        <section class="gallery-hero">
            <div class="container">
                <h1 class="gallery-title">Baddie Sets by Lupita</h1>
                <p class="gallery-subtitle">Luxury Nail Art Gallery</p>
            </div>
        </section>

        <section class="gallery-grid">
            <div class="container">
                <div class="grid-container" id="full-gallery">
                    <!-- Full gallery images will be loaded here -->
                </div>
            </div>
        </section>
    </div>

    <!-- BOOKING PAGE -->
    <div class="page" id="booking-page">
        <section class="booking-hero">
            <div class="booking-overlay"></div>
            <div class="booking-content">
                <h1 class="booking-title">Book Your Appointment</h1>
                
                <div class="booking-form-container">
                    <form id="bookingForm">
                        <div class="form-row">
                            <div class="form-group">
                                <label for="firstName" class="form-label">First Name</label>
                                <input type="text" id="firstName" class="form-control" placeholder="Your first name" required>
                                <div class="error-message" id="firstNameError">Please enter your first name</div>
                            </div>
                            <div class="form-group">
                                <label for="lastName" class="form-label">Last Name</label>
                                <input type="text" id="lastName" class="form-control" placeholder="Your last name" required>
                                <div class="error-message" id="lastNameError">Please enter your last name</div>
                            </div>
                        </div>
                        
                        <div class="form-row">
                            <div class="form-group">
                                <label for="phone" class="form-label">Phone Number</label>
                                <input type="tel" id="phone" class="form-control" placeholder="912-401-3684" required>
                                <div class="error-message" id="phoneError">Please enter a valid phone number</div>
                            </div>
                            <div class="form-group">
                                <label for="email" class="form-label">Email Address</label>
                                <input type="email" id="email" class="form-control" placeholder="cluptiaskyla@gmail.com" required>
                                <div class="error-message" id="emailError">Please enter a valid email address</div>
                            </div>
                        </div>
                        
                        <div class="form-group">
                            <label for="service" class="form-label">Select Service</label>
                            <select id="service" class="form-control" required>
                                <option value="" disabled selected>Choose a service</option>
                                <option value="nails-acrylic">Acrylic Nails</option>
                                <option value="nails-custom">Custom Nail Art</option>
                                <option value="toes">Toe Services</option>
                                <option value="lashes">Lash Services</option>
                                <option value="piercings">Piercings</option>
                                <option value="nails-fill">Nail Fill</option>
                                <option value="nails-removal">Nail Removal</option>
                                <option value="sneeze-in">Sneeze-In Appointment (+$15)</option>
                                <option value="other">Other/Consultation</option>
                            </select>
                            <div class="error-message" id="serviceError">Please select a service</div>
                        </div>
                        
                        <div class="form-row">
                            <div class="form-group">
                                <label for="date" class="form-label">Preferred Date</label>
                                <input type="date" id="date" class="form-control" required>
                                <div class="error-message" id="dateError">Please select a date</div>
                            </div>
                            <div class="form-group">
                                <label for="time" class="form-label">Preferred Time</label>
                                <select id="time" class="form-control" required>
                                    <option value="" disabled selected>Select time</option>
                                    <option value="9am">9:00 AM</option>
                                    <option value="10am">10:00 AM</option>
                                    <option value="11am">11:00 AM</option>
                                    <option value="12pm">12:00 PM</option>
                                    <option value="1pm">1:00 PM</option>
                                    <option value="2pm">2:00 PM</option>
                                    <option value="3pm">3:00 PM</option>
                                    <option value="4pm">4:00 PM</option>
                                    <option value="5pm">5:00 PM</option>
                                </select>
                                <div class="error-message" id="timeError">Please select a time</div>
                            </div>
                        </div>
                        
                        <div class="form-group">
                            <label for="notes" class="form-label">Additional Notes or Inspiration</label>
                            <textarea id="notes" class="form-control" rows="4" placeholder="Any specific designs, colors, or details you'd like to share..."></textarea>
                        </div>
                        
                        <div class="form-submit">
                            <button type="submit" class="submit-btn">Submit Booking Request</button>
                        </div>
                    </form>
                    
                    <div class="booking-instructions">
                        <p><strong>Important Information:</strong></p>
                        <p>After submitting your booking request, you will receive a confirmation text or email within 24 hours. A deposit is required to secure your appointment time.</p>
                        <p>Please review our booking policies on the home page before submitting your request.</p>
                        
                        <div class="booking-contact-info">
                            <div class="contact-method">
                                <i class="fab fa-instagram"></i>
                                <span>@nailssbygloxn</span>
                            </div>
                            <div class="contact-method">
                                <i class="fas fa-phone"></i>
                                <span>912-401-3684</span>
                            </div>
                            <div class="contact-method">
                                <i class="fas fa-envelope"></i>
                                <span>cluptiaskyla@gmail.com</span>
                            </div>
                            <div class="contact-method">
                                <i class="fas fa-map-marker-alt"></i>
                                <span>Reidsville, GA</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- ENHANCED: BOOKING CONFIRMATION MODAL -->
    <div class="modal-overlay" id="confirmationModal">
        <div class="modal-content">
            <div class="modal-icon">
                <i class="fas fa-check-circle"></i>
            </div>
            <h2 class="modal-title">Booking Request Sent!</h2>
            <div class="modal-message" id="modalMessage">
                Your appointment request has been received.
            </div>
            <button class="modal-btn" id="modalCloseBtn">Okay</button>
        </div>
    </div>

    <!-- FOOTER -->
    <footer id="contact">
        <div class="container">
            <div class="footer-container">
                <div class="footer-brand">
                    <div class="footer-logo">Nails By Lupita</div>
                    <p>Home-based nail, toe, lash & piercing services in Reidsville, GA. Pretty things done right.</p>
                </div>
                
                <div class="footer-contact">
                    <h3>Contact Info</h3>
                    <ul class="contact-info">
                        <li><i class="fas fa-phone"></i> 912-401-3684</li>
                        <li><i class="fas fa-envelope"></i> cluptiaskyla@gmail.com</li>
                        <li><i class="fas fa-map-marker-alt"></i> Reidsville, GA</li>
                        <li><i class="fab fa-facebook"></i> Facebook: Lupita Castillo</li>
                    </ul>
                </div>
                
                <div class="footer-social">
                    <h3>Follow Me</h3>
                    <div class="social-icons">
                        <a href="https://instagram.com/nailssbygloxn" target="_blank" aria-label="Instagram">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="https://facebook.com" target="_blank" aria-label="Facebook">
                            <i class="fab fa-facebook"></i>
                        </a>
                        <a href="mailto:cluptiaskyla@gmail.com" aria-label="Email">
                            <i class="fas fa-envelope"></i>
                        </a>
                        <a href="tel:9124013684" aria-label="Phone">
                            <i class="fas fa-phone"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="copyright">
                &copy; 2023 Nails By Lupita. All rights reserved. | Home-based services in Reidsville, GA
            </div>
        </div>
    </footer>

    <script>
        // ENHANCED: Create animated particles for hero section
        function createParticles() {
            const container = document.getElementById('heroParticles');
            if (!container) return;
            
            const particleCount = window.innerWidth < 768 ? 20 : 40;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                
                // Random positioning
                const size = Math.random() * 4 + 2;
                const posX = Math.random() * 100;
                const delay = Math.random() * 15;
                const duration = Math.random() * 10 + 15;
                
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${posX}%`;
                particle.style.animationDelay = `${delay}s`;
                particle.style.animationDuration = `${duration}s`;
                
                container.appendChild(particle);
            }
        }
        
        // YOUR ACTUAL NAIL ART IMAGES (15 unique images)
        const galleryImageUrls = [
            'https://i.postimg.cc/9XgY6ghw/Screenshot-2026-01-30-230948.png',
            'https://i.postimg.cc/qBDxPDTN/Screenshot-2026-01-30-231010.png',
            'https://i.postimg.cc/nVSGySJj/Screenshot-2026-01-30-231020.png',
            'https://i.postimg.cc/VsZWxZ8b/Screenshot-2026-01-30-231038.png',
            'https://i.postimg.cc/bYV97Vhb/Screenshot-2026-01-30-231058.png',
            'https://i.postimg.cc/3rfFsfTF/Screenshot-2026-01-30-231110.png',
            'https://i.postimg.cc/bYV97VhQ/Screenshot-2026-01-30-231134.png',
            'https://i.postimg.cc/h4Z1kZBr/Screenshot-2026-01-30-231146.png',
            'https://i.postimg.cc/xjp3wp25/Screenshot-2026-01-30-231200.png',
            'https://i.postimg.cc/66bfkbXY/Screenshot-2026-01-30-231210.png',
            'https://i.postimg.cc/XN1kR1b1/Screenshot-2026-01-30-231224.png',
            'https://i.postimg.cc/PfVQgVj7/Screenshot-2026-01-30-231230.png',
            'https://i.postimg.cc/mZpyvp4x/Screenshot-2026-01-30-231241.png',
            'https://i.postimg.cc/zD2Fs2rs/Screenshot-2026-01-30-231306.png',
            'https://i.postimg.cc/gkwHmyzM/Screenshot-2026-01-30-231319.png'
        ];
        
        // Page navigation system
        const pages = {
            'home': document.getElementById('home-page'),
            'gallery': document.getElementById('gallery-page'),
            'booking': document.getElementById('booking-page')
        };
        
        const navLinks = document.querySelectorAll('.nav-link');
        const logo = document.querySelector('.logo');
        const header = document.getElementById('main-header');
        const heroSection = document.querySelector('.hero');
        const bookingHero = document.querySelector('.booking-hero');
        const scrollTopBtn = document.getElementById('scrollTop');
        const confirmationModal = document.getElementById('confirmationModal');
        const modalMessage = document.getElementById('modalMessage');
        const modalCloseBtn = document.getElementById('modalCloseBtn');
        
        // Enhanced function to switch pages
        function switchPage(pageId) {
            // Hide all pages
            Object.values(pages).forEach(page => {
                if (page.classList.contains('active')) {
                    page.style.opacity = '0';
                    page.style.transform = 'translateY(10px)';
                    setTimeout(() => {
                        page.classList.remove('active');
                        page.style.opacity = '';
                        page.style.transform = '';
                    }, 200);
                }
            });
            
            // Show selected page
            setTimeout(() => {
                pages[pageId].classList.add('active');
                pages[pageId].style.opacity = '0';
                pages[pageId].style.transform = 'translateY(10px)';
                requestAnimationFrame(() => {
                    pages[pageId].style.transition = 'opacity 0.3s ease, transform 0.3s ease';
                    pages[pageId].style.opacity = '1';
                    pages[pageId].style.transform = 'translateY(0)';
                });
                
                // Remove transition after animation completes
                setTimeout(() => {
                    pages[pageId].style.transition = '';
                }, 300);
            }, 200);
            
            // Update active nav link
            navLinks.forEach(link => {
                if (link.dataset.page === pageId) {
                    link.classList.add('active-page');
                } else {
                    link.classList.remove('active-page');
                }
            });
            
            // Update header transparency based on page
            updateHeaderTransparency();
            
            // Scroll to top with smooth behavior
            window.scrollTo({ top: 0, behavior: 'smooth' });
            
            // Load gallery images if on gallery page
            if (pageId === 'gallery') {
                loadFullGallery();
            }
            
            // Load preview slider if on home page
            if (pageId === 'home') {
                loadGallerySlider();
            }
            
            // Set minimum date for booking form to today
            if (pageId === 'booking') {
                const today = new Date().toISOString().split('T')[0];
                document.getElementById('date').min = today;
                
                // Set placeholder date to tomorrow
                const tomorrow = new Date();
                tomorrow.setDate(tomorrow.getDate() + 1);
                const tomorrowFormatted = tomorrow.toISOString().split('T')[0];
                document.getElementById('date').value = tomorrowFormatted;
            }
            
            // Update URL hash
            history.pushState(null, '', `#${pageId}`);
        }
        
        // Enhanced gallery slider with lazy loading
        function loadGallerySlider() {
            const slider = document.getElementById('gallery-slider');
            if (!slider) return;
            
            slider.innerHTML = '';
            
            // Create slides for smooth scrolling
            const numSlides = window.innerWidth < 768 ? 6 : 8;
            for (let i = 0; i < numSlides; i++) {
                const imgIndex = i % galleryImageUrls.length;
                const slide = document.createElement('div');
                slide.className = 'gallery-slide';
                slide.setAttribute('data-index', i);
                
                // Create loading placeholder
                const loadingDiv = document.createElement('div');
                loadingDiv.className = 'gallery-loading';
                loadingDiv.innerHTML = '<i class="fas fa-spinner"></i>';
                
                const img = document.createElement('img');
                img.src = galleryImageUrls[imgIndex];
                img.alt = `Luxury nail design ${i+1} by Nails By Lupita`;
                img.loading = 'lazy';
                img.style.opacity = '0';
                img.style.transition = 'opacity 0.3s ease';
                
                // Handle image load
                img.onload = () => {
                    img.style.opacity = '1';
                    if (loadingDiv.parentNode) {
                        loadingDiv.remove();
                    }
                };
                
                // Handle image error
                img.onerror = () => {
                    img.src = 'data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="320" height="320" viewBox="0 0 320 320"><rect width="320" height="320" fill="%23F5F5F5"/><text x="160" y="160" font-family="Arial" font-size="16" text-anchor="middle" fill="%234A4A4A">Image not available</text></svg>';
                    img.alt = 'Image not available';
                    img.style.opacity = '1';
                    if (loadingDiv.parentNode) {
                        loadingDiv.remove();
                    }
                };
                
                slide.appendChild(loadingDiv);
                slide.appendChild(img);
                slider.appendChild(slide);
            }
        }
        
        // Enhanced full gallery with lazy loading
        function loadFullGallery() {
            const galleryGrid = document.getElementById('full-gallery');
            if (!galleryGrid) return;
            
            galleryGrid.innerHTML = '';
            
            // Create all gallery items
            for (let i = 0; i < galleryImageUrls.length; i++) {
                const item = document.createElement('div');
                item.className = 'gallery-item';
                item.setAttribute('data-index', i);
                
                // Create loading placeholder
                const loadingDiv = document.createElement('div');
                loadingDiv.className = 'gallery-loading';
                loadingDiv.innerHTML = '<i class="fas fa-spinner"></i>';
                
                const img = document.createElement('img');
                img.src = galleryImageUrls[i];
                img.alt = `Premium nail design ${i+1} by Nails By Lupita in Reidsville, GA`;
                img.loading = 'lazy';
                img.style.opacity = '0';
                img.style.transition = 'opacity 0.3s ease';
                
                // Handle image load
                img.onload = () => {
                    img.style.opacity = '1';
                    if (loadingDiv.parentNode) {
                        loadingDiv.remove();
                    }
                };
                
                // Handle image error
                img.onerror = () => {
                    img.src = 'data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="320" height="350" viewBox="0 0 320 350"><rect width="320" height="350" fill="%23F5F5F5"/><text x="160" y="175" font-family="Arial" font-size="16" text-anchor="middle" fill="%234A4A4A">Image not available</text></svg>';
                    img.alt = 'Image not available';
                    img.style.opacity = '1';
                    if (loadingDiv.parentNode) {
                        loadingDiv.remove();
                    }
                };
                
                item.appendChild(loadingDiv);
                item.appendChild(img);
                galleryGrid.appendChild(item);
            }
        }
        
        // Enhanced header transparency update
        function updateHeaderTransparency() {
            const currentPage = Object.keys(pages).find(key => pages[key].classList.contains('active'));
            
            if (currentPage === 'home') {
                if (window.scrollY < heroSection.offsetHeight - 100) {
                    header.classList.add('header-transparent');
                } else {
                    header.classList.remove('header-transparent');
                }
            } else if (currentPage === 'booking') {
                if (window.scrollY < bookingHero.offsetHeight - 100) {
                    header.classList.add('header-transparent');
                } else {
                    header.classList.remove('header-transparent');
                }
            } else {
                header.classList.remove('header-transparent');
            }
        }
        
        // Enhanced form validation
        function validateForm() {
            let isValid = true;
            
            // Reset all errors
            document.querySelectorAll('.error-message').forEach(error => {
                error.classList.remove('show');
            });
            
            document.querySelectorAll('.form-control').forEach(input => {
                input.classList.remove('error');
            });
            
            // Validate first name
            const firstName = document.getElementById('firstName');
            if (!firstName.value.trim()) {
                isValid = false;
                firstName.classList.add('error');
                document.getElementById('firstNameError').classList.add('show');
            }
            
            // Validate last name
            const lastName = document.getElementById('lastName');
            if (!lastName.value.trim()) {
                isValid = false;
                lastName.classList.add('error');
                document.getElementById('lastNameError').classList.add('show');
            }
            
            // Validate phone
            const phone = document.getElementById('phone');
            const phoneRegex = /^[\+]?[1-9][\d]{0,15}$/;
            if (!phoneRegex.test(phone.value.replace(/[\s\-\(\)]/g, ''))) {
                isValid = false;
                phone.classList.add('error');
                document.getElementById('phoneError').classList.add('show');
            }
            
            // Validate email
            const email = document.getElementById('email');
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailRegex.test(email.value)) {
                isValid = false;
                email.classList.add('error');
                document.getElementById('emailError').classList.add('show');
            }
            
            // Validate service
            const service = document.getElementById('service');
            if (!service.value) {
                isValid = false;
                service.classList.add('error');
                document.getElementById('serviceError').classList.add('show');
            }
            
            // Validate date
            const date = document.getElementById('date');
            if (!date.value) {
                isValid = false;
                date.classList.add('error');
                document.getElementById('dateError').classList.add('show');
            }
            
            // Validate time
            const time = document.getElementById('time');
            if (!time.value) {
                isValid = false;
                time.classList.add('error');
                document.getElementById('timeError').classList.add('show');
            }
            
            return isValid;
        }
        
        // Enhanced modal functions
        function showModal(message) {
            modalMessage.textContent = message;
            confirmationModal.classList.add('active');
            document.body.style.overflow = 'hidden';
        }
        
        function hideModal() {
            confirmationModal.classList.remove('active');
            document.body.style.overflow = 'auto';
        }
        
        // Initialize page navigation
        navLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                switchPage(link.dataset.page);
                
                // Close mobile menu if open
                mobileMenu.classList.remove('active');
                hamburger.classList.remove('active');
                document.body.style.overflow = 'auto';
            });
        });
        
        // Logo click goes to home
        logo.addEventListener('click', (e) => {
            e.preventDefault();
            switchPage('home');
        });
        
        // Book Now buttons
        document.querySelectorAll('.btn[data-page], .gallery-link').forEach(btn => {
            btn.addEventListener('click', (e) => {
                e.preventDefault();
                switchPage(btn.dataset.page);
                
                // Close mobile menu if open
                mobileMenu.classList.remove('active');
                hamburger.classList.remove('active');
                document.body.style.overflow = 'auto';
            });
        });
        
        // Mobile menu toggle
        const hamburger = document.getElementById('hamburger');
        const mobileMenu = document.getElementById('mobile-menu');
        
        hamburger.addEventListener('click', () => {
            mobileMenu.classList.toggle('active');
            hamburger.classList.toggle('active');
            document.body.style.overflow = mobileMenu.classList.contains('active') ? 'hidden' : 'auto';
        });
        
        // Close mobile menu when clicking a link
        const mobileLinks = document.querySelectorAll('.mobile-links a, .mobile-menu-btn a');
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.remove('active');
                hamburger.classList.remove('active');
                document.body.style.overflow = 'auto';
            });
        });
        
        // Close mobile menu when clicking outside
        document.addEventListener('click', (e) => {
            if (mobileMenu.classList.contains('active') && 
                !mobileMenu.contains(e.target) && 
                !hamburger.contains(e.target)) {
                mobileMenu.classList.remove('active');
                hamburger.classList.remove('active');
                document.body.style.overflow = 'auto';
            }
        });
        
        // Modal close button
        modalCloseBtn.addEventListener('click', hideModal);
        
        // Close modal when clicking outside
        confirmationModal.addEventListener('click', (e) => {
            if (e.target === confirmationModal) {
                hideModal();
            }
        });
        
        // Close modal with Escape key
        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape' && confirmationModal.classList.contains('active')) {
                hideModal();
            }
        });
        
        // Enhanced booking form submission
        document.getElementById('bookingForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Validate form
            if (!validateForm()) {
                // Scroll to first error
                const firstError = document.querySelector('.error-message.show');
                if (firstError) {
                    firstError.scrollIntoView({ behavior: 'smooth', block: 'center' });
                }
                return;
            }
            
            // Get form values
            const firstName = document.getElementById('firstName').value;
            const lastName = document.getElementById('lastName').value;
            const phone = document.getElementById('phone').value;
            const email = document.getElementById('email').value;
            const service = document.getElementById('service').value;
            const date = document.getElementById('date').value;
            const time = document.getElementById('time').value;
            const notes = document.getElementById('notes').value;
            
            // Format date for display
            const dateObj = new Date(date);
            const formattedDate = dateObj.toLocaleDateString('en-US', { 
                weekday: 'long', 
                year: 'numeric', 
                month: 'long', 
                day: 'numeric' 
            });
            
            // Format time for display
            const timeDisplay = {
                '9am': '9:00 AM',
                '10am': '10:00 AM', 
                '11am': '11:00 AM',
                '12pm': '12:00 PM',
                '1pm': '1:00 PM',
                '2pm': '2:00 PM',
                '3pm': '3:00 PM',
                '4pm': '4:00 PM',
                '5pm': '5:00 PM'
            }[time];
            
            // Service display names
            const serviceDisplay = {
                'nails-acrylic': 'Acrylic Nails',
                'nails-custom': 'Custom Nail Art',
                'toes': 'Toe Services',
                'lashes': 'Lash Services',
                'piercings': 'Piercings',
                'nails-fill': 'Nail Fill',
                'nails-removal': 'Nail Removal',
                'sneeze-in': 'Sneeze-In Appointment (+$15)',
                'other': 'Other/Consultation'
            }[service];
            
            // Create confirmation message
            const confirmationMessage = `Thank you, ${firstName} ${lastName}!\n\n✅ Your booking request has been received.\n\n📋 Appointment Details:\n• Service: ${serviceDisplay}\n• Date: ${formattedDate}\n• Time: ${timeDisplay}\n• Contact: ${phone}, ${email}\n\n📝 Notes: ${notes || 'None provided'}\n\n📍 Location: Home-based service in Reidsville, GA\n\nYou will receive a confirmation text/email within 24 hours. A deposit is required to secure your appointment.\n\nFor questions, contact:\n📱 Phone: 912-401-3684\n📧 Email: cluptiaskyla@gmail.com\n📸 Instagram: @nailssbygloxn\n📘 Facebook: Lupita Castillo`;
            
            // Show confirmation modal
            showModal(confirmationMessage);
            
            // Reset form
            this.reset();
            
            // Set minimum date to today
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('date').min = today;
            
            // Set placeholder date to tomorrow
            const tomorrow = new Date();
            tomorrow.setDate(tomorrow.getDate() + 1);
            const tomorrowFormatted = tomorrow.toISOString().split('T')[0];
            document.getElementById('date').value = tomorrowFormatted;
            
            // Auto-fill user's contact info for convenience
            document.getElementById('phone').value = phone;
            document.getElementById('email').value = email;
        });
        
        // Scroll to top button functionality
        scrollTopBtn.addEventListener('click', () => {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });
        
        // Show/hide scroll to top button
        function updateScrollTopButton() {
            if (window.scrollY > 500) {
                scrollTopBtn.classList.add('visible');
            } else {
                scrollTopBtn.classList.remove('visible');
            }
        }
        
        // Update header transparency and scroll button on scroll
        let scrollTimeout;
        window.addEventListener('scroll', () => {
            updateHeaderTransparency();
            updateScrollTopButton();
            
            // Debounce scroll events for performance
            clearTimeout(scrollTimeout);
            scrollTimeout = setTimeout(updateHeaderTransparency, 100);
        });
        
        // Handle window resize for responsive adjustments
        let resizeTimer;
        window.addEventListener('resize', () => {
            clearTimeout(resizeTimer);
            resizeTimer = setTimeout(() => {
                // Reload gallery slider on resize
                if (document.getElementById('home-page').classList.contains('active')) {
                    loadGallerySlider();
                }
                // Recalculate header transparency
                updateHeaderTransparency();
                // Recreate particles
                const heroParticles = document.getElementById('heroParticles');
                if (heroParticles) {
                    heroParticles.innerHTML = '';
                    createParticles();
                }
            }, 250);
        });
        
        // Initialize the page
        window.addEventListener('DOMContentLoaded', () => {
            // Create particles for hero section
            createParticles();
            
            // Load gallery slider on home page
            loadGallerySlider();
            
            // Load full gallery initially
            loadFullGallery();
            
            // Set initial header transparency
            updateHeaderTransparency();
            
            // Set minimum date for booking form to today
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('date').min = today;
            
            // Set placeholder date to tomorrow
            const tomorrow = new Date();
            tomorrow.setDate(tomorrow.getDate() + 1);
            const tomorrowFormatted = tomorrow.toISOString().split('T')[0];
            document.getElementById('date').value = tomorrowFormatted;
            
            // Check if there's a hash in the URL to navigate to specific page
            const hash = window.location.hash.substring(1);
            if (hash && pages[hash]) {
                switchPage(hash);
            }
            
            // Handle browser back/forward buttons
            window.addEventListener('popstate', () => {
                const hash = window.location.hash.substring(1);
                if (hash && pages[hash]) {
                    switchPage(hash);
                }
            });
            
            // Add touch event listeners for mobile
            if ('ontouchstart' in window) {
                document.addEventListener('touchstart', function() {}, {passive: true});
            }
        });
        
        // Enhanced form input validation on blur
        document.querySelectorAll('.form-control').forEach(input => {
            input.addEventListener('blur', function() {
                if (this.value.trim() && this.classList.contains('error')) {
                    this.classList.remove('error');
                    const errorId = this.id + 'Error';
                    const errorElement = document.getElementById(errorId);
                    if (errorElement) {
                        errorElement.classList.remove('show');
                    }
                }
            });
            
            input.addEventListener('input', function() {
                if (this.value.trim() && this.classList.contains('error')) {
                    this.classList.remove('error');
                    const errorId = this.id + 'Error';
                    const errorElement = document.getElementById(errorId);
                    if (errorElement) {
                        errorElement.classList.remove('show');
                    }
                }
            });
        });
        
        // Enhanced smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                if (this.getAttribute('href') === '#') return;
                
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    const headerHeight = document.querySelector('header').offsetHeight;
                    const targetPosition = targetElement.getBoundingClientRect().top + window.pageYOffset - headerHeight;
                    
                    window.scrollTo({
                        top: targetPosition,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Prevent zoom on double tap for mobile
        let lastTouchEnd = 0;
        document.addEventListener('touchend', function(event) {
            const now = (new Date()).getTime();
            if (now - lastTouchEnd <= 300) {
                event.preventDefault();
            }
            lastTouchEnd = now;
        }, false);
        
        // Add keyboard navigation support
        document.addEventListener('keydown', (e) => {
            // Close mobile menu with Escape
            if (e.key === 'Escape' && mobileMenu.classList.contains('active')) {
                mobileMenu.classList.remove('active');
                hamburger.classList.remove('active');
                document.body.style.overflow = 'auto';
            }
            
            // Navigate pages with arrow keys when focused
            if (e.key === 'ArrowRight' || e.key === 'ArrowLeft') {
                const currentPage = Object.keys(pages).find(key => pages[key].classList.contains('active'));
                const pageOrder = ['home', 'gallery', 'booking'];
                const currentIndex = pageOrder.indexOf(currentPage);
                
                if (e.key === 'ArrowRight' && currentIndex < pageOrder.length - 1) {
                    switchPage(pageOrder[currentIndex + 1]);
                } else if (e.key === 'ArrowLeft' && currentIndex > 0) {
                    switchPage(pageOrder[currentIndex - 1]);
                }
            }
        });
    </script>
</body>
</html>

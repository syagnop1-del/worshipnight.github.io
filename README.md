<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WN'25 - Worship Night 2025 | Jesus: Worthy Forever</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0a0a0a;
            line-height: 1.6;
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
                radial-gradient(circle at 20% 30%, rgba(139, 0, 0, 0.2) 0%, transparent 50%),
                radial-gradient(circle at 80% 70%, rgba(255, 107, 107, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 50% 50%, rgba(255, 165, 0, 0.08) 0%, transparent 70%);
            pointer-events: none;
            z-index: 0;
            animation: morphBackground 15s ease-in-out infinite;
        }

        @keyframes morphBackground {
            0%, 100% {
                transform: scale(1) rotate(0deg);
                opacity: 1;
            }
            50% {
                transform: scale(1.1) rotate(5deg);
                opacity: 0.8;
            }
        }

        body::after {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(rgba(139, 0, 0, 0.04) 1px, transparent 1px),
                linear-gradient(90deg, rgba(139, 0, 0, 0.04) 1px, transparent 1px);
            background-size: 50px 50px;
            pointer-events: none;
            z-index: 0;
            animation: gridSlide 20s linear infinite;
        }

        @keyframes gridSlide {
            0% {
                transform: translate(0, 0);
            }
            100% {
                transform: translate(50px, 50px);
            }
        }

        /* Hero Banner - Full Screen */
        .hero-banner {
            width: 100%;
            height: 100vh;
            position: relative;
            overflow: hidden;
            background: #000;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 1;
        }

        .hero-banner img {
            width: 100%;
            height: 100%;
            display: block;
            object-fit: cover;
            object-position: center;
        }

        /* Hero Button Overlay */
        .hero-overlay {
            position: absolute;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            z-index: 10;
            text-align: center;
        }

        .hero-btn {
            display: inline-block;
            background: linear-gradient(135deg, #ffa500 0%, #ff6b6b 100%);
            color: white;
            padding: 18px 70px;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.2em;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 8px 30px rgba(255, 165, 0, 0.4);
            text-transform: uppercase;
            letter-spacing: 2px;
            animation: bounce 2s infinite;
            white-space: nowrap;
        }

        .hero-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 40px rgba(255, 165, 0, 0.6);
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }

        /* Desktop/Mobile banner toggle */
        .hero-banner .desktop-banner {
            display: block;
        }

        .hero-banner .mobile-banner {
            display: none;
        }

        /* Smooth scroll behavior */
        html {
            scroll-behavior: smooth;
        }

        /* Container */
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 1;
        }

        /* ===== AESTHETIC POSTER STYLES ===== */
        .aesthetic-poster {
            width: 100%;
            max-width: 900px;
            margin: 60px auto;
            background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%);
            border-radius: 30px;
            overflow: hidden;
            box-shadow: 
                0 30px 80px rgba(139, 0, 0, 0.5),
                0 0 0 1px rgba(255, 165, 0, 0.2),
                inset 0 1px 0 rgba(255, 255, 255, 0.9);
            position: relative;
            border: 4px solid transparent;
            background-clip: padding-box;
            animation: floatPoster 6s ease-in-out infinite;
        }

        @keyframes floatPoster {
            0%, 100% {
                transform: translateY(0px) scale(1);
            }
            50% {
                transform: translateY(-8px) scale(1.01);
            }
        }

        .aesthetic-poster::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(135deg, #ffa500, #ff6b6b, #ffa500);
            border-radius: 30px;
            z-index: -1;
            animation: rotateBorder 4s linear infinite;
            opacity: 0.6;
        }

        @keyframes rotateBorder {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }

        .aesthetic-poster::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(
                90deg,
                transparent,
                rgba(255, 255, 255, 0.3),
                transparent
            );
            animation: shimmer 3s ease-in-out infinite;
        }

        @keyframes shimmer {
            0% {
                left: -100%;
            }
            50%, 100% {
                left: 100%;
            }
        }

        .poster-content {
            padding: 70px 60px;
            position: relative;
            z-index: 1;
        }

        .poster-header {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 40px;
            padding-bottom: 30px;
            border-bottom: 4px solid transparent;
            background: linear-gradient(white, white) padding-box,
                        linear-gradient(90deg, #ffa500, #ff6b6b, #ffa500) border-box;
            border-image: linear-gradient(90deg, #ffa500, #ff6b6b, #ffa500) 1;
            border-width: 0 0 4px 0;
            border-style: solid;
            animation: borderFlow 3s linear infinite;
        }

        @keyframes borderFlow {
            0% {
                border-image-source: linear-gradient(90deg, #ffa500, #ff6b6b, #ffa500);
            }
            50% {
                border-image-source: linear-gradient(90deg, #ff6b6b, #ffa500, #ff6b6b);
            }
            100% {
                border-image-source: linear-gradient(90deg, #ffa500, #ff6b6b, #ffa500);
            }
        }

        .poster-icon {
            font-size: 4em;
            filter: drop-shadow(0 5px 15px rgba(255, 165, 0, 0.4));
            animation: iconBounce 2s ease-in-out infinite;
        }

        @keyframes iconBounce {
            0%, 100% {
                transform: translateY(0px) rotate(0deg);
            }
            25% {
                transform: translateY(-10px) rotate(-5deg);
            }
            75% {
                transform: translateY(-5px) rotate(5deg);
            }
        }

        .poster-title {
            font-size: 4.5em;
            font-weight: 900;
            font-style: italic;
            background: linear-gradient(135deg, #ffa500, #ff8c00, #ff6b6b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-transform: uppercase;
            line-height: 0.9;
            letter-spacing: -3px;
            text-shadow: 3px 3px 0px rgba(0,0,0,0.1);
            animation: gradientText 3s ease-in-out infinite;
        }

        @keyframes gradientText {
            0%, 100% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
        }

        .poster-featured {
            background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
            padding: 50px;
            border-radius: 20px;
            margin: 30px 0;
            box-shadow: 
                0 15px 40px rgba(0,0,0,0.3),
                inset 0 -5px 20px rgba(255, 165, 0, 0.1),
                0 0 0 3px rgba(255, 165, 0, 0.2);
            position: relative;
            overflow: hidden;
        }

        .poster-featured::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: 
                radial-gradient(circle, rgba(255, 165, 0, 0.15) 0%, transparent 70%),
                radial-gradient(circle at 70% 70%, rgba(255, 107, 107, 0.1) 0%, transparent 60%);
        }

        .poster-featured::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 50%;
            height: 100%;
            background: linear-gradient(
                90deg,
                transparent,
                rgba(255, 165, 0, 0.1),
                transparent
            );
        }

        .featured-content {
            position: relative;
            z-index: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }

        .featured-main {
            font-size: 5.5em;
            font-weight: 900;
            color: white;
            font-style: italic;
            text-align: center;
            line-height: 0.9;
            text-shadow: 
                3px 3px 6px rgba(0,0,0,0.5),
                0 0 40px rgba(255, 165, 0, 0.4),
                0 0 80px rgba(255, 165, 0, 0.2);
            animation: glow 2s ease-in-out infinite;
        }

        @keyframes glow {
            0%, 100% {
                text-shadow: 
                    3px 3px 6px rgba(0,0,0,0.5),
                    0 0 40px rgba(255, 165, 0, 0.4),
                    0 0 80px rgba(255, 165, 0, 0.2);
            }
            50% {
                text-shadow: 
                    3px 3px 6px rgba(0,0,0,0.5),
                    0 0 50px rgba(255, 165, 0, 0.6),
                    0 0 100px rgba(255, 165, 0, 0.3);
            }
        }

        .featured-sub {
            font-size: 1.8em;
            color: #ffa500;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 3px;
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% {
                opacity: 0.9;
                transform: scale(1);
            }
            50% {
                opacity: 1;
                transform: scale(1.05);
            }
        }

        .poster-body {
            margin-top: 40px;
        }

        .body-section {
            margin: 30px 0;
        }

        .body-heading {
            font-size: 1.8em;
            font-weight: 900;
            color: #ff6b6b;
            text-transform: uppercase;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .body-text {
            font-size: 1.15em;
            color: #555;
            line-height: 1.8;
            font-weight: 500;
        }

        .body-text strong {
            color: #1a1a1a;
            font-weight: 700;
        }

        .highlight-box {
            background: #f8f9fa;
            color: #555;
            padding: 20px 30px;
            border-radius: 10px;
            text-align: center;
            font-weight: 600;
            font-size: 1.1em;
            margin: 30px 0;
            border: 2px solid #e0e0e0;
        }

        .info-badge {
            display: inline-block;
            background: #ff6b6b;
            color: white;
            padding: 8px 20px;
            border-radius: 25px;
            font-size: 0.95em;
            font-weight: 700;
            margin: 5px;
            text-transform: uppercase;
        }

        /* Where Poster Specific */
        .venue-showcase {
            margin: 40px 0;
        }

        .venue-card {
            background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
            border: 2px solid #e0e0e0;
        }

        .venue-image-container {
            width: 100%;
            height: 350px;
            border-radius: 15px;
            overflow: hidden;
            margin: 25px 0;
            box-shadow: 0 15px 40px rgba(0,0,0,0.15);
            border: 4px solid #ffa500;
        }

        .venue-image-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .venue-name {
            font-size: 2.2em;
            font-weight: 900;
            color: #1a1a1a;
            text-align: center;
            margin: 20px 0;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .parking-info {
            background: white;
            padding: 35px;
            border-radius: 15px;
            border: 3px solid #ff6b6b;
            margin-top: 30px;
            box-shadow: 0 5px 20px rgba(255, 107, 107, 0.2);
        }

        .parking-header {
            color: #ff6b6b;
            font-size: 1.6em;
            font-weight: 900;
            text-align: center;
            text-transform: uppercase;
            margin-bottom: 25px;
            letter-spacing: 1px;
        }

        .parking-content {
            display: grid;
            grid-template-columns: 140px 1fr;
            gap: 25px;
            align-items: center;
        }

        .qr-code-box {
            width: 140px;
            height: 140px;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
            border: 4px solid #ffa500;
        }

        .qr-code-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .map-box {
            height: 140px;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            border: 2px solid #e0e0e0;
        }

        .map-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        /* Tickets Poster Specific */
        .ticket-showcase {
            background: linear-gradient(135deg, #ffa500 0%, #ff8c00 100%);
            padding: 60px;
            border-radius: 20px;
            margin: 30px 0;
            box-shadow: 
                0 20px 60px rgba(255, 165, 0, 0.5),
                inset 0 -5px 20px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }

        .ticket-showcase::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                repeating-linear-gradient(
                    45deg,
                    transparent,
                    transparent 10px,
                    rgba(255,255,255,0.05) 10px,
                    rgba(255,255,255,0.05) 20px
                );
            pointer-events: none;
        }

        .ticket-display {
            position: relative;
            z-index: 1;
            text-align: center;
        }

        .ticket-price {
            font-size: 7em;
            font-weight: 900;
            color: white;
            font-style: italic;
            line-height: 1;
            text-shadow: 
                4px 4px 8px rgba(0,0,0,0.3),
                0 0 50px rgba(255, 255, 255, 0.3);
            display: flex;
            align-items: flex-start;
            justify-content: center;
            gap: 10px;
        }

        .currency {
            font-size: 0.5em;
            margin-top: 15px;
        }

        .ticket-label {
            font-size: 1.8em;
            color: white;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-top: 15px;
            opacity: 0.95;
        }

        /* ===== ORIGINAL STYLES ===== */
        .info-section {
            background: white;
            padding: 50px 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            margin: 40px 0;
            text-align: center;
        }

        .info-section h2 {
            color: #ffa500;
            font-size: 2.5em;
            margin-bottom: 20px;
            font-weight: 900;
            text-transform: uppercase;
        }

        .info-section p {
            font-size: 1.2em;
            color: #555;
            line-height: 1.8;
            max-width: 800px;
            margin: 20px auto;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .info-card {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .info-card h3 {
            color: #ff6b6b;
            font-size: 1.5em;
            margin-bottom: 15px;
        }

        .info-card p {
            font-size: 1.1em;
            color: #333;
        }

        /* CTA Section */
        .cta {
            background: linear-gradient(135deg, #ff6b6b 0%, #c92a2a 100%);
            color: white;
            text-align: center;
            padding: 80px 20px;
            border-radius: 15px;
            margin: 60px 0;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .cta h2 {
            font-size: 3em;
            margin-bottom: 20px;
            font-weight: 900;
        }

        .cta p {
            font-size: 1.4em;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background: white;
            color: #ff6b6b;
            padding: 18px 50px;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.3em;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 6px 20px rgba(0,0,0,0.2);
            margin: 10px;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.3);
        }

        .btn-secondary {
            background: #1a1a1a;
            color: white;
        }

        .social-links {
            margin-top: 40px;
            font-size: 1.1em;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: 600;
            transition: opacity 0.3s ease;
        }

        .social-links a:hover {
            opacity: 0.8;
        }

        /* Footer */
        footer {
            background: #0a0a0a;
            color: white;
            text-align: center;
            padding: 40px 20px;
            position: relative;
            z-index: 1;
            border-top: 2px solid rgba(139, 0, 0, 0.3);
        }

        footer p {
            margin: 10px 0;
        }

        .ministry-name {
            color: #ffa500;
            font-weight: 700;
            font-size: 1.3em;
        }

        /* Responsive Design */
        @media (max-width: 1200px) {
            .container {
                max-width: 95%;
            }

            .aesthetic-poster {
                max-width: 90%;
            }

            .poster-content {
                padding: 60px 40px;
            }

            .poster-title {
                font-size: 4em;
            }

            .featured-main {
                font-size: 4.5em;
            }

            .ticket-price {
                font-size: 6em;
            }
        }

        @media (max-width: 992px) {
            .poster-content {
                padding: 50px 35px;
            }

            .poster-title {
                font-size: 3.5em;
            }

            .poster-icon {
                font-size: 3.5em;
            }

            .featured-main {
                font-size: 4em;
            }

            .featured-sub {
                font-size: 1.5em;
            }

            .ticket-price {
                font-size: 5.5em;
            }

            .venue-image-container {
                height: 280px;
            }

            .venue-name {
                font-size: 1.8em;
            }

            .body-heading {
                font-size: 1.6em;
            }

            .body-text {
                font-size: 1.05em;
            }

            .highlight-box {
                font-size: 1em;
                padding: 16px 24px;
            }

            .info-section h2 {
                font-size: 2.2em;
            }

            .info-section p {
                font-size: 1.1em;
            }

            .cta h2 {
                font-size: 2.5em;
            }

            .cta p {
                font-size: 1.2em;
            }

            .btn {
                font-size: 1.2em;
                padding: 16px 45px;
            }
        }

        @media (max-width: 768px) {
            .hero-banner .desktop-banner {
                display: none;
            }

            .hero-banner .mobile-banner {
                display: block;
            }

            .hero-btn {
                font-size: 0.95em;
                padding: 15px 45px;
                letter-spacing: 1px;
            }

            .hero-overlay {
                bottom: 25px;
                width: 90%;
            }

            .aesthetic-poster {
                margin: 40px auto;
                border-radius: 20px;
            }

            .poster-content {
                padding: 45px 28px;
            }

            .poster-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 12px;
                margin-bottom: 30px;
                padding-bottom: 25px;
            }

            .poster-icon {
                font-size: 3em;
            }

            .poster-title {
                font-size: 2.8em;
                letter-spacing: -2px;
            }

            .poster-featured {
                padding: 40px 30px;
                margin: 25px 0;
            }

            .featured-main {
                font-size: 3.2em;
            }

            .featured-sub {
                font-size: 1.3em;
                letter-spacing: 2px;
            }

            .highlight-box {
                font-size: 0.95em;
                padding: 14px 22px;
                margin: 25px 0;
            }

            .body-heading {
                font-size: 1.4em;
            }

            .body-text {
                font-size: 1em;
                line-height: 1.7;
            }

            .venue-showcase {
                margin: 30px 0;
            }

            .venue-card {
                padding: 30px 25px;
            }

            .venue-image-container {
                height: 240px;
                margin: 20px 0;
                border-width: 3px;
            }

            .venue-name {
                font-size: 1.6em;
                margin: 15px 0;
            }

            .parking-info {
                padding: 28px 20px;
                margin-top: 25px;
            }

            .parking-header {
                font-size: 1.3em;
                margin-bottom: 20px;
            }

            .parking-content {
                grid-template-columns: 1fr;
                gap: 20px;
                justify-items: center;
            }

            .qr-code-box {
                width: 130px;
                height: 130px;
            }

            .map-box {
                width: 100%;
                height: 200px;
            }

            .ticket-showcase {
                padding: 45px 30px;
            }

            .ticket-price {
                font-size: 4.5em;
                gap: 8px;
            }

            .currency {
                font-size: 0.5em;
                margin-top: 12px;
            }

            .ticket-label {
                font-size: 1.5em;
                letter-spacing: 2px;
            }

            .info-badge {
                display: inline-block;
                margin: 6px 4px;
                padding: 7px 16px;
                font-size: 0.85em;
            }

            .info-section {
                padding: 40px 25px;
                margin: 30px 0;
            }

            .info-section h2 {
                font-size: 1.9em;
            }

            .info-section p {
                font-size: 1.05em;
            }

            .info-grid {
                grid-template-columns: 1fr;
                gap: 25px;
            }

            .info-card {
                padding: 25px;
            }

            .info-card h3 {
                font-size: 1.3em;
            }

            .info-card p {
                font-size: 1em;
            }

            .cta {
                padding: 60px 20px;
                margin: 40px 0;
            }

            .cta h2 {
                font-size: 1.9em;
            }

            .cta p {
                font-size: 1.1em;
            }

            .btn {
                display: block;
                width: 90%;
                max-width: 350px;
                margin: 10px auto;
                font-size: 1.1em;
                padding: 16px 40px;
            }

            .social-links {
                margin-top: 35px;
                font-size: 1em;
            }

            .social-links a {
                display: inline-block;
                margin: 8px 10px;
            }

            footer {
                padding: 35px 20px;
            }

            .ministry-name {
                font-size: 1.2em;
            }

            footer p {
                font-size: 0.95em;
            }
        }

        @media (max-width: 480px) {
            .hero-btn {
                font-size: 0.85em;
                padding: 14px 35px;
            }

            .poster-content {
                padding: 35px 22px;
            }

            .poster-icon {
                font-size: 2.5em;
            }

            .poster-title {
                font-size: 2.2em;
                letter-spacing: -1px;
            }

            .featured-main {
                font-size: 2.5em;
            }

            .featured-sub {
                font-size: 1.1em;
                letter-spacing: 1px;
            }

            .highlight-box {
                font-size: 0.9em;
                padding: 12px 20px;
            }

            .body-heading {
                font-size: 1.2em;
            }

            .body-text {
                font-size: 0.95em;
            }

            .venue-image-container {
                height: 200px;
            }

            .venue-name {
                font-size: 1.3em;
            }

            .parking-header {
                font-size: 1.1em;
            }

            .qr-code-box {
                width: 110px;
                height: 110px;
            }

            .map-box {
                height: 160px;
            }

            .ticket-price {
                font-size: 3.5em;
            }

            .ticket-label {
                font-size: 1.2em;
            }

            .info-section h2 {
                font-size: 1.6em;
            }

            .info-section p {
                font-size: 1em;
            }

            .info-card {
                padding: 20px;
            }

            .cta h2 {
                font-size: 1.6em;
            }

            .cta p {
                font-size: 1em;
            }

            .btn {
                font-size: 1em;
                padding: 14px 35px;
            }

            .social-links {
                font-size: 0.95em;
            }
        }

        @media (max-width: 360px) {
            .poster-content {
                padding: 30px 18px;
            }

            .poster-title {
                font-size: 1.9em;
            }

            .featured-main {
                font-size: 2.2em;
            }

            .ticket-price {
                font-size: 3em;
            }

            .venue-name {
                font-size: 1.1em;
            }

            .info-section h2 {
                font-size: 1.4em;
            }

            .cta h2 {
                font-size: 1.4em;
            }
        }

        /* Loading animation */
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .aesthetic-poster {
            animation: fadeIn 0.6s ease-out;
        }

        .aesthetic-poster:nth-child(1) { animation-delay: 0.1s; }
        .aesthetic-poster:nth-child(2) { animation-delay: 0.2s; }
        .aesthetic-poster:nth-child(3) { animation-delay: 0.3s; }
        .aesthetic-poster:nth-child(4) { animation-delay: 0.4s; }
    </style>
</head>
<body>
    <!-- Hero Banner - Full Screen -->
    <div class="hero-banner" id="hero">
        <!-- Desktop Banner -->
        <img src="images/poster1-desktop.png" alt="WN'25 - Jesus: Worthy Forever - Worship Night 2025" class="desktop-banner">
        
        <!-- Mobile Banner -->
        <img src="images/poster1.png" alt="WN'25 - Jesus: Worthy Forever - Worship Night 2025" class="mobile-banner">
        
        <!-- Button Overlay -->
        <div class="hero-overlay">
            <a href="#event-details" class="hero-btn">See Event Details</a>
        </div>
    </div>

    <!-- Event Details Section -->
    <div id="event-details">
        <div class="container">

            <!-- WHEN Poster -->
            <div class="aesthetic-poster">
                <div class="poster-content">
                    <div class="poster-header">
                        <div class="poster-icon">📅</div>
                        <div class="poster-title">WHEN?</div>
                    </div>

                    <div class="poster-featured">
                        <div class="featured-content">
                            <div class="featured-main">DECEMBER</div>
                            <div class="featured-main" style="font-size: 1.2em; margin-top: -20px;">30</div>
                            <div class="featured-sub">Tuesday, 2025</div>
                        </div>
                    </div>

                    <div class="poster-body">
                        <div class="body-text">
                            Worship Night will happen at <strong>December 30</strong>—the perfect moment to look back and celebrate all that God has done for us throughout the year.
                        </div>
                        <div class="body-text" style="margin-top: 20px;">
                            As the year comes to a close, we want to end it in His presence, thanking Him for His faithfulness and preparing our hearts for the year ahead.
                        </div>
                    </div>
                </div>
            </div>

            <!-- TIME Poster -->
            <div class="aesthetic-poster">
                <div class="poster-content">
                    <div class="poster-header">
                        <div class="poster-icon">🕔</div>
                        <div class="poster-title">TIME?</div>
                    </div>

                    <div class="poster-featured">
                        <div class="featured-content">
                            <div class="featured-main">5:00</div>
                            <div class="featured-sub">PM</div>
                        </div>
                    </div>

                    <div class="highlight-box">
                        Come Early!
                    </div>

                    <div class="poster-body">
                        <div class="body-section">
                            <div class="body-heading">
                                ☕ What's Available
                            </div>
                            <div class="body-text">
                                Our venue will have a <strong>coffee cart</strong> and <strong>photowall</strong> ready for you—perfect for hanging out, connecting with others, and soaking in the atmosphere before worship begins.
                            </div>
                        </div>

                        <div class="body-section">
                            <div class="body-heading">
                                📌 Important Note
                            </div>
                            <div class="body-text">
                                The coffee cart will only be taking orders <strong>BEFORE</strong> and <strong>AFTER</strong> the event. Arrive early, settle in, and enjoy the full experience!
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- WHERE Poster -->
            <div class="aesthetic-poster">
                <div class="poster-content">
                    <div class="poster-header">
                        <div class="poster-icon">📍</div>
                        <div class="poster-title">WHERE?</div>
                    </div>

                    <div class="venue-showcase">
                        <div class="venue-card">
                            <div class="venue-image-container">
                                <img src="images/venue.jpg" alt="Mexico Mini Convention Center">
                            </div>
                            
                            <div class="venue-name">
                                Mexico Mini<br>Convention Center
                            </div>

                            <div class="body-text" style="text-align: center; margin: 25px 0;">
                                By the provision of the Lord, Worship Night 2025 will take place at this blessed venue.
                            </div>

                            <div class="parking-info">
                                <div class="parking-header">
                                    🚗 Parking Located Here
                                </div>
                                <div class="parking-content">
                                    <div class="qr-code-box">
                                        <img src="images/qr-code.png" alt="QR Code for Parking">
                                    </div>
                                    <div class="map-box">
                                        <img src="images/map.png" alt="Parking Map">
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- TICKETS Poster -->
            <div class="aesthetic-poster">
                <div class="poster-content">
                    <div class="poster-header">
                        <div class="poster-icon">🎟️</div>
                        <div class="poster-title">TICKETS?</div>
                    </div>

                    <div class="poster-featured">
                        <div class="featured-content">
                            <div class="featured-main">₱100</div>
                            <div class="featured-sub">Only!</div>
                        </div>
                    </div>

                    <div class="poster-body">
                        <div class="body-section">
                            <div class="body-heading">
                                ✨ What's Included
                            </div>
                            <div class="body-text">
                                Your ticket includes <strong>food</strong> and supports the event. Get yours now and secure your spot for this blessed night of worship!
                            </div>
                        </div>

                        <div class="body-section">
                            <div class="body-heading">
                                🎫 How to Get Your Ticket
                            </div>
                            <div class="body-text">
                                Contact <strong>Regine Bondoc</strong> on Facebook to avail your ticket:<br>
                                <a href="https://www.facebook.com/regine.bondoc.98" target="_blank" style="color: #ff6b6b; font-weight: 700; text-decoration: none;">
                                    📘 facebook.com/regine.bondoc.98
                                </a>
                            </div>
                        </div>

                        <div style="text-align: center; margin-top: 30px;">
                            <span class="info-badge">💰 Affordable</span>
                            <span class="info-badge">🍽️ Food Included</span>
                            <span class="info-badge">🙏 Support Ministry</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Additional Info -->
            <div class="info-section">
                <h2>✨ What to Expect</h2>
                <p>Join us as we celebrate all that God has done throughout the year! As 2025 comes to a close, we want to end it in His presence—thanking Him for His faithfulness and preparing our hearts for the year ahead.</p>
                <p><strong>Coffee Cart & Photowall:</strong> Arrive early to enjoy our coffee cart and photowall. Perfect for hanging out, connecting with others, and soaking in the atmosphere before worship begins!</p>
                <p><strong>Note:</strong> The coffee cart will only be taking orders <strong>before</strong> and <strong>after</strong> the event.</p>
            </div>

            <!-- Call to Action -->
            <div class="cta">
                <h2>🙏 SEE YOU THERE! 🙏</h2>
                <p>Mark your calendar and join us for this blessed night of worship</p>
                
                <div class="social-links">
                    <p><strong>Follow us on social media:</strong></p>
                    <a href="https://facebook.com/CLMintrl" target="_blank" style="color: #4267B2; text-decoration: underline;">📘 facebook.com/CLMintrl</a>
                    <br>
                    <a href="https://instagram.com/clm.intrl" target="_blank" style="color: #E1306C; text-decoration: underline;">📸 instagram.com/clm.intrl</a>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <p class="ministry-name">CHRISTIAN LIFE MINISTRY</p>
        <p><strong>Worship Night 2025</strong></p>
        <p>"Jesus: Worthy Forever" - Revelation 5:12</p>
        <p style="margin-top: 20px;">December 30, 2025 | 5:00 PM | Mexico Mini Convention Center</p>
        <p style="margin-top: 20px;">&copy; 2024-2025 Christian Life Ministry International. All rights reserved.</p>
        <p><strong>God bless you! 🙏</strong></p>
    </footer>
</body>
</html>

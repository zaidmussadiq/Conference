<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IIMC 2026 — Pakistan's First Cultural Internal Medicine Conference | Alhamrah, Lahore</title>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;0,700;1,400;1,600&family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@400;500&family=Noto+Nastaliq+Urdu:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --mughal-green: #1A5C3A;
            --mughal-green-deep: #0F3D24;
            --gold-lahore: #C9A84C;
            --gold-bright: #E8C96A;
            --maroon-royal: #7A1C2E;
            --maroon-deep: #5C1522;
            --indigo-tile: #2C3E7B;
            --terracotta: #C67B4B;
            --white: #FFFFFF;
            --cream: #FDF8F0;
            --warm-cream: #FBF3E3;
            --slate: #64748B;
            --dark-slate: #334155;
            --navy: #0D1B3E;
            --teal: #0E7C86;
            --teal-light: #14A4B0;
            --off-white: #F4F7FA;
            --light-gray: #E8EEF4;
            --truck-art-red: #D42B3F;
            --truck-art-blue: #1B5FA8;
            --truck-art-yellow: #F5A623;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'DM Sans', sans-serif;
            background: var(--cream);
            color: var(--dark-slate);
            min-height: 100vh;
            background-image:
                radial-gradient(ellipse at 15% 5%, rgba(26, 92, 58, 0.03) 0%, transparent 55%),
                radial-gradient(ellipse at 85% 92%, rgba(122, 28, 46, 0.03) 0%, transparent 55%),
                radial-gradient(ellipse at 50% 50%, rgba(201, 168, 76, 0.02) 0%, transparent 70%);
        }

        /* Decorative geometric pattern overlay — inspired by Mughal jaali */
        body::before {
            content: '';
            position: fixed;
            inset: 0;
            pointer-events: none;
            z-index: 0;
            opacity: 0.015;
            background-image: repeating-linear-gradient(45deg, var(--mughal-green) 0px, var(--mughal-green) 1px, transparent 1px, transparent 28px),
                repeating-linear-gradient(-45deg, var(--mughal-green) 0px, var(--mughal-green) 1px, transparent 1px, transparent 28px);
            mask-image: radial-gradient(ellipse at 50% 30%, black 30%, transparent 70%);
            -webkit-mask-image: radial-gradient(ellipse at 50% 30%, black 30%, transparent 70%);
        }

        /* ── TOP CULTURAL RIBBON ── */
        .cultural-ribbon {
            background: var(--mughal-green-deep);
            color: var(--gold-bright);
            text-align: center;
            padding: 8px 20px;
            font-family: 'DM Mono', monospace;
            font-size: 9.5px;
            letter-spacing: 3px;
            text-transform: uppercase;
            position: relative;
            z-index: 1;
            border-bottom: 2px solid var(--gold-lahore);
            overflow: hidden;
        }
        .cultural-ribbon::before {
            content: '';
            position: absolute;
            inset: 0;
            background: repeating-linear-gradient(90deg, transparent, transparent 40px, rgba(201, 168, 76, 0.06) 40px, rgba(201, 168, 76, 0.06) 42px);
        }
        .cultural-ribbon span {
            position: relative;
            z-index: 1;
        }
        .cultural-ribbon .truck-dot {
            display: inline-block;
            width: 6px;
            height: 6px;
            border-radius: 50%;
            margin: 0 6px;
            vertical-align: middle;
            animation: truckPulse 2s ease-in-out infinite;
        }
        .cultural-ribbon .truck-dot:nth-child(1) {
            background: var(--truck-art-red);
            animation-delay: 0s;
        }
        .cultural-ribbon .truck-dot:nth-child(2) {
            background: var(--truck-art-yellow);
            animation-delay: 0.4s;
        }
        .cultural-ribbon .truck-dot:nth-child(3) {
            background: var(--truck-art-blue);
            animation-delay: 0.8s;
        }
        .cultural-ribbon .truck-dot:nth-child(4) {
            background: var(--truck-art-red);
            animation-delay: 1.2s;
        }
        .cultural-ribbon .truck-dot:nth-child(5) {
            background: var(--gold-bright);
            animation-delay: 1.6s;
        }

        @keyframes truckPulse {
            0%,
            100% {
                transform: scale(1);
                opacity: 0.7;
            }
            50% {
                transform: scale(1.8);
                opacity: 1;
            }
        }

        /* ── VENUE BADGE ── */
        .venue-strip {
            background: var(--maroon-royal);
            color: var(--white);
            text-align: center;
            padding: 6px 20px;
            font-size: 10px;
            letter-spacing: 2.5px;
            text-transform: uppercase;
            font-weight: 500;
            border-bottom: 1px solid rgba(255, 255, 255, 0.15);
            position: relative;
            z-index: 1;
        }
        .venue-strip .alamhra-icon {
            display: inline-block;
            font-size: 14px;
            margin: 0 8px;
            vertical-align: middle;
        }

        /* ── HERO ── */
        .hero {
            background: linear-gradient(170deg, #0F1F14 0%, #1A2F1F 25%, #162818 50%, #0F1F14 100%);
            position: relative;
            overflow: hidden;
            padding: 0;
            z-index: 1;
        }
        .hero::before {
            content: '';
            position: absolute;
            inset: 0;
            background:
                radial-gradient(ellipse at 70% 40%, rgba(201, 168, 76, 0.12) 0%, transparent 55%),
                radial-gradient(ellipse at 25% 75%, rgba(26, 92, 58, 0.25) 0%, transparent 50%),
                radial-gradient(ellipse at 80% 85%, rgba(122, 28, 46, 0.18) 0%, transparent 45%);
        }
        /* Mughal arch silhouette */
        .hero::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 90px;
            background:
                radial-gradient(ellipse at 50% 100%, transparent 60%, rgba(201, 168, 76, 0.08) 60%, rgba(201, 168, 76, 0.08) 62%, transparent 62%),
                radial-gradient(ellipse at 20% 100%, transparent 55%, rgba(201, 168, 76, 0.05) 55%, rgba(201, 168, 76, 0.05) 57%, transparent 57%),
                radial-gradient(ellipse at 80% 100%, transparent 55%, rgba(201, 168, 76, 0.05) 55%, rgba(201, 168, 76, 0.05) 57%, transparent 57%);
            pointer-events: none;
            z-index: 0;
        }
        .hero-accent-left {
            position: absolute;
            left: 0;
            top: 0;
            bottom: 0;
            width: 8px;
            background: linear-gradient(180deg, var(--gold-lahore) 0%, var(--maroon-royal) 50%, var(--mughal-green) 100%);
            z-index: 2;
        }
        .hero-accent-right {
            position: absolute;
            right: 0;
            top: 0;
            width: 34%;
            height: 100%;
            background: rgba(255, 255, 255, 0.015);
            border-left: 1px solid rgba(201, 168, 76, 0.2);
            z-index: 0;
        }
        /* Truck art inspired decorative dots */
        .hero-dots {
            position: absolute;
            right: 6%;
            top: 8%;
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            gap: 16px;
            z-index: 1;
        }
        .hero-dots span {
            width: 7px;
            height: 7px;
            border-radius: 50%;
            opacity: 0.3;
            animation: pulse 3s ease-in-out infinite;
        }
        .hero-dots span:nth-child(1) {
            background: var(--truck-art-red);
        }
        .hero-dots span:nth-child(2) {
            background: var(--gold-bright);
        }
        .hero-dots span:nth-child(3) {
            background: var(--truck-art-blue);
        }
        .hero-dots span:nth-child(4) {
            background: var(--truck-art-yellow);
            animation-delay: 0.5s;
        }
        .hero-dots span:nth-child(5) {
            background: var(--truck-art-red);
            animation-delay: 1s;
        }
        .hero-dots span:nth-child(6) {
            background: var(--gold-bright);
            animation-delay: 1.5s;
        }
        .hero-dots span:nth-child(7) {
            background: var(--truck-art-blue);
            animation-delay: 0.3s;
        }
        .hero-dots span:nth-child(8) {
            background: var(--truck-art-yellow);
            animation-delay: 0.8s;
        }
        .hero-dots span:nth-child(9) {
            background: var(--truck-art-red);
            animation-delay: 1.3s;
        }
        .hero-dots span:nth-child(10) {
            background: var(--gold-bright);
            animation-delay: 0.6s;
        }
        .hero-dots span:nth-child(11) {
            background: var(--truck-art-blue);
            animation-delay: 1.1s;
        }
        .hero-dots span:nth-child(12) {
            background: var(--truck-art-yellow);
            animation-delay: 1.6s;
        }

        @keyframes pulse {
            0%,
            100% {
                transform: scale(1);
                opacity: 0.3;
            }
            50% {
                transform: scale(1.5);
                opacity: 0.55;
            }
        }
        .hero-inner {
            position: relative;
            display: grid;
            grid-template-columns: 1fr 320px;
            min-height: 440px;
            max-width: 1240px;
            margin: 0 auto;
            padding: 56px 56px 56px 68px;
            gap: 50px;
            z-index: 1;
        }
        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: var(--gold-lahore);
            color: var(--mughal-green-deep);
            font-family: 'DM Mono', monospace;
            font-size: 10.5px;
            font-weight: 600;
            letter-spacing: 3px;
            text-transform: uppercase;
            padding: 7px 18px;
            margin-bottom: 24px;
            position: relative;
        }
        .hero-badge::after {
            content: '';
            position: absolute;
            right: -6px;
            top: 50%;
            transform: translateY(-50%);
            width: 12px;
            height: 12px;
            background: var(--maroon-royal);
            border-radius: 50%;
        }
        .hero h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: clamp(34px, 5vw, 54px);
            font-weight: 700;
            color: var(--white);
            line-height: 1.06;
            margin-bottom: 8px;
            animation: fadeUp 0.7s ease both;
            letter-spacing: -0.3px;
        }
        .hero h1 .lahore-accent {
            color: var(--gold-bright);
            font-style: italic;
        }
        @keyframes fadeUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .hero-divider {
            width: 240px;
            height: 2px;
            background: linear-gradient(90deg, var(--gold-lahore) 0%, transparent 100%);
            margin: 20px 0 22px;
            animation: fadeUp 0.8s 0.1s ease both;
        }
        .hero-subtitle {
            font-family: 'Cormorant Garamond', serif;
            font-size: 18px;
            font-style: italic;
            color: rgba(255, 255, 255, 0.8);
            line-height: 1.5;
            max-width: 540px;
            animation: fadeUp 0.8s 0.2s ease both;
        }
        .hero-subtitle strong {
            color: var(--gold-bright);
            font-weight: 600;
        }
        .hero-tags {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 28px;
            animation: fadeUp 0.8s 0.3s ease both;
        }
        .hero-tag {
            padding: 7px 18px;
            font-size: 10.5px;
            font-weight: 600;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            border-radius: 1px;
        }
        .hero-tag.teal {
            background: var(--mughal-green);
            color: var(--white);
        }
        .hero-tag.outline {
            border: 1px solid rgba(255, 255, 255, 0.25);
            color: rgba(255, 255, 255, 0.7);
        }
        .hero-right {
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 16px;
            animation: fadeUp 0.9s 0.2s ease both;
        }
        .hero-org-card {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid rgba(201, 168, 76, 0.3);
            padding: 22px 18px;
            text-align: center;
        }
        .hero-org-icon {
            font-size: 38px;
            margin-bottom: 8px;
        }
        .hero-org-name {
            font-family: 'Cormorant Garamond', serif;
            font-size: 15px;
            font-weight: 600;
            color: var(--gold-lahore);
            letter-spacing: 1px;
            margin-bottom: 3px;
        }
        .hero-org-sub {
            font-size: 10px;
            color: rgba(255, 255, 255, 0.4);
            letter-spacing: 0.5px;
        }
        .hero-days {
            background: rgba(26, 92, 58, 0.25);
            border: 1px solid rgba(201, 168, 76, 0.25);
            padding: 16px 20px;
        }
        .hero-days-row {
            display: flex;
            align-items: flex-start;
            gap: 10px;
            padding: 7px 0;
        }
        .hero-days-row+.hero-days-row {
            border-top: 1px solid rgba(255, 255, 255, 0.06);
        }
        .day-num {
            background: var(--gold-lahore);
            color: var(--mughal-green-deep);
            font-family: 'DM Mono', monospace;
            font-size: 9px;
            font-weight: 600;
            padding: 3px 9px;
            flex-shrink: 0;
            margin-top: 2px;
            letter-spacing: 1px;
        }
        .day-label {
            font-size: 11px;
            color: rgba(255, 255, 255, 0.65);
            line-height: 1.4;
        }

        /* ── SECTION WRAPPER ── */
        .section {
            max-width: 1240px;
            margin: 0 auto;
            padding: 56px 56px;
            position: relative;
            z-index: 1;
        }
        .section-header {
            display: flex;
            align-items: center;
            gap: 14px;
            margin-bottom: 32px;
        }
        .section-tag {
            font-family: 'DM Mono', monospace;
            font-size: 9.5px;
            font-weight: 500;
            letter-spacing: 3px;
            text-transform: uppercase;
            color: var(--mughal-green);
        }
        .section-line {
            flex: 1;
            height: 1px;
            background: linear-gradient(90deg, var(--light-gray) 0%, transparent 100%);
        }
        .section-title {
            font-family: 'Cormorant Garamond', serif;
            font-size: 32px;
            font-weight: 700;
            color: var(--mughal-green-deep);
            margin-bottom: 6px;
        }
        .section-sub {
            font-size: 13.5px;
            color: var(--slate);
            line-height: 1.6;
        }

        /* ── CULTURAL HIGHLIGHT BOX ── */
        .cultural-highlight {
            background: linear-gradient(135deg, var(--maroon-royal) 0%, var(--maroon-deep) 100%);
            color: var(--white);
            padding: 28px 32px;
            margin-bottom: 28px;
            display: flex;
            align-items: center;
            gap: 20px;
            border-left: 5px solid var(--gold-lahore);
            position: relative;
            overflow: hidden;
        }
        .cultural-highlight::before {
            content: '';
            position: absolute;
            right: -30px;
            top: -30px;
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 3px solid rgba(201, 168, 76, 0.2);
            pointer-events: none;
        }
        .cultural-highlight-icon {
            font-size: 44px;
            flex-shrink: 0;
        }
        .cultural-highlight h3 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 22px;
            font-weight: 700;
            margin-bottom: 4px;
            color: var(--gold-bright);
        }
        .cultural-highlight p {
            font-size: 13px;
            color: rgba(255, 255, 255, 0.8);
            line-height: 1.5;
        }

        /* ── OVERVIEW CARDS ── */
        .overview-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 18px;
        }
        .overview-card {
            background: white;
            padding: 26px 20px;
            border-top: 3px solid transparent;
            box-shadow: 0 2px 14px rgba(15, 31, 20, 0.06);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            position: relative;
        }
        .overview-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 8px 26px rgba(15, 31, 20, 0.11);
        }
        .overview-card:nth-child(1) {
            border-color: var(--mughal-green);
        }
        .overview-card:nth-child(2) {
            border-color: var(--gold-lahore);
        }
        .overview-card:nth-child(3) {
            border-color: var(--indigo-tile);
        }
        .overview-card:nth-child(4) {
            border-color: var(--maroon-royal);
        }
        .ov-icon {
            font-size: 28px;
            margin-bottom: 12px;
        }
        .ov-title {
            font-family: 'Cormorant Garamond', serif;
            font-size: 17px;
            font-weight: 700;
            color: var(--mughal-green-deep);
            margin-bottom: 8px;
        }
        .ov-desc {
            font-size: 12.5px;
            color: var(--slate);
            line-height: 1.55;
        }

        /* ── DAY DIVIDER ── */
        .day-divider {
            background: linear-gradient(180deg, #0F1F14 0%, #162818 100%);
            color: white;
            position: relative;
            overflow: hidden;
        }
        .day-divider::after {
            content: '';
            position: absolute;
            inset: 0;
            background: radial-gradient(ellipse at 78% 50%, rgba(201, 168, 76, 0.1) 0%, transparent 60%),
                radial-gradient(ellipse at 20% 50%, rgba(26, 92, 58, 0.2) 0%, transparent 55%);
        }
        .day-divider-inner {
            position: relative;
            z-index: 1;
            max-width: 1240px;
            margin: 0 auto;
            padding: 44px 56px;
            display: flex;
            align-items: center;
            gap: 36px;
        }
        .day-number-badge {
            flex-shrink: 0;
            width: 95px;
            height: 95px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border: 2px solid var(--gold-lahore);
            position: relative;
        }
        .day-number-badge::after {
            content: '';
            position: absolute;
            inset: -6px;
            border: 1px solid rgba(201, 168, 76, 0.3);
            pointer-events: none;
        }
        .day-divider.day2 .day-number-badge {
            border-color: var(--mughal-green);
        }
        .day-number-badge .day-word {
            font-family: 'DM Mono', monospace;
            font-size: 10px;
            letter-spacing: 3px;
            color: var(--gold-lahore);
            margin-bottom: 1px;
        }
        .day-divider.day2 .day-number-badge .day-word {
            color: #5CAB7D;
        }
        .day-number-badge .day-n {
            font-family: 'Cormorant Garamond', serif;
            font-size: 50px;
            font-weight: 700;
            color: white;
            line-height: 1;
        }
        .day-divider-content h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 32px;
            font-weight: 700;
            color: white;
            margin-bottom: 8px;
        }
        .day-divider-content p {
            font-size: 12.5px;
            color: rgba(255, 255, 255, 0.5);
            line-height: 1.6;
        }
        .day-accent {
            width: 3px;
            align-self: stretch;
            background: var(--gold-lahore);
            flex-shrink: 0;
            margin: 0 8px;
        }
        .day-divider.day2 .day-accent {
            background: var(--mughal-green);
        }

        /* ── SCHEDULE BLOCKS ── */
        .schedule-block {
            background: white;
            box-shadow: 0 2px 14px rgba(15, 31, 20, 0.06);
            margin-bottom: 18px;
            overflow: hidden;
            transition: box-shadow 0.2s ease;
            border-radius: 1px;
        }
        .schedule-block:hover {
            box-shadow: 0 6px 22px rgba(15, 31, 20, 0.1);
        }
        .sb-header {
            display: flex;
            align-items: stretch;
            border-left: 5px solid var(--mughal-green);
        }
        .sb-header.gold-accent {
            border-left-color: var(--gold-lahore);
        }
        .sb-header.slate-accent {
            border-left-color: var(--slate);
        }
        .sb-header.purple-accent {
            border-left-color: var(--indigo-tile);
        }
        .sb-header.maroon-accent {
            border-left-color: var(--maroon-royal);
        }
        .sb-time {
            background: var(--mughal-green);
            color: white;
            font-family: 'DM Mono', monospace;
            font-size: 10.5px;
            font-weight: 500;
            padding: 13px 16px;
            display: flex;
            align-items: center;
            min-width: 125px;
            justify-content: center;
            text-align: center;
            flex-shrink: 0;
            letter-spacing: 0.5px;
        }
        .sb-header.gold-accent .sb-time {
            background: var(--gold-lahore);
            color: var(--mughal-green-deep);
        }
        .sb-header.slate-accent .sb-time {
            background: var(--slate);
        }
        .sb-header.purple-accent .sb-time {
            background: var(--indigo-tile);
        }
        .sb-header.maroon-accent .sb-time {
            background: var(--maroon-royal);
        }
        .sb-title-wrap {
            padding: 13px 22px;
            display: flex;
            align-items: center;
            gap: 10px;
            flex: 1;
        }
        .sb-icon {
            font-size: 19px;
            flex-shrink: 0;
        }
        .sb-title {
            font-family: 'Cormorant Garamond', serif;
            font-size: 18px;
            font-weight: 700;
            color: var(--mughal-green-deep);
        }
        .sb-subtitle {
            font-size: 11.5px;
            font-style: italic;
            color: var(--mughal-green);
            margin-left: auto;
            flex-shrink: 0;
            padding-right: 6px;
        }
        .sb-body {
            padding: 18px 26px 22px;
        }
        .bullet-list {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 6px;
        }
        .bullet-list li {
            font-size: 13px;
            color: var(--dark-slate);
            padding-left: 18px;
            position: relative;
            line-height: 1.5;
        }
        .bullet-list li::before {
            content: '✦';
            position: absolute;
            left: 0;
            color: var(--gold-lahore);
            font-size: 7px;
            top: 5px;
        }

        /* ── TRACKS GRID ── */
        .tracks-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 14px;
            margin-top: 4px;
        }
        .track-card {
            background: var(--warm-cream);
            overflow: hidden;
            border: 1px solid rgba(201, 168, 76, 0.15);
        }
        .track-card-top {
            display: flex;
            align-items: center;
            gap: 0;
        }
        .track-label {
            padding: 7px 13px;
            font-family: 'DM Mono', monospace;
            font-size: 9.5px;
            font-weight: 500;
            color: white;
            letter-spacing: 1px;
        }
        .track-name {
            padding: 7px 13px;
            font-size: 11.5px;
            font-weight: 600;
            color: var(--mughal-green-deep);
        }
        .track-desc {
            padding: 10px 13px 12px;
            font-size: 11.5px;
            color: var(--slate);
            line-height: 1.5;
            border-top: 1px solid rgba(201, 168, 76, 0.1);
        }

        /* ── WORKSHOPS ── */
        .workshops-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 14px;
            margin-top: 4px;
        }
        .ws-card {
            background: var(--mughal-green-deep);
            padding: 22px 16px 18px;
            text-align: center;
            position: relative;
            overflow: hidden;
            transition: transform 0.2s ease;
            border: 1px solid rgba(201, 168, 76, 0.2);
        }
        .ws-card:hover {
            transform: translateY(-3px);
        }
        .ws-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
        }
        .ws-card.t1::before {
            background: var(--gold-lahore);
        }
        .ws-card.t2::before {
            background: var(--mughal-green);
        }
        .ws-icon {
            font-size: 26px;
            margin-bottom: 12px;
            display: block;
        }
        .ws-label {
            font-family: 'DM Mono', monospace;
            font-size: 8.5px;
            letter-spacing: 2px;
            text-transform: uppercase;
            margin-bottom: 6px;
        }
        .ws-card.t1 .ws-label {
            color: var(--gold-bright);
        }
        .ws-card.t2 .ws-label {
            color: #5CAB7D;
        }
        .ws-name {
            font-size: 12px;
            font-weight: 500;
            color: rgba(255, 255, 255, 0.82);
            line-height: 1.4;
        }

        /* ── CULTURAL EXPERIENCE CARD ── */
        .cultural-experience-card {
            background: linear-gradient(135deg, #FDF8F0 0%, #FBF3E3 100%);
            border: 2px solid var(--gold-lahore);
            padding: 22px 26px;
            margin-top: 16px;
            display: flex;
            align-items: center;
            gap: 16px;
            position: relative;
            overflow: hidden;
        }
        .cultural-experience-card::before {
            content: '';
            position: absolute;
            right: -20px;
            bottom: -20px;
            width: 80px;
            height: 80px;
            border-radius: 50%;
            border: 2px solid rgba(201, 168, 76, 0.25);
            pointer-events: none;
        }
        .cultural-experience-icon {
            font-size: 32px;
            flex-shrink: 0;
        }
        .cultural-experience-text {
            font-size: 13px;
            color: var(--mughal-green-deep);
            line-height: 1.5;
        }
        .cultural-experience-text strong {
            color: var(--maroon-royal);
        }

        /* ── GALA BANNER ── */
        .gala-banner {
            background: linear-gradient(135deg, var(--gold-lahore) 0%, var(--gold-bright) 100%);
            padding: 16px 26px;
            display: flex;
            align-items: center;
            gap: 14px;
            margin-top: 18px;
            color: var(--mughal-green-deep);
        }
        .gala-banner-icon {
            font-size: 22px;
        }
        .gala-banner-text {
            font-size: 13.5px;
            font-weight: 600;
        }
        .gala-banner-text span {
            font-family: 'DM Mono', monospace;
            font-size: 10px;
            font-weight: 500;
            margin-right: 6px;
            opacity: 0.7;
        }

        /* ── PLENARY NOTE ── */
        .plenary-note {
            background: rgba(26, 92, 58, 0.06);
            border-left: 3px solid var(--mughal-green);
            padding: 11px 16px;
            font-size: 12px;
            font-style: italic;
            color: var(--mughal-green);
            margin-top: 14px;
        }

        /* ── AT A GLANCE ── */
        .glance-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 24px;
        }
        .glance-col-header {
            padding: 13px 18px;
            font-family: 'DM Mono', monospace;
            font-size: 9.5px;
            letter-spacing: 2.5px;
            text-transform: uppercase;
            font-weight: 500;
            color: white;
            margin-bottom: 10px;
        }
        .glance-col-header.d1 {
            background: var(--mughal-green);
        }
        .glance-col-header.d2 {
            background: var(--gold-lahore);
            color: var(--mughal-green-deep);
        }
        .glance-row {
            background: white;
            display: flex;
            align-items: flex-start;
            gap: 0;
            margin-bottom: 7px;
            overflow: hidden;
            box-shadow: 0 1px 5px rgba(15, 31, 20, 0.05);
        }
        .glance-bar {
            width: 4px;
            align-self: stretch;
            flex-shrink: 0;
        }
        .glance-row-inner {
            padding: 12px 15px;
            flex: 1;
        }
        .glance-time {
            font-family: 'DM Mono', monospace;
            font-size: 9.5px;
            font-weight: 500;
            margin-bottom: 2px;
        }
        .glance-label {
            font-size: 12.5px;
            color: var(--dark-slate);
        }

        /* ── AWARDS ── */
        .awards-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin-top: 4px;
        }
        .award-item {
            background: var(--warm-cream);
            border: 1px solid rgba(201, 168, 76, 0.2);
            padding: 13px 16px;
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 13px;
            font-weight: 500;
            color: var(--dark-slate);
        }
        .award-icon {
            font-size: 17px;
        }

        /* ── CLOSING ── */
        .closing {
            background: linear-gradient(180deg, #0F1F14 0%, #0A1810 100%);
            padding: 70px 56px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        .closing::before {
            content: '';
            position: absolute;
            inset: 0;
            background: radial-gradient(ellipse at 50% 55%, rgba(201, 168, 76, 0.12) 0%, transparent 60%),
                radial-gradient(ellipse at 40% 70%, rgba(26, 92, 58, 0.18) 0%, transparent 55%);
        }
        .closing-inner {
            position: relative;
            z-index: 1;
            max-width: 680px;
            margin: 0 auto;
        }
        .closing-icon {
            font-size: 50px;
            margin-bottom: 20px;
            display: block;
        }
        .closing h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 36px;
            font-weight: 700;
            color: var(--gold-lahore);
            letter-spacing: 1px;
            margin-bottom: 14px;
        }
        .closing-divider {
            width: 100px;
            height: 2px;
            background: var(--mughal-green);
            margin: 18px auto;
        }
        .closing-sub {
            font-family: 'Cormorant Garamond', serif;
            font-size: 18px;
            font-style: italic;
            color: rgba(255, 255, 255, 0.7);
            line-height: 1.6;
            margin-bottom: 22px;
        }
        .closing-org {
            font-family: 'DM Mono', monospace;
            font-size: 10.5px;
            letter-spacing: 2px;
            color: rgba(255, 255, 255, 0.3);
            text-transform: uppercase;
        }
        .closing-welcome {
            font-size: 13.5px;
            color: #5CAB7D;
            font-style: italic;
            margin-top: 18px;
        }

        /* ── FOOTER ── */
        footer {
            background: #081008;
            padding: 16px 56px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-top: 1px solid rgba(201, 168, 76, 0.2);
        }
        .footer-left {
            font-family: 'DM Mono', monospace;
            font-size: 9.5px;
            letter-spacing: 2px;
            color: var(--gold-lahore);
            text-transform: uppercase;
        }
        .footer-right {
            font-size: 10.5px;
            color: rgba(255, 255, 255, 0.25);
        }

        /* ── ADVISOR SECTION ── */
        .advisor-strip {
            background: white;
            border-top: 3px solid var(--gold-lahore);
            border-bottom: 1px solid rgba(201, 168, 76, 0.3);
            padding: 18px 56px;
            text-align: center;
            font-size: 13px;
            color: var(--dark-slate);
            letter-spacing: 0.5px;
        }
        .advisor-strip strong {
            color: var(--maroon-royal);
            font-family: 'Cormorant Garamond', serif;
            font-size: 16px;
            letter-spacing: 1px;
        }

        /* ── RESPONSIVE ── */
        @media (max-width: 900px) {
            .hero-inner {
                grid-template-columns: 1fr;
                padding: 44px 28px;
            }
            .hero-right {
                display: none;
            }
            .section {
                padding: 44px 28px;
            }
            .overview-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .tracks-grid {
                grid-template-columns: 1fr;
            }
            .workshops-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .glance-grid {
                grid-template-columns: 1fr;
            }
            .awards-grid {
                grid-template-columns: 1fr;
            }
            .day-divider-inner {
                padding: 32px 28px;
                flex-direction: column;
                text-align: center;
            }
            .day-accent {
                display: none;
            }
            footer {
                flex-direction: column;
                gap: 6px;
                text-align: center;
                padding: 16px 28px;
            }
            .cultural-highlight {
                flex-direction: column;
                text-align: center;
            }
            .advisor-strip {
                padding: 14px 28px;
            }
        }
        @media (max-width: 600px) {
            .overview-grid {
                grid-template-columns: 1fr;
            }
            .workshops-grid {
                grid-template-columns: 1fr;
            }
            .hero-dots {
                display: none;
            }
        }
    </style>
</head>
<body>

    <!-- ═══════════════ TOP CULTURAL RIBBON ═══════════════ -->
    <div class="cultural-ribbon">
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        &nbsp; Pakistan's First Culturally-Infused Medical Conference &nbsp;·&nbsp; Where Heritage Meets Innovation &nbsp;
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
        <span class="truck-dot"></span>
    </div>

    <!-- ═══════════════ VENUE STRIP ═══════════════ -->
    <div class="venue-strip">
        <span class="alamhra-icon">🏛️</span> Venue: Alhamrah Arts Council, The Mall, Lahore &nbsp;—&nbsp; The Cultural Heart of Pakistan
        <span class="alamhra-icon">🏛️</span>
    </div>

    <!-- ═══════════════ ADVISOR STRIP ═══════════════ -->
    <div class="advisor-strip">
        Proposed for the kind consideration of &nbsp;<strong>Dr. Mehmood Nasir Malik</strong>&nbsp; — Head of Department of Medicine
    </div>

    <!-- ═══════════════ HERO ═══════════════ -->
    <section class="hero">
        <div class="hero-accent-left"></div>
        <div class="hero-accent-right"></div>
        <div class="hero-dots">
            <span></span><span></span><span></span><span></span><span></span><span></span>
            <span></span><span></span><span></span><span></span><span></span><span></span>
        </div>
        <div class="hero-inner">
            <div class="hero-left">
                <div class="hero-badge">IIMC 2026 · Lahore</div>
                <h1>International<br>Internal Medicine<br>Conference</h1>
                <p class="hero-subtitle" style="margin-top:4px; font-size:15px; color:var(--gold-bright); font-style:normal; letter-spacing:1px; font-weight:600;">
                    <span class="lahore-accent">— The Lahore Edition —</span>
                </p>
                <div class="hero-divider"></div>
                <p class="hero-subtitle">
                    Redefining Evidence-Based Internal Medicine in the Era of Artificial Intelligence
                    <br><strong>— Infused with Pakistan's Rich Cultural Heritage —</strong>
                </p>
                <div class="hero-tags">
                    <span class="hero-tag teal">Two-Day Cultural Experience</span>
                    <span class="hero-tag outline">Clinical Intelligence</span>
                    <span class="hero-tag outline">AI in Medicine</span>
                    <span class="hero-tag outline">Heritage & Innovation</span>
                </div>
            </div>
            <div class="hero-right">
                <div class="hero-org-card">
                    <div class="hero-org-icon">🏥</div>
                    <div class="hero-org-name">SCORE IFMSA Pakistan</div>
                    <div class="hero-org-sub">Organizing Committee · IIMC 2026</div>
                </div>
                <div class="hero-days">
                    <div class="hero-days-row">
                        <span class="day-num">DAY 1</span>
                        <span class="day-label">Clinical Intelligence &amp; Cultural Engagement</span>
                    </div>
                    <div class="hero-days-row">
                        <span class="day-num">DAY 2</span>
                        <span class="day-label">Research, Innovation &amp; Lahore's Heritage</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ═══════════════ OVERVIEW ═══════════════ -->
    <div style="background: var(--cream);">
        <div class="section">
            <div class="section-header">
                <span class="section-tag">Conference Overview</span>
                <div class="section-line"></div>
            </div>
            <p class="section-title">What to Expect</p>
            <p class="section-sub" style="margin-bottom: 24px;">A first-of-its-kind conference in Pakistan — merging world-class internal medicine with the vibrant cultural tapestry of Lahore and Pakistan</p>

            <!-- Cultural Highlight Box -->
            <div class="cultural-highlight">
                <span class="cultural-highlight-icon">🏛️</span>
                <div>
                    <h3>Pakistan's First Cultural-Aspect Medical Conference</h3>
                    <p>Hosted at the iconic <strong>Alhamrah Arts Council, Lahore</strong> — a venue steeped in the artistic and architectural legacy of the Mughal era. This conference goes beyond academia, offering delegates an immersive experience of Pakistani hospitality, Lahori cuisine, Sufi music, truck art displays, calligraphy exhibitions, and the warmth of our centuries-old cultural traditions — all woven seamlessly into a cutting-edge medical programme.</p>
                </div>
            </div>

            <div class="overview-grid">
                <div class="overview-card">
                    <div class="ov-icon">🩺</div>
                    <div class="ov-title">Academic Tracks</div>
                    <div class="ov-desc">Oral &amp; poster presentations, clinical quizzes, rapid-fire challenges, diagnostic arenas, and research innovation pitches across both days</div>
                </div>
                <div class="overview-card">
                    <div class="ov-icon">💻</div>
                    <div class="ov-title">Hands-On Workshops</div>
                    <div class="ov-desc">8 parallel workshops across 2 days — pre-registration required for focused, hands-on skill-building in AI, clinical trials, radiology & more</div>
                </div>
                <div class="overview-card">
                    <div class="ov-icon">🎨</div>
                    <div class="ov-title">Cultural Immersion</div>
                    <div class="ov-desc">Traditional Pakistani welcome, live Sufi/Qawwali performances, truck art gallery, calligraphy demonstrations, and Lahori culinary experiences</div>
                </div>
                <div class="overview-card">
                    <div class="ov-icon">🏆</div>
                    <div class="ov-title">Competitions &amp; Awards</div>
                    <div class="ov-desc">Best oral, poster, research pitch and competition winners awarded with traditional Pakistani craftsmanship trophies at the closing ceremony</div>
                </div>
            </div>
        </div>
    </div>

    <!-- ═══════════════ DAY 1 DIVIDER ═══════════════ -->
    <div class="day-divider">
        <div class="day-divider-inner">
            <div class="day-number-badge">
                <span class="day-word">DAY</span>
                <span class="day-n">1</span>
            </div>
            <div class="day-accent"></div>
            <div class="day-divider-content">
                <h2>Clinical Intelligence &amp; Cultural Engagement</h2>
                <p>08:00 – Opening Ceremony with Traditional Welcome &nbsp;·&nbsp; Parallel Academic Tracks &nbsp;·&nbsp; Hands-On Workshops &nbsp;·&nbsp; Sufi Night &amp; Gala Dinner</p>
            </div>
        </div>
    </div>

    <!-- ═══════════════ DAY 1 SESSIONS ═══════════════ -->
    <div style="background: white;">
        <div class="section">
            <div class="section-header">
                <span class="section-tag">Day 1 — Morning</span>
                <div class="section-line"></div>
            </div>

            <!-- Opening Ceremony -->
            <div class="schedule-block">
                <div class="sb-header maroon-accent">
                    <div class="sb-time">08:00 – 10:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">🎙️</span>
                        <span class="sb-title">Opening Ceremony — Traditional Pakistani Welcome</span>
                    </div>
                </div>
                <div class="sb-body">
                    <ul class="bullet-list">
                        <li>Registration with traditional rose-petal welcome &amp; chai service</li>
                        <li>Recitation from the Holy Quran</li>
                        <li>National Anthem &amp; formal opening</li>
                        <li>Welcome address by organizing committee &amp; Advisor <strong>Dr. Mehmood Nasir Malik</strong></li>
                        <li>Introduction of collaborators, partners, and sponsors</li>
                        <li><strong>Opening Keynote (Plenary Session 1):</strong> Redefining Evidence-Based Internal Medicine in the Era of Artificial Intelligence</li>
                        <li>Cultural showcase: Short Sufi instrumental performance</li>
                    </ul>
                    <div class="cultural-experience-card">
                        <span class="cultural-experience-icon">🌹</span>
                        <span class="cultural-experience-text"><strong>Cultural Touch:</strong> Delegates receive a traditional Pakistani welcome with rose garlands, accompanied by authentic Lahori chai and traditional mithai — setting the tone for a uniquely Pakistani conference experience.</span>
                    </div>
                </div>
            </div>

            <!-- Parallel Tracks -->
            <div class="schedule-block">
                <div class="sb-header gold-accent">
                    <div class="sb-time">10:00 – 13:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">📊</span>
                        <span class="sb-title">Parallel Academic &amp; Competitive Tracks</span>
                    </div>
                </div>
                <div class="sb-body">
                    <div class="tracks-grid">
                        <div class="track-card">
                            <div class="track-card-top">
                                <div class="track-label" style="background: var(--mughal-green);">Track A</div>
                                <div class="track-name">Oral Presentations</div>
                            </div>
                            <div class="track-desc">Research-based oral abstract presentations evaluated by expert panel</div>
                        </div>
                        <div class="track-card">
                            <div class="track-card-top">
                                <div class="track-label" style="background: var(--gold-lahore); color: var(--mughal-green-deep);">Track B</div>
                                <div class="track-name">Clinical Quiz Competition</div>
                            </div>
                            <div class="track-desc">Case-based and concept-driven competitive rounds</div>
                        </div>
                        <div class="track-card">
                            <div class="track-card-top">
                                <div class="track-label" style="background: var(--indigo-tile);">Track C</div>
                                <div class="track-name">Rapid Fire Clinical Challenge</div>
                            </div>
                            <div class="track-desc">ECG interpretation · Image-based diagnosis · Laboratory data interpretation</div>
                        </div>
                    </div>
                    <div class="plenary-note">⬡ Parallel Plenary: AI in Clinical Decision-Making and Diagnostics — running alongside selected tracks</div>
                </div>
            </div>

            <!-- Lunch Day 1 -->
            <div class="schedule-block">
                <div class="sb-header slate-accent">
                    <div class="sb-time">13:00 – 15:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">🍽️</span>
                        <span class="sb-title">Lunch &amp; Networking — Lahori Dastarkhwan</span>
                    </div>
                </div>
                <div class="sb-body">
                    <ul class="bullet-list">
                        <li>Traditional Lahori cuisine served in a communal dastarkhwan setting</li>
                        <li>Live food stations featuring local delicacies</li>
                        <li>Faculty–student networking over cultural tea stalls</li>
                        <li>Collaboration discussions</li>
                    </ul>
                    <div class="cultural-experience-card">
                        <span class="cultural-experience-icon">🍛</span>
                        <span class="cultural-experience-text"><strong>Cultural Touch:</strong> Experience the legendary flavours of Lahore — from aromatic biryani and nihari to freshly prepared naan from a traditional tandoor. A culinary journey through the walled city's most beloved dishes, served in an ambiance inspired by Lahore's historic food streets.</span>
                    </div>
                </div>
            </div>

            <!-- Workshops Day 1 -->
            <div class="schedule-block">
                <div class="sb-header">
                    <div class="sb-time">15:00 – 18:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">🔬</span>
                        <span class="sb-title">Hands-On Workshops — Day 1</span>
                        <span class="sb-subtitle">4 Parallel Sessions · Pre-registration required</span>
                    </div>
                </div>
                <div class="sb-body">
                    <div class="workshops-grid">
                        <div class="ws-card t1">
                            <span class="ws-icon">🔬</span>
                            <div class="ws-label">Workshop 1</div>
                            <div class="ws-name">Clinical Audit &amp; Quality Improvement</div>
                        </div>
                        <div class="ws-card t1">
                            <span class="ws-icon">🎓</span>
                            <div class="ws-label">Workshop 2</div>
                            <div class="ws-name">Peer Review &amp; Scientific Writing</div>
                        </div>
                        <div class="ws-card t1">
                            <span class="ws-icon">🤖</span>
                            <div class="ws-label">Workshop 3</div>
                            <div class="ws-name">AI in Diagnostics</div>
                        </div>
                        <div class="ws-card t1">
                            <span class="ws-icon">❤️</span>
                            <div class="ws-label">Workshop 4</div>
                            <div class="ws-name">BLS / CPR &amp; Emergency Skills</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Gala / Sufi Night -->
            <div class="gala-banner">
                <span class="gala-banner-icon">🌟</span>
                <div class="gala-banner-text">
                    <span>19:00 onwards</span>
                    Sufi Night &amp; Gala Dinner (Optional) — Live Qawwali performance, traditional Pakistani dinner, networking &amp; cultural immersion
                </div>
            </div>
            <div class="cultural-experience-card" style="margin-top:0; border-top:none;">
                <span class="cultural-experience-icon">🎶</span>
                <span class="cultural-experience-text"><strong>Cultural Touch:</strong> An unforgettable evening of live Qawwali — the soul-stirring Sufi devotional music that has echoed through the shrines of Lahore for centuries. Accompanied by a grand Pakistani dinner featuring regional specialties from across all provinces. Delegates experience the spiritual heart of Pakistan's cultural capital.</span>
            </div>
        </div>
    </div>

    <!-- ═══════════════ DAY 2 DIVIDER ═══════════════ -->
    <div class="day-divider day2">
        <div class="day-divider-inner">
            <div class="day-number-badge">
                <span class="day-word">DAY</span>
                <span class="day-n">2</span>
            </div>
            <div class="day-accent"></div>
            <div class="day-divider-content">
                <h2>Research, Innovation &amp; Lahore's Heritage</h2>
                <p>09:00 – Plenary Session 2 &nbsp;·&nbsp; Parallel Academic Tracks &nbsp;·&nbsp; Hands-On Workshops &nbsp;·&nbsp; Cultural Closing Ceremony &amp; Awards</p>
            </div>
        </div>
    </div>

    <!-- ═══════════════ DAY 2 SESSIONS ═══════════════ -->
    <div style="background: white;">
        <div class="section">
            <div class="section-header">
                <span class="section-tag">Day 2 — Full Programme</span>
                <div class="section-line"></div>
            </div>

            <!-- Plenary 2 -->
            <div class="schedule-block">
                <div class="sb-header maroon-accent">
                    <div class="sb-time">09:00 – 10:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">🧠</span>
                        <span class="sb-title">Plenary Session 2</span>
                        <span class="sb-subtitle">AI and the Future of Evidence-Based Medicine</span>
                    </div>
                </div>
                <div class="sb-body">
                    <ul class="bullet-list">
                        <li>Keynote by invited international speaker</li>
                        <li>Panel discussion: Integrating AI into clinical practice in resource-limited settings</li>
                    </ul>
                </div>
            </div>

            <!-- Parallel Tracks Day 2 -->
            <div class="schedule-block">
                <div class="sb-header gold-accent">
                    <div class="sb-time">10:00 – 13:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">📋</span>
                        <span class="sb-title">Parallel Academic &amp; Competitive Tracks</span>
                    </div>
                </div>
                <div class="sb-body">
                    <div class="tracks-grid">
                        <div class="track-card">
                            <div class="track-card-top">
                                <div class="track-label" style="background: var(--mughal-green);">Track A</div>
                                <div class="track-name">Poster Presentations</div>
                            </div>
                            <div class="track-desc">Poster display with interactive judging by expert panel</div>
                        </div>
                        <div class="track-card">
                            <div class="track-card-top">
                                <div class="track-label" style="background: var(--gold-lahore); color: var(--mughal-green-deep);">Track B</div>
                                <div class="track-name">Research Innovation Arena</div>
                            </div>
                            <div class="track-desc">Research idea pitching · Collaboration &amp; mentorship opportunities</div>
                        </div>
                        <div class="track-card">
                            <div class="track-card-top">
                                <div class="track-label" style="background: var(--indigo-tile);">Track C</div>
                                <div class="track-name">Clinical Case Challenge / Diagnostic Arena</div>
                            </div>
                            <div class="track-desc">Case-based discussion · Clinical reasoning &amp; decision-making</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Lunch Day 2 -->
            <div class="schedule-block">
                <div class="sb-header slate-accent">
                    <div class="sb-time">13:00 – 15:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">🍽️</span>
                        <span class="sb-title">Lunch &amp; Cultural Exhibition</span>
                    </div>
                </div>
                <div class="sb-body">
                    <ul class="bullet-list">
                        <li>Multi-province Pakistani cuisine experience</li>
                        <li>Live truck art painting demonstration</li>
                        <li>Islamic calligraphy exhibition &amp; interactive session</li>
                        <li>Traditional handicraft display from across Pakistan</li>
                        <li>Faculty–student networking &amp; collaboration discussions</li>
                    </ul>
                    <div class="cultural-experience-card">
                        <span class="cultural-experience-icon">🎨</span>
                        <span class="cultural-experience-text"><strong>Cultural Touch:</strong> A curated cultural bazaar within Alhamrah — featuring live truck art painting, where delegates can witness the vibrant, iconic art form of Pakistan's highways. Calligraphy masters demonstrate the ancient Islamic art, and regional handicraft stalls showcase the craftsmanship of Sindh, Punjab, Balochistan, Khyber Pakhtunkhwa, Gilgit-Baltistan, and Azad Kashmir.</span>
                    </div>
                </div>
            </div>

            <!-- Workshops Day 2 -->
            <div class="schedule-block">
                <div class="sb-header">
                    <div class="sb-time">15:00 – 18:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">💡</span>
                        <span class="sb-title">Hands-On Workshops — Day 2</span>
                        <span class="sb-subtitle">4 Parallel Sessions · Pre-registration required</span>
                    </div>
                </div>
                <div class="sb-body">
                    <div class="workshops-grid">
                        <div class="ws-card t2">
                            <span class="ws-icon">🧪</span>
                            <div class="ws-label">Workshop 5</div>
                            <div class="ws-name">ABC of Clinical Trials</div>
                        </div>
                        <div class="ws-card t2">
                            <span class="ws-icon">🩻</span>
                            <div class="ws-label">Workshop 6</div>
                            <div class="ws-name">Clinical Radiology Essentials</div>
                        </div>
                        <div class="ws-card t2">
                            <span class="ws-icon">📚</span>
                            <div class="ws-label">Workshop 7</div>
                            <div class="ws-name">USMLE &amp; Clinical Reasoning Lab</div>
                        </div>
                        <div class="ws-card t2">
                            <span class="ws-icon">🤖</span>
                            <div class="ws-label">Workshop 8</div>
                            <div class="ws-name">Advanced AI in Healthcare Applications</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Closing Ceremony -->
            <div class="schedule-block">
                <div class="sb-header gold-accent">
                    <div class="sb-time">18:00 – 20:00</div>
                    <div class="sb-title-wrap">
                        <span class="sb-icon">🏆</span>
                        <span class="sb-title">Cultural Closing Ceremony &amp; Awards</span>
                    </div>
                </div>
                <div class="sb-body">
                    <div class="awards-grid">
                        <div class="award-item"><span class="award-icon">🥇</span> Best Oral Presentation</div>
                        <div class="award-item"><span class="award-icon">🥇</span> Best Poster Presentation</div>
                        <div class="award-item"><span class="award-icon">🥇</span> Best Research Pitch</div>
                        <div class="award-item"><span class="award-icon">🥇</span> Competition Winners</div>
                    </div>
                    <ul class="bullet-list" style="margin-top: 14px;">
                        <li>Acknowledgment of organizing committee, partners, and sponsors</li>
                        <li>Special recognition of Advisor <strong>Dr. Mehmood Nasir Malik</strong></li>
                        <li>Cultural farewell performance — fusion of traditional and contemporary Pakistani music</li>
                        <li>Closing address &amp; distribution of traditional Pakistani craftsmanship trophies</li>
                    </ul>
                    <div class="cultural-experience-card">
                        <span class="cultural-experience-icon">🏆</span>
                        <span class="cultural-experience-text"><strong>Cultural Touch:</strong> Awards and trophies are handcrafted by Pakistani artisans, featuring traditional design elements such as intricate woodwork, brass inlay, and miniature truck art motifs — making each award a unique piece of Pakistani cultural heritage that winners can cherish as a memento of their time in Lahore.</span>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- ═══════════════ AT A GLANCE ═══════════════ -->
    <div style="background: var(--cream);">
        <div class="section">
            <div class="section-header">
                <span class="section-tag">Quick Reference</span>
                <div class="section-line"></div>
            </div>
            <p class="section-title" style="margin-bottom: 24px;">At-a-Glance Schedule</p>
            <div class="glance-grid">
                <div>
                    <div class="glance-col-header d1">Day 1 — Clinical Intelligence &amp; Cultural Engagement</div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--maroon-royal);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--maroon-royal);">08:00 – 10:00</div>
                            <div class="glance-label">Opening Ceremony &amp; Keynote with Traditional Welcome</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--mughal-green);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--mughal-green);">10:00 – 13:00</div>
                            <div class="glance-label">Parallel Tracks A / B / C + Plenary</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--slate);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--slate);">13:00 – 15:00</div>
                            <div class="glance-label">Lahori Dastarkhwan Lunch &amp; Networking</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--mughal-green);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--mughal-green);">15:00 – 18:00</div>
                            <div class="glance-label">4 × Hands-On Workshops</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--gold-lahore);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--gold-lahore);">19:00 onwards</div>
                            <div class="glance-label">Sufi Night &amp; Gala Dinner (Optional)</div>
                        </div>
                    </div>
                </div>
                <div>
                    <div class="glance-col-header d2">Day 2 — Research, Innovation &amp; Lahore's Heritage</div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--maroon-royal);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--maroon-royal);">09:00 – 10:00</div>
                            <div class="glance-label">Plenary Session 2: AI &amp; Future of EBM</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--gold-lahore);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--gold-lahore);">10:00 – 13:00</div>
                            <div class="glance-label">Parallel Tracks A / B / C</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--slate);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--slate);">13:00 – 15:00</div>
                            <div class="glance-label">Lunch &amp; Cultural Exhibition (Bazaar)</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--gold-lahore);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--gold-lahore);">15:00 – 18:00</div>
                            <div class="glance-label">4 × Hands-On Workshops</div>
                        </div>
                    </div>
                    <div class="glance-row">
                        <div class="glance-bar" style="background: var(--gold-lahore);"></div>
                        <div class="glance-row-inner">
                            <div class="glance-time" style="color: var(--gold-lahore);">18:00 – 20:00</div>
                            <div class="glance-label">Cultural Closing Ceremony &amp; Awards</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- ═══════════════ CLOSING ═══════════════ -->
    <div class="closing">
        <div class="closing-inner">
            <span class="closing-icon">🩺</span>
            <h2>International Internal Medicine Conference</h2>
            <p style="color:var(--gold-bright); font-family:'Cormorant Garamond',serif; font-size:20px; font-style:italic; margin-bottom:6px;">— The Lahore Edition —</p>
            <div class="closing-divider"></div>
            <p class="closing-sub">Redefining Evidence-Based Internal Medicine<br>in the Era of Artificial Intelligence<br><span style="color:var(--gold-lahore); font-size:14px;">— Infused with the Soul of Pakistan —</span></p>
            <p class="closing-welcome">We look forward to welcoming you to the cultural heart of Pakistan!</p>
            <p class="closing-org" style="margin-top: 18px;">SCORE IFMSA Pakistan &nbsp;·&nbsp; IIMC 2026 &nbsp;·&nbsp; Alhamrah Arts Council, Lahore</p>
            <p class="closing-org" style="margin-top:6px; color:rgba(255,255,255,0.2);">Under the Guidance of Dr. Mehmood Nasir Malik &nbsp;·&nbsp; Head of Department of Medicine</p>
        </div>
    </div>

    <!-- ═══════════════ FOOTER ═══════════════ -->
    <footer>
        <div class="footer-left">IIMC 2026 &nbsp;·&nbsp; SCORE IFMSA Pakistan &nbsp;·&nbsp; Lahore</div>
        <div class="footer-right">Pakistan's First Culturally-Infused Medical Conference</div>
    </footer>

</body>
</html>

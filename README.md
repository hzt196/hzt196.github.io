<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>和子腾 - 个人简历 | hzt196.github.io</title>
    <meta name="description" content="和子腾的个人简历，展示专业技能、项目经验和教育背景">
    <meta name="keywords" content="和子腾,简历,前端开发,Java,Python,北京邮电大学">
    <meta name="author" content="和子腾">
    <meta name="robots" content="index, follow">
    <link rel="canonical" href="https://hzt196.github.io/">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://hzt196.github.io/">
    <meta property="og:title" content="和子腾 - 个人简历">
    <meta property="og:description" content="和子腾的个人简历，展示专业技能、项目经验和教育背景">
    
    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://hzt196.github.io/">
    <meta property="twitter:title" content="和子腾 - 个人简历">
    <meta property="twitter:description" content="和子腾的个人简历，展示专业技能、项目经验和教育背景">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Microsoft YaHei', 'PingFang SC', 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.6;
            color: #c9d1d9;
            background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }

        .container {
            width: 100%;
            max-width: 1600px;
            min-height: 100vh;
            background: #0d1117;
            display: flex;
            flex-direction: column;
            position: relative;
            margin: 0 auto;
        }

        .header {
            background: linear-gradient(135deg, #161b22 0%, #30363d 100%);
            color: #c9d1d9;
            padding: 80px 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="25" cy="25" r="1" fill="white" opacity="0.1"/><circle cx="75" cy="75" r="1" fill="white" opacity="0.1"/><circle cx="50" cy="10" r="0.5" fill="white" opacity="0.1"/><circle cx="10" cy="60" r="0.5" fill="white" opacity="0.1"/><circle cx="90" cy="40" r="0.5" fill="white" opacity="0.1"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
            opacity: 0.3;
        }

        .github-link {
            position: absolute;
            top: 20px;
            right: 20px;
            background: rgba(255,255,255,0.1);
            color: #c9d1d9;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 0.9em;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }

        .github-link:hover {
            background: rgba(255,255,255,0.2);
            transform: translateY(-2px);
        }

        .header-content {
            position: relative;
            z-index: 1;
        }

        .name {
            font-size: 4.5em;
            font-weight: 700;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            letter-spacing: 3px;
            background: linear-gradient(45deg, #c9d1d9, #58a6ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { filter: drop-shadow(0 0 5px rgba(255,255,255,0.3)); }
            to { filter: drop-shadow(0 0 20px rgba(255,255,255,0.6)); }
        }

        .title {
            font-size: 1.6em;
            opacity: 0.95;
            margin-bottom: 50px;
            font-weight: 300;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.2);
        }

        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
            margin-top: 40px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 12px;
            background: rgba(255,255,255,0.05);
            padding: 18px 30px;
            border-radius: 50px;
            backdrop-filter: blur(15px);
            border: 2px solid rgba(255,255,255,0.1);
            font-size: 1.1em;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .contact-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent);
            transition: left 0.5s;
        }

        .contact-item:hover::before {
            left: 100%;
        }

        .contact-item:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            background: rgba(255,255,255,0.1);
            border-color: rgba(255,255,255,0.2);
        }

        .contact-item:active {
            transform: translateY(-1px) scale(1.02);
        }

        .main-content {
            flex: 1;
            padding: 60px 40px;
            background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
        }

        .content-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            max-width: 1500px;
            margin: 0 auto;
        }

        .left-column, .right-column {
            display: flex;
            flex-direction: column;
            gap: 35px;
        }

        .section {
            background: #161b22;
            border-radius: 25px;
            padding: 35px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.08);
            border-left: 6px solid #58a6ff;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
            cursor: pointer;
        }

        .section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(88, 166, 255, 0.02) 0%, rgba(88, 166, 255, 0.02) 100%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .section:hover::before {
            opacity: 1;
        }

        .section:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: 0 25px 50px rgba(0,0,0,0.15);
            border-left-color: #f85149;
        }

        .section:active {
            transform: translateY(-4px) scale(1.01);
        }

        .section-title {
            font-size: 2em;
            color: #c9d1d9;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 4px solid #58a6ff;
            position: relative;
            font-weight: 700;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, #f85149, #f0883e);
            border-radius: 2px;
        }

        .section-title::before {
            content: '';
            position: absolute;
            bottom: -4px;
            right: 0;
            width: 40px;
            height: 4px;
            background: linear-gradient(90deg, #a371f7, #58a6ff);
            border-radius: 2px;
        }

        .basic-info {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .info-item {
            background: linear-gradient(135deg, #161b22 0%, #21262d 100%);
            padding: 25px;
            border-radius: 20px;
            text-align: center;
            border: 3px solid #30363d;
            transition: all 0.3s ease;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .info-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(88, 166, 255, 0.1) 0%, rgba(88, 166, 255, 0.1) 100%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .info-item:hover::before {
            opacity: 1;
        }

        .info-item:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
            border-color: #58a6ff;
        }

        .info-item:active {
            transform: translateY(-2px) scale(1.02);
        }

        .info-label {
            font-weight: 700;
            color: #c9d1d9;
            margin-bottom: 10px;
            font-size: 1.2em;
            position: relative;
            z-index: 1;
        }

        .info-value {
            color: #8b949e;
            font-size: 1.4em;
            font-weight: 600;
            position: relative;
            z-index: 1;
        }

        .awards-list {
            list-style: none;
        }

        .awards-list li {
            background: linear-gradient(135deg, #21262d 0%, #30363d 100%);
            margin-bottom: 20px;
            padding: 25px;
            border-radius: 20px;
            border-left: 5px solid #f85149;
            position: relative;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 2px solid #484f58;
            cursor: pointer;
            overflow: hidden;
        }

        .awards-list li::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(248, 81, 73, 0.1) 0%, rgba(248, 81, 73, 0.1) 100%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .awards-list li:hover::before {
            opacity: 1;
        }

        .awards-list li:hover {
            transform: translateX(15px) scale(1.02);
            box-shadow: 0 10px 25px rgba(248, 81, 73, 0.25);
            border-left-color: #f0883e;
        }

        .awards-list li:active {
            transform: translateX(8px) scale(1.01);
        }

        .awards-list li::after {
            content: '🏆';
            position: absolute;
            left: -25px;
            top: 50%;
            transform: translateY(-50%);
            background: #161b22;
            padding: 12px;
            border-radius: 50%;
            box-shadow: 0 5px 15px rgba(0,0,0,0.15);
            font-size: 1.3em;
            transition: all 0.3s ease;
        }

        .awards-list li:hover::after {
            transform: translateY(-50%) scale(1.2) rotate(10deg);
            box-shadow: 0 8px 20px rgba(0,0,0,0.2);
        }

        .education-item {
            background: linear-gradient(135deg, #21262d 0%, #30363d 100%);
            padding: 30px;
            border-radius: 25px;
            border-left: 5px solid #238636;
            border: 2px solid #3fb950;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .education-item:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(35, 134, 54, 0.2);
            border-left-color: #2da44e;
        }

        .education-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .school {
            font-size: 1.5em;
            font-weight: 700;
            color: #c9d1d9;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .degree {
            color: #8b949e;
            font-style: italic;
            font-size: 1.2em;
            font-weight: 500;
        }

        .courses {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 25px;
        }

        .course-tag {
            background: linear-gradient(135deg, #58a6ff 0%, #388bfd 100%);
            color: #0d1117;
            padding: 10px 20px;
            border-radius: 25px;
            font-size: 0.95em;
            font-weight: 600;
            box-shadow: 0 4px 10px rgba(88, 166, 255, 0.3);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .course-tag:hover {
            transform: translateY(-3px) scale(1.1);
            box-shadow: 0 8px 20px rgba(88, 166, 255, 0.4);
        }

        .course-tag:active {
            transform: translateY(-1px) scale(1.05);
        }

        .project-item {
            background: linear-gradient(135deg, #21262d 0%, #30363d 100%);
            padding: 30px;
            border-radius: 25px;
            margin-bottom: 30px;
            border-left: 5px solid #a371f7;
            border: 2px solid #d29922;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .project-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(163, 113, 247, 0.1) 0%, rgba(88, 166, 255, 0.1) 100%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .project-item:hover::before {
            opacity: 1;
        }

        .project-item:hover {
            transform: translateY(-8px) scale(1.03);
            box-shadow: 0 20px 40px rgba(163, 113, 247, 0.25);
            border-left-color: #f85149;
        }

        .project-item:active {
            transform: translateY(-4px) scale(1.01);
        }

        .project-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .project-title {
            font-size: 1.4em;
            font-weight: 700;
            color: #c9d1d9;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .project-period {
            color: #8b949e;
            font-size: 0.95em;
            background: rgba(163, 113, 247, 0.15);
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: 600;
        }

        .project-role {
            color: #f85149;
            font-weight: 700;
            margin-bottom: 20px;
            font-size: 1.2em;
        }

        .project-description {
            color: #8b949e;
            line-height: 1.8;
            font-size: 1.1em;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .skill-category {
            background: linear-gradient(135deg, #21262d 0%, #30363d 100%);
            padding: 30px;
            border-radius: 20px;
            border-left: 5px solid #f0883e;
            border: 2px solid #d29922;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .skill-category:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(240, 136, 62, 0.2);
            border-left-color: #d29922;
        }

        .skill-category h4 {
            color: #c9d1d9;
            margin-bottom: 20px;
            font-size: 1.3em;
            font-weight: 700;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
        }

        .skill-tag {
            background: linear-gradient(135deg, #f0883e 0%, #d29922 100%);
            color: #0d1117;
            padding: 10px 20px;
            border-radius: 25px;
            font-size: 0.8em;
            font-weight: 600;
            box-shadow: 0 4px 10px rgba(240, 136, 62, 0.3);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .skill-tag:hover {
            transform: translateY(-3px) scale(1.1);
            box-shadow: 0 8px 20px rgba(240, 136, 62, 0.4);
        }

        .skill-tag:active {
            transform: translateY(-1px) scale(1.05);
        }

        .self-evaluation {
            background: linear-gradient(135deg, #21262d 0%, #30363d 100%);
            padding: 35px;
            border-radius: 25px;
            border-left: 5px solid #39d353;
            font-style: italic;
            color: #8b949e;
            line-height: 1.9;
            font-size: 1.15em;
            border: 2px solid #238636;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .self-evaluation:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(57, 211, 83, 0.2);
            border-left-color: #238636;
        }

        .internship-item {
            background: linear-gradient(135deg, #21262d 0%, #30363d 100%);
            padding: 30px;
            border-radius: 25px;
            border-left: 5px solid #f0883e;
            border: 2px solid #d29922;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .internship-item:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(240, 136, 62, 0.2);
            border-left-color: #d29922;
        }

        .internship-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .company {
            font-size: 1.4em;
            font-weight: 700;
            color: #c9d1d9;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .position {
            color: #f85149;
            font-weight: 700;
            font-size: 1.2em;
        }

        .full-width {
            grid-column: 1 / -1;
        }

        .footer {
            background: linear-gradient(135deg, #161b22 0%, #21262d 100%);
            color: #c9d1d9;
            text-align: center;
            padding: 30px;
            margin-top: 50px;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-bottom: 20px;
        }

        .footer-links a {
            color: #c9d1d9;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 20px;
            background: rgba(255,255,255,0.05);
            transition: all 0.3s ease;
        }

        .footer-links a:hover {
            background: rgba(255,255,255,0.1);
            transform: translateY(-2px);
        }

        .footer-text {
            opacity: 0.8;
            font-size: 0.9em;
        }

        /* 响应式设计 - 大屏幕优化 */
        @media (min-width: 1600px) {
            .container {
                max-width: 1600px;
                margin: 0 auto;
            }
            
            .main-content {
                padding: 80px 60px;
            }
            
            .section {
                padding: 45px;
            }
            
            .name {
                font-size: 5em;
            }
        }

        /* 中等屏幕 - 平板横屏 */
        @media (max-width: 1200px) {
            .content-grid {
                grid-template-columns: 1fr;
                gap: 40px;
            }
            
            .skills-grid {
                grid-template-columns: 1fr;
            }
            
            .main-content {
                padding: 50px 30px;
            }
            
            .section {
                padding: 30px;
            }
        }

        /* 平板竖屏和小屏幕 */
        @media (max-width: 992px) {
            .header {
                padding: 60px 30px;
            }
            
            .name {
                font-size: 3.5em;
                letter-spacing: 2px;
            }
            
            .title {
                font-size: 1.4em;
            }
            
            .contact-info {
                gap: 20px;
            }
            
            .contact-item {
                padding: 15px 25px;
                font-size: 1em;
            }
            
            .main-content {
                padding: 40px 25px;
            }
            
            .section {
                padding: 25px;
                margin-bottom: 20px;
            }
            
            .section-title {
                font-size: 1.8em;
                margin-bottom: 20px;
            }
            
            .basic-info {
                grid-template-columns: repeat(2, 1fr);
                gap: 20px;
            }
            
            .info-item {
                padding: 20px;
            }
            
            .info-label {
                font-size: 1.1em;
            }
            
            .info-value {
                font-size: 1.3em;
            }
        }

        /* 手机横屏 */
        @media (max-width: 768px) {
            .header {
                padding: 40px 20px;
            }

            .name {
                font-size: 2.8em;
                letter-spacing: 1px;
                margin-bottom: 15px;
            }

            .title {
                font-size: 1.2em;
                margin-bottom: 30px;
            }

            .contact-info {
                flex-direction: column;
                gap: 15px;
                margin-top: 30px;
            }
            
            .contact-item {
                padding: 12px 20px;
                font-size: 0.95em;
                width: 100%;
                justify-content: center;
            }

            .main-content {
                padding: 30px 20px;
            }
            
            .section {
                padding: 20px;
                margin-bottom: 15px;
            }
            
            .section-title {
                font-size: 1.6em;
                margin-bottom: 15px;
                padding-bottom: 10px;
            }

            .education-header,
            .project-header,
            .internship-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
            
            .project-header {
                margin-bottom: 15px;
            }

            .basic-info {
                grid-template-columns: 1fr;
                gap: 15px;
            }
            
            .info-item {
                padding: 15px;
            }
            
            .info-label {
                font-size: 1em;
                margin-bottom: 8px;
            }
            
            .info-value {
                font-size: 1.2em;
            }
            
            .awards-list li {
                padding: 20px;
                margin-bottom: 15px;
            }
            
            .education-item,
            .project-item,
            .internship-item {
                padding: 20px;
            }
            
            .school,
            .company,
            .project-title {
                font-size: 1.3em;
            }
            
            .degree,
            .position,
            .project-role {
                font-size: 1.1em;
            }
            
            .project-description {
                font-size: 1em;
                line-height: 1.6;
            }
            
            .skill-category {
                padding: 20px;
            }
            
            .skill-category h4 {
                font-size: 1.2em;
                margin-bottom: 15px;
            }
            
            .skill-tag {
                padding: 8px 16px;
                font-size: 0.85em;
            }
            
            .course-tag {
                padding: 8px 16px;
                font-size: 0.9em;
            }
            
            .self-evaluation {
                padding: 25px;
                font-size: 1.1em;
                line-height: 1.7;
            }
        }

        /* 小屏手机 */
        @media (max-width: 480px) {
            .header {
                padding: 30px 15px;
            }

            .name {
                font-size: 2.2em;
                letter-spacing: 0.5px;
                margin-bottom: 10px;
            }

            .title {
                font-size: 1em;
                margin-bottom: 25px;
            }

            .contact-info {
                margin-top: 25px;
            }
            
            .contact-item {
                padding: 10px 15px;
                font-size: 0.9em;
            }

            .main-content {
                padding: 20px 15px;
            }
            
            .section {
                padding: 15px;
                margin-bottom: 10px;
            }
            
            .section-title {
                font-size: 1.4em;
                margin-bottom: 12px;
                padding-bottom: 8px;
            }

            .basic-info {
                gap: 10px;
            }
            
            .info-item {
                padding: 12px;
            }
            
            .info-label {
                font-size: 0.95em;
                margin-bottom: 6px;
            }
            
            .info-value {
                font-size: 1.1em;
            }
            
            .awards-list li {
                padding: 15px;
                margin-bottom: 12px;
                font-size: 0.95em;
            }
            
            .education-item,
            .project-item,
            .internship-item {
                padding: 15px;
            }
            
            .school,
            .company,
            .project-title {
                font-size: 1.2em;
            }
            
            .degree,
            .position,
            .project-role {
                font-size: 1em;
            }
            
            .project-description {
                font-size: 0.95em;
                line-height: 1.5;
            }
            
            .skill-category {
                padding: 15px;
            }
            
            .skill-category h4 {
                font-size: 1.1em;
                margin-bottom: 12px;
            }
            
            .skill-tag {
                padding: 6px 12px;
                font-size: 0.8em;
            }
            
            .course-tag {
                padding: 6px 12px;
                font-size: 0.85em;
            }
            
            .self-evaluation {
                padding: 20px;
                font-size: 1em;
                line-height: 1.6;
            }
            
            .courses {
                gap: 8px;
            }
            
            .skill-tags {
                gap: 8px;
            }
        }

        /* 超小屏设备 */
        @media (max-width: 360px) {
            .name {
                font-size: 1.8em;
            }
            
            .title {
                font-size: 0.9em;
            }
            
            .contact-item {
                padding: 8px 12px;
                font-size: 0.85em;
            }
            
            .main-content {
                padding: 15px 10px;
            }
            
            .section {
                padding: 12px;
            }
            
            .section-title {
                font-size: 1.3em;
            }
            
            .info-item {
                padding: 10px;
            }
            
            .skill-tag,
            .course-tag {
                padding: 5px 10px;
                font-size: 0.75em;
            }
        }

        /* 横屏手机优化 */
        @media (max-height: 500px) and (orientation: landscape) {
            .header {
                padding: 20px 30px;
            }
            
            .name {
                font-size: 2.5em;
                margin-bottom: 10px;
            }
            
            .title {
                font-size: 1.1em;
                margin-bottom: 20px;
            }
            
            .contact-info {
                margin-top: 20px;
                flex-direction: row;
                flex-wrap: wrap;
                gap: 15px;
            }
            
            .main-content {
                padding: 20px 30px;
            }
        }

        /* 高分辨率屏幕优化 */
        @media (-webkit-min-device-pixel-ratio: 2), (min-resolution: 192dpi) {
            .section {
                box-shadow: 0 8px 25px rgba(0,0,0,0.06);
            }
            
            .contact-item {
                border: 1px solid rgba(255,255,255,0.1);
            }
        }

        /* GitHub Pages 移动端优化 */
        @media (max-width: 768px) {
            .github-link {
                top: 15px;
                right: 15px;
                padding: 8px 15px;
                font-size: 0.8em;
            }
            
            .footer-links {
                flex-direction: column;
                gap: 15px;
            }
            
            .footer-links a {
                padding: 8px 15px;
            }
        }

        .fade-in {
            animation: fadeIn 1.2s ease-in;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .section {
            animation: slideIn 1s ease-out;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        /* 添加点击波纹效果 */
        .ripple {
            position: relative;
            overflow: hidden;
        }

        .ripple::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            transform: translate(-50%, -50%);
            transition: width 0.6s, height 0.6s;
        }

        .ripple:active::after {
            width: 300px;
            height: 300px;
        }

        .ripple-effect {
            position: absolute;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.2);
            transform: scale(0);
            animation: ripple-animation 0.6s linear;
            pointer-events: none;
        }

        @keyframes ripple-animation {
            to {
                transform: scale(4);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container fade-in">
        <header class="header">
            <a href="https://github.com/hzt196" class="github-link" target="_blank">
                <i>📱</i> GitHub
            </a>
            <div class="header-content">
                <h1 class="name">和子腾</h1>
                <p class="title">电信工程 | 北京邮电大学</p>
                <div class="contact-info">
                    <div class="contact-item ripple">
                        <span>👨</span>   
                        <span>15188830026 (同微信)</span>
                    </div>
                    <div class="contact-item ripple">
                        <span>📧</span>
                        <span>heziteng666@bupt.edu.cn</span>
                    </div>
                    <div class="contact-item ripple">
                        <span>👨</span>
                        <span>男 | 2004年</span>
                    </div>
                </div>
            </div>
        </header>

        <main class="main-content">
            <div class="content-grid">
                <!-- 左列 -->
                <div class="left-column">
                    <!-- 基本信息 -->
                    <section class="section ripple">
                        <h2 class="section-title">基本信息</h2>
                        <div class="basic-info">
                            <div class="info-item ripple">
                                <div class="info-label">GPA</div>
                                <div class="info-value">87</div>
                            </div>
                            <div class="info-item ripple">
                                <div class="info-label">IELTS</div>
                                <div class="info-value">6.0</div>
                            </div>
                            <div class="info-item ripple">
                                <div class="info-label">专业</div>
                                <div class="info-value">电信工程及管理</div>
                            </div>
                            <div class="info-item ripple">
                                <div class="info-label">学校</div>
                                <div class="info-value">北京邮电大学<br>英国玛丽女王大学</div>
                            </div>
                        </div>
                    </section>

                    <!-- 自我评价 -->
                    <section class="section ripple">
                        <h2 class="section-title">自我评价</h2>
                        <div class="self-evaluation">
                            我是一名热衷于单片机嵌入式AI开发并且具有全流程科研能力的学生，持续打磨技术、善于沟通、乐于协作，期待在未来不断学习并为团队贡献自己的力量。
                        </div>
                    </section>

                    <!-- 相关技能 -->
                    <section class="section ripple">
                        <h2 class="section-title">相关技能</h2>
                        <div class="skills-grid">
                            <div class="skill-category">
                                <h4>核心技术栈</h4>
                                <div class="skill-tags">
                                    <span class="skill-tag">Python</span>
                                    <span class="skill-tag">C++</span>
                                    <span class="skill-tag">VHDL</span>
                                    <span class="skill-tag">STM32CubeIDE</span>
                                    <span class="skill-tag">Keil MDK</span>
                                    <span class="skill-tag">Cadence Virtuoso</span>
                                    <span class="skill-tag">Linux</span>
                                </div>
                            </div>
                            <div class="skill-category">
                                <h4>AI开发体系</h4>
                                <div class="skill-tags">
                                    <span class="skill-tag">PyTorch</span>
                                    <span class="skill-tag">ONNX</span>
                                    <span class="skill-tag">TensorRT</span>
                                    <span class="skill-tag">深度学习</span>
                                    <span class="skill-tag">Transformer</span>
                                </div>
                            </div>
                            <div class="skill-category">
                                <h4>工程实施能力</h4>
                                <div class="skill-tags">
                                    <span class="skill-tag">STM32</span>
                                    <span class="skill-tag">CST Design</span>
                                    <span class="skill-tag">MATLAB</span>
                                    <span class="skill-tag">嵌入式开发</span>
                                    <span class="skill-tag">硬件设计</span>
                                </div>
                            </div>
                            <div class="skill-category">
                                <h4>研发协作支撑</h4>
                                <div class="skill-tags">
                                    <span class="skill-tag">Git</span>
                                    <span class="skill-tag">版本控制</span>
                                    <span class="skill-tag">项目管理</span>
                                    <span class="skill-tag">敏捷协作</span>
                                    <span class="skill-tag">跨团队合作</span>
                                </div>
                            </div>
                        </div>
                    </section>

                    <!-- 荣誉奖项 -->
                    <section class="section ripple">
                        <h2 class="section-title">荣誉奖项</h2>
                        <ul class="awards-list">
                            <li>大学生创新创业训练计划，国家级评审 (2024)</li>
                            <li>第六届中国研究生人工智能创新大赛(华为杯)，国家三等奖 (2024)</li>
                            <li>中国大学生"互联网+"创新创业大赛，北京邮电大学赛区二等奖 (2023)</li>
                            <li>第二届"英语世界"杯全国大学生翻译大赛，全国三等奖 (2022)</li>
                            <li>大学英语四级、大学英语六级</li>
                        </ul>
                    </section>
                </div>

                <!-- 右列 -->
                <div class="right-column">
                    <!-- 教育经历 -->
                    <section class="section ripple">
                        <h2 class="section-title">教育经历</h2>
                        <div class="education-item">
                            <div class="education-header">
                                <div class="school">北京邮电大学</div>
                                <div class="degree">2022.9 - 2026.6</div>
                            </div>
                            <div class="degree">电信工程及管理 | 本科</div>
                            <div style="margin-top: 20px;">
                                <strong>主修课程：</strong>模拟电路、信号与系统、数字电路设计、微处理器系统设计、数字信号处理、通信原理、电磁场与电磁波、互联网协议与网络、高级网络编程
                            </div>
                            <div class="courses">
                                <span class="course-tag">C语言</span>
                                <span class="course-tag">数据结构</span>
                                <span class="course-tag">JAVA</span>
                                <span class="course-tag">Python</span>
                                <span class="course-tag">VHDL技术</span>
                                <span class="course-tag">人工智能导论</span>
                                <span class="course-tag">深度学习</span>
                                <span class="course-tag">Linux系统</span>
                                <span class="course-tag">模拟CMOS集成电路设计</span>
                                <span class="course-tag">数字集成电路设计</span>
                            </div>
                        </div>
                    </section>

                    <!-- 项目经历 -->
                    <section class="section full-width ripple">
                        <h2 class="section-title">项目经历</h2>
                        
                        <div class="project-item">
                            <div class="project-header">
                                <div class="project-title">中国科学院自动化研究所</div>
                                <div class="project-period">2025.3 - 至今</div>
                            </div>
                            <div class="project-role">侯增广教授-李国涛教授-科研实习生</div>
                            <div class="project-description">
                                <strong>呼吸采集系统设计：</strong>主导设计并实现基于单片机的呼吸信号采集系统，采用嵌入式开发技术优化系统性能，确保高精度、低延迟的生理信号采集与处理。<br><br>
                                <strong>节点预测网络架构设计：</strong>负责开发用于预测呼吸关键节点的人工智能Transformer网络架构，结合嵌入式系统实现高效数据处理与实时反馈。
                            </div>
                        </div>

                        <div class="project-item">
                            <div class="project-header">
                                <div class="project-title">CMOS近似加法器设计</div>
                                <div class="project-period">2024.10 - 2025.5</div>
                            </div>
                            <div class="project-role">科研实习生</div>
                            <div class="project-description">
                                <strong>核心成果：</strong>以第一作者在2025 IEEE ICSECE发表论文"A Dual-Mode Precision Configurable: Error-Correctable Adder for Energy-Efficient Applications"，获EI Compendex等数据库收录。<br><br>
                                <strong>技术突破：</strong>创新双模式可配置精度架构，实现动态容错与能耗优化，提升神经网络加速器能效。
                            </div>
                        </div>

                        <div class="project-item">
                            <div class="project-header">
                                <div class="project-title">智能语音与情感交互实验室</div>
                                <div class="project-period">2023.9 - 2024.9</div>
                            </div>
                            <div class="project-role">李雅教授-科研实习</div>
                            <div class="project-description">
                                <strong>垃圾分类低开销框架：</strong>以第二作者发表"A Low-overhead Framework for Trash Classification Based on DenseNet"被ICCEA 2025接收，并由IEEE CSCPS出版，收录于EI Compendex、CNKI及Scopus数据库。<br><br>
                                <strong>"康慧培优"便民医疗陪护系统：</strong>提供AI技术支持，主导智能陪护模块开发与医疗数据可视化，优化用户体验。项目获"互联网+"校级二等奖及国家级大创结项。<br><br>
                                <strong>反电信网络诈骗AI Agent平台：</strong>参与智能代理系统开发，构建反诈骗模型并优化训练流程，显著提升平台识别率。团队荣获华为杯全国三等奖。
                            </div>
                        </div>
                    </section>

                    <!-- 实习经历 -->
                    <section class="section ripple">
                        <h2 class="section-title">实习经历</h2>
                        <div class="internship-item">
                            <div class="internship-header">
                                <div class="company">北京志凌海纳科技股份有限公司 (SmartX)</div>
                                <div class="project-period">2025.7 - 2026.1</div>
                            </div>
                            <div class="position">硬件兼容性测试实习工程师</div>
                            <div class="project-description">
                                负责在服务器部署SMTX OS系统、配置网络及部署集群，运用Linux操作系统，结合VMware，开展虚拟化分布式系统领域测试及超融合硬件兼容与一体化产品测试，支撑公司IT基础设施产品线，保障硬件适配性。
                            </div>
                        </div>
                    </section>
                </div>
            </div>
        </main>
        
        <footer class="footer">
            <div class="footer-content">
                <div class="footer-links">
                    <a href="https://github.com/hzt196" target="_blank">GitHub</a>
                    <a href="mailto:heziteng666@bupt.edu.cn">Email</a>
                    <a href="tel:15188830026">Phone</a>
                </div>
                <div class="footer-text">
                    <p>&copy; 2024 和子腾. 个人简历 | 托管于 GitHub Pages</p>
                </div>
            </div>
        </footer>
    </div>

    <script>
        // 添加滚动动画效果
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

        // 观察所有section元素
        document.querySelectorAll('.section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(30px)';
            section.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
            observer.observe(section);
        });

        // 添加点击音效和触觉反馈
        document.querySelectorAll('.ripple').forEach(element => {
            element.addEventListener('click', function(e) {
                // 创建波纹效果
                const ripple = document.createElement('span');
                const rect = this.getBoundingClientRect();
                const size = Math.max(rect.width, rect.height);
                const x = e.clientX - rect.left - size / 2;
                const y = e.clientY - rect.top - size / 2;
                
                ripple.style.width = ripple.style.height = size + 'px';
                ripple.style.left = x + 'px';
                ripple.style.top = y + 'px';
                ripple.classList.add('ripple-effect');
                
                this.appendChild(ripple);
                
                setTimeout(() => {
                    ripple.remove();
                }, 600);
            });
        });

        // 添加键盘导航支持
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Enter' || e.key === ' ') {
                const focused = document.activeElement;
                if (focused && focused.classList.contains('ripple')) {
                    e.preventDefault();
                    focused.click();
                }
            }
        });
    </script>
</body>
</html>

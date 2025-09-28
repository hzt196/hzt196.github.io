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
            color: #333;
            background: #ffffff;
            min-height: 100vh;
            overflow-x: hidden;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            min-height: 100vh;
            background: #ffffff;
            display: flex;
            flex-direction: column;
            position: relative;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            background: #f8f9fa;
            color: #333;
            padding: 60px 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            margin-bottom: 40px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .header:hover {
            box-shadow: 0 8px 24px rgba(0,0,0,0.15);
        }

        .github-link {
            position: absolute;
            top: 20px;
            right: 20px;
            background: #e9ecef;
            color: #333;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 0.9em;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
        }

        .github-link:hover {
            background: #dee2e6;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .header-content {
            position: relative;
            z-index: 1;
        }

        .name {
            font-size: 3.5em;
            font-weight: 700;
            margin-bottom: 15px;
            letter-spacing: 2px;
            color: #007bff;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        .title {
            font-size: 1.4em;
            margin-bottom: 40px;
            font-weight: 300;
            color: #666;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            background: #ffffff;
            padding: 15px 25px;
            border-radius: 30px;
            font-size: 1em;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .contact-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #f0f4ff;
        }

        .main-content {
            flex: 1;
            padding: 0 20px;
            display: flex;
            flex-direction: column;
            gap: 30px;
        }

        .section {
            background: #ffffff;
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-left: 5px solid #007bff;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            cursor: pointer;
        }

        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-left-color: #0056b3;
        }

        .section-title {
            font-size: 1.8em;
            color: #333;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #007bff;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .basic-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
        }

        .info-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
            cursor: pointer;
        }

        .info-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #e9ecef;
        }

        .info-label {
            font-weight: 600;
            color: #333;
            margin-bottom: 8px;
            font-size: 1.1em;
        }

        .info-value {
            color: #666;
            font-size: 1.3em;
            font-weight: 500;
        }

        .awards-list {
            list-style: none;
        }

        .awards-list li {
            background: #f8f9fa;
            margin-bottom: 15px;
            padding: 20px;
            border-radius: 15px;
            border-left: 5px solid #dc3545;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .awards-list li:hover {
            transform: translateX(10px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #ffe5e5;
        }

        .awards-list li::before {
            content: '🏆';
            font-size: 1.2em;
        }

        .education-item {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #28a745;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
        }

        .education-item:hover {
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #e6ffe6;
        }

        .education-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .school {
            font-size: 1.4em;
            font-weight: 600;
            color: #333;
        }

        .degree {
            color: #666;
            font-size: 1.1em;
        }

        .courses {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 20px;
        }

        .course-tag {
            background: #007bff;
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9em;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .course-tag:hover {
            transform: scale(1.05);
            box-shadow: 0 2px 5px rgba(0,123,255,0.3);
        }

        .project-item {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 15px;
            margin-bottom: 25px;
            border-left: 5px solid #6f42c1;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
        }

        .project-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #f3e8ff;
        }

        .project-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .project-title {
            font-size: 1.3em;
            font-weight: 600;
            color: #333;
        }

        .project-period {
            color: #666;
            font-size: 0.9em;
            background: #e9ecef;
            padding: 6px 12px;
            border-radius: 15px;
        }

        .project-role {
            color: #dc3545;
            font-weight: 600;
            margin-bottom: 15px;
            font-size: 1.1em;
        }

        .project-description {
            color: #666;
            line-height: 1.7;
            font-size: 1em;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .skill-category {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #fd7e14;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
            cursor: pointer;
        }

        .skill-category:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #fff3e6;
        }

        .skill-category h4 {
            color: #333;
            margin-bottom: 15px;
            font-size: 1.2em;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill-tag {
            background: #fd7e14;
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.85em;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .skill-tag:hover {
            transform: scale(1.05);
            box-shadow: 0 2px 5px rgba(253,126,20,0.3);
        }

        .self-evaluation {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 15px;
            border-left: 5px solid #17a2b8;
            color: #666;
            line-height: 1.8;
            font-size: 1.05em;
            border: 1px solid #dee2e6;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .self-evaluation:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #e6f7ff;
        }

        .internship-item {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #ffc107;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
        }

        .internship-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            background: #fff3cd;
        }

        .internship-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .company {
            font-size: 1.3em;
            font-weight: 600;
            color: #333;
        }

        .position {
            color: #dc3545;
            font-weight: 600;
            font-size: 1.1em;
        }

        .footer {
            background: #f8f9fa;
            color: #333;
            text-align: center;
            padding: 25px;
            margin-top: 40px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .footer:hover {
            box-shadow: 0 8px 24px rgba(0,0,0,0.15);
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin-bottom: 15px;
        }

        .footer-links a {
            color: #333;
            text-decoration: none;
            padding: 8px 16px;
            border-radius: 15px;
            background: #ffffff;
            transition: all 0.3s ease;
            border: 1px solid #dee2e6;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .footer-links a:hover {
            background: #e9ecef;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .footer-text {
            opacity: 0.8;
            font-size: 0.9em;
        }

        /* Ripple effect */
        .ripple {
            position: relative;
            overflow: hidden;
        }

        .ripple-effect {
            position: absolute;
            border-radius: 50%;
            background: rgba(0, 123, 255, 0.2);
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

        /* Animations */
        .fade-in {
            animation: fadeIn 1s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .section {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.5s ease, transform 0.5s ease;
        }

        .section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* 响应式设计 */
        @media (max-width: 1200px) {
            .container {
                max-width: 100%;
                padding: 15px;
            }
        }

        @media (max-width: 768px) {
            .header {
                padding: 40px 20px;
            }

            .name {
                font-size: 2.5em;
            }

            .title {
                font-size: 1.2em;
            }

            .contact-info {
                flex-direction: column;
                gap: 15px;
            }

            .contact-item {
                width: 100%;
                justify-content: center;
            }

            .main-content {
                padding: 0 15px;
            }

            .section {
                padding: 25px;
            }

            .section-title {
                font-size: 1.6em;
            }

            .basic-info {
                grid-template-columns: 1fr;
            }

            .education-header,
            .project-header,
            .internship-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
        }

        @media (max-width: 480px) {
            .header {
                padding: 30px 15px;
            }

            .name {
                font-size: 2em;
            }

            .title {
                font-size: 1em;
            }

            .section {
                padding: 20px;
            }

            .section-title {
                font-size: 1.4em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header ripple fade-in">
            <a href="https://github.com/hzt196" class="github-link" target="_blank">
                GitHub
            </a>
            <div class="header-content">
                <h1 class="name">和子腾</h1>
                <p class="title">电信工程及管理专业 | 北京邮电大学</p>
                <div class="contact-info">
                    <div class="contact-item ripple">
                        <span>📞</span>   
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
            <!-- 基本信息 -->
            <section class="section ripple">
                <h2 class="section-title"><span>ℹ️</span>基本信息</h2>
                <div class="basic-info">
                    <div class="info-item ripple">
                        <div class="info-label">GPA</div>
                        <div class="info-value">87.35</div>
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

            <!-- 教育经历 -->
            <section class="section ripple">
                <h2 class="section-title"><span>🎓</span>教育经历</h2>
                <div class="education-item">
                    <div class="education-header">
                        <div class="school">北京邮电大学</div>
                        <div class="degree">2022.9 - 2026.6</div>
                    </div>
                    <div class="degree">电信工程及管理 | 本科</div>
                    <div style="margin-top: 15px;">
                        <strong>主修课程：</strong>模拟电路、信号与系统、数字电路设计、微处理器系统设计、数字信号处理、通信原理、电磁场与电磁波、互联网协议与网络、高级网络编程
                    </div>
                    <div class="courses">
                        <span class="course-tag">数据结构</span>
                        <span class="course-tag">JAVA</span>
                        <span class="course-tag">Python</span>
                        <span class="course-tag">VHDL技术</span>
                        <span class="course-tag">深度学习</span>
                        <span class="course-tag">Linux系统</span>
                        <span class="course-tag">模拟CMOS集成电路设计</span>
                        <span class="course-tag">数字集成电路设计</span>
                    </div>
                </div>
            </section>

            <!-- 实习经历 -->
            <section class="section ripple">
                <h2 class="section-title"><span>💼</span>实习经历</h2>
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

            <!-- 项目经历 -->
            <section class="section ripple">
                <h2 class="section-title"><span>🚀</span>项目经历</h2>
                
                <div class="project-item ripple">
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

                <div class="project-item ripple">
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

                <div class="project-item ripple">
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

            <!-- 荣誉奖项 -->
            <section class="section ripple">
                <h2 class="section-title"><span>🏅</span>荣誉奖项</h2>
                <ul class="awards-list">
                    <li>大学生创新创业训练计划，国家级评审 (2024)</li>
                    <li>第六届中国研究生人工智能创新大赛(华为杯)，国家三等奖 (2024)</li>
                    <li>中国大学生"互联网+"创新创业大赛，北京邮电大学赛区二等奖 (2023)</li>
                    <li>第二届"英语世界"杯全国大学生翻译大赛，全国三等奖 (2022)</li>
                    <li>大学英语四级、大学英语六级</li>
                </ul>
            </section>

            <!-- 相关技能 -->
            <section class="section ripple">
                <h2 class="section-title"><span>🛠️</span>相关技能</h2>
                <div class="skills-grid">
                    <div class="skill-category ripple">
                        <h4><span>🔥</span>核心技术栈</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Python</span>
                            <span class="skill-tag">Linux系统</span>
                            <span class="skill-tag">Keil MDK</span>
                            <span class="skill-tag">Virtuoso</span>
                            <span class="skill-tag">STM32CubeIDE</span>

 
                        </div>
                    </div>
                    <div class="skill-category ripple">
                        <h4><span>🤖</span>AI开发体系</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">PyTorch</span>
                            <span class="skill-tag">ONNX</span>
                            <span class="skill-tag">TensorRT</span>
                            <span class="skill-tag">深度学习</span>
                            <span class="skill-tag">Transformer</span>
                        </div>
                    </div>
                    <div class="skill-category ripple">
                        <h4><span>⚙️</span>工程实施能力</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">STM32</span>
                            <span class="skill-tag">CST Design</span>
                            <span class="skill-tag">MATLAB</span>
                            <span class="skill-tag">嵌入式开发</span>
                            <span class="skill-tag">硬件设计</span>
                        </div>
                    </div>
                    <div class="skill-category ripple">
                        <h4><span>🤝</span>研发协作支撑</h4>
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

            <!-- 自我评价 -->
            <section class="section ripple">
                <h2 class="section-title"><span>💬</span>自我评价</h2>
                <div class="self-evaluation">
                    我是一名热衷于单片机嵌入式AI开发并且具有全流程科研能力的学生，持续打磨技术、善于沟通、乐于协作，期待在未来不断学习并为团队贡献自己的力量。
                </div>
            </section>
        </main>
        
        <footer class="footer ripple">
            <div class="footer-content">
                <div class="footer-links">
                    <a href="https://github.com/hzt196" target="_blank"><span>🔗</span>GitHub</a>
                    <a href="mailto:heziteng666@bupt.edu.cn"><span>📧</span>Email</a>
                    <a href="tel:15188830026"><span>📞</span>Phone</a>
                </div>
                <div class="footer-text">
                    <p>&copy; 2025 和子腾. 个人简历 | 托管于 GitHub Pages</p>
                </div>
            </div>
        </footer>
    </div>

    <script>
        // Ripple effect
        document.querySelectorAll('.ripple').forEach(element => {
            element.addEventListener('click', function(e) {
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

        // Intersection Observer for fade-in
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    observer.unobserve(entry.target);
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.section').forEach(section => {
            observer.observe(section);
        });
    </script>
</body>
</html>

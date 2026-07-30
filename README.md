<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>作品集 · 医疗影像系统</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Segoe UI', 'Microsoft YaHei', -apple-system, sans-serif;
            background: #f0f4f8;
            color: #1e293b;
            min-height: 100vh;
        }
        .hero {
            background: linear-gradient(135deg, #0f172a 0%, #1e3a5f 40%, #2563eb 100%);
            padding: 64px 24px 48px;
            text-align: center;
            color: #fff;
        }
        .hero h1 {
            font-size: 2.2rem;
            font-weight: 700;
            letter-spacing: 1px;
            margin-bottom: 12px;
        }
        .hero p {
            font-size: 1rem;
            color: #94a3b8;
            max-width: 520px;
            margin: 0 auto;
            line-height: 1.6;
        }
        .container {
            max-width: 1120px;
            margin: -32px auto 60px;
            padding: 0 24px;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(500px, 1fr));
            gap: 24px;
        }
        .card {
            background: #fff;
            border-radius: 20px;
            padding: 28px 32px;
            box-shadow: 0 4px 16px rgba(0,0,0,0.04), 0 1px 4px rgba(0,0,0,0.02);
            transition: transform 0.2s, box-shadow 0.2s;
            display: flex;
            flex-direction: column;
            gap: 16px;
        }
        .card:hover {
            transform: translateY(-4px);
            box-shadow: 0 12px 32px rgba(0,0,0,0.08), 0 2px 8px rgba(0,0,0,0.04);
        }
        .card-header {
            display: flex;
            align-items: flex-start;
            gap: 16px;
        }
        .card-icon {
            width: 48px;
            height: 48px;
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 22px;
            flex-shrink: 0;
        }
        .icon-report { background: #eef2ff; color: #4f46e5; }
        .icon-empi   { background: #ecfdf5; color: #059669; }
        .icon-forum  { background: #fef3c7; color: #d97706; }
        .icon-book   { background: #fce7f3; color: #db2777; }
        .card-title {
            font-size: 1.15rem;
            font-weight: 700;
            color: #0f172a;
            line-height: 1.4;
        }
        .card-subtitle {
            font-size: 0.8rem;
            color: #64748b;
            margin-top: 2px;
        }
        .card-desc {
            font-size: 0.875rem;
            color: #475569;
            line-height: 1.65;
            flex: 1;
        }
        .card-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }
        .tag {
            font-size: 0.7rem;
            padding: 4px 12px;
            border-radius: 20px;
            background: #f1f5f9;
            color: #475569;
            font-weight: 500;
        }
        .card-actions {
            display: flex;
            gap: 12px;
            padding-top: 4px;
            border-top: 1px solid #f1f5f9;
        }
        .btn {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            padding: 10px 22px;
            border-radius: 12px;
            font-size: 0.85rem;
            font-weight: 600;
            text-decoration: none;
            cursor: pointer;
            transition: all 0.2s;
            border: none;
        }
        .btn-primary {
            background: #2563eb;
            color: #fff;
        }
        .btn-primary:hover { background: #1d4ed8; }
        .btn-outline {
            background: #fff;
            color: #334155;
            border: 1px solid #e2e8f0;
        }
        .btn-outline:hover { background: #f8fafc; border-color: #cbd5e1; }
        footer {
            text-align: center;
            padding: 32px 24px;
            color: #94a3b8;
            font-size: 0.8rem;
        }
        @media (max-width: 600px) {
            .container { grid-template-columns: 1fr; padding: 0 16px; }
            .hero h1 { font-size: 1.6rem; }
            .card { padding: 20px 24px; }
            .card-actions { flex-direction: column; }
        }
    </style>
</head>
<body>

    <header class="hero">
        <h1>医疗影像系统 · 作品集</h1>
        <p>面向区域影像云平台的前端原型设计，覆盖预约登记、报告书写、患者主索引管理及病例研讨等核心业务场景</p>
    </header>

    <div class="container">

        <!-- 卡片1：单屏书写报告 -->
        <div class="card">
            <div class="card-header">
                <div class="card-icon icon-report">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="3" width="20" height="14" rx="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg>
                </div>
                <div>
                    <div class="card-title">单屏书写报告</div>
                    <div class="card-subtitle">影像报告书写工作站</div>
                </div>
            </div>
            <div class="card-desc">
                左侧阅片 + 右侧报告编辑的单屏工作台，支持结构化模板插入、富文本编辑、报告状态流转（草稿/待审核/已驳回/已通过）、危急值上报及打印输出等全流程操作。
            </div>
            <div class="card-tags">
                <span class="tag">CT 阅片</span>
                <span class="tag">报告编辑</span>
                <span class="tag">模板管理</span>
                <span class="tag">审核流转</span>
                <span class="tag">危急值上报</span>
            </div>
            <div class="card-actions">
                <a href="单屏书写报告.html" class="btn btn-primary" target="_blank">打开预览</a>
                <a href="单屏书写报告.html" class="btn btn-outline" target="_blank">新窗口打开 ↗</a>
            </div>
        </div>

        <!-- 卡片2：患者主索引 -->
        <div class="card">
            <div class="card-header">
                <div class="card-icon icon-empi">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="4"/><path d="M4 20c0-4 4-7 8-7s8 3 8 7"/></svg>
                </div>
                <div>
                    <div class="card-title">患者主索引</div>
                    <div class="card-subtitle">EMPI 管理与跨院数据整合</div>
                </div>
            </div>
            <div class="card-desc">
                区域影像云 EMPI 管理平台，提供患者主索引列表查询、按城市/医院分组的就诊记录浏览、检查记录筛选排序，以及匹配规则配置与沙盒试算等能力。
            </div>
            <div class="card-tags">
                <span class="tag">EMPI</span>
                <span class="tag">跨院数据</span>
                <span class="tag">规则匹配</span>
                <span class="tag">沙盒试算</span>
                <span class="tag">HL7 网关</span>
            </div>
            <div class="card-actions">
                <a href="患者主索引.html" class="btn btn-primary" target="_blank">打开预览</a>
                <a href="患者主索引.html" class="btn btn-outline" target="_blank">新窗口打开 ↗</a>
            </div>
        </div>

        <!-- 卡片3：病例研讨论坛 -->
        <div class="card">
            <div class="card-header">
                <div class="card-icon icon-forum">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
                </div>
                <div>
                    <div class="card-title">病例研讨论坛</div>
                    <div class="card-subtitle">影像病例研讨管理模块</div>
                </div>
            </div>
            <div class="card-desc">
                区域内影像病例讨论社区，支持发布病例、多级评论回复、影像标注批注、权限范围控制（全区域/本院/指定范围）、收藏及知识要点总结等协作功能。
            </div>
            <div class="card-tags">
                <span class="tag">病例研讨</span>
                <span class="tag">影像标注</span>
                <span class="tag">权限控制</span>
                <span class="tag">知识总结</span>
                <span class="tag">多级评论</span>
            </div>
            <div class="card-actions">
                <a href="病例研讨论坛.html" class="btn btn-primary" target="_blank">打开预览</a>
                <a href="病例研讨论坛.html" class="btn btn-outline" target="_blank">新窗口打开 ↗</a>
            </div>
        </div>

        <!-- 卡片4：预约登记 -->
        <div class="card">
            <div class="card-header">
                <div class="card-icon icon-book">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
                </div>
                <div>
                    <div class="card-title">预约登记</div>
                    <div class="card-subtitle">智能预约登记工作台</div>
                </div>
            </div>
            <div class="card-desc">
                影像检查预约登记工作台，提供患者信息录入、检查项目管理、号源日历选择、院区设备调度，以及护士到检工作站（含生命体征记录、造影剂管理、不良反应监测）等全流程功能。
            </div>
            <div class="card-tags">
                <span class="tag">预约登记</span>
                <span class="tag">号源管理</span>
                <span class="tag">设备调度</span>
                <span class="tag">到检工作站</span>
                <span class="tag">造影剂管理</span>
            </div>
            <div class="card-actions">
                <a href="预约登记.html" class="btn btn-primary" target="_blank">打开预览</a>
                <a href="预约登记.html" class="btn btn-outline" target="_blank">新窗口打开 ↗</a>
            </div>
        </div>

    </div>

    <footer>
        医疗影像系统原型作品集 · 前端交互设计展示
    </footer>

</body>
</html>

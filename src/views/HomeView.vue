<template>
  <div class="app">
    <!-- 导航栏 -->
    <nav class="navbar">
      <div class="container">
        <div class="nav-brand">
          <h1>ABACUS</h1>
          <span class="subtitle">第一性原理计算软件包 | Ab initio Package</span>
        </div>
        <div class="nav-links">
          <a href="#home" class="nav-link">首页</a>
          <a href="#download" class="nav-link">下载</a>
          <a href="#docs" class="nav-link">文档</a>
          <div class="nav-dropdown">
            <a href="#ecosystem" class="nav-link dropdown-trigger">生态系统 <i class="fas fa-chevron-down"></i></a>
            <div class="dropdown-menu">
              <a href="#ecosystem" class="dropdown-item">软件接口</a>
              <a href="#pseudopotentials" class="dropdown-item">赝势与轨道</a>
              <a href="#tools" class="dropdown-item">在线工具</a>
              <a href="#ai-agents" class="dropdown-item">AI 智能体</a>
              <a href="#supercomputers" class="dropdown-item">超算部署</a>
            </div>
          </div>
          <div class="nav-dropdown">
            <a href="#" class="nav-link dropdown-trigger">资源 <i class="fas fa-chevron-down"></i></a>
            <div class="dropdown-menu">
              <a href="#examples" class="dropdown-item">算例展示</a>
              <a href="#publications" class="dropdown-item">学术文章</a>
              <a href="#datasets" class="dropdown-item">数据集</a>
              <a href="#channels" class="dropdown-item">官方渠道</a>
            </div>
          </div>
          <a href="#news" class="nav-link">新闻</a>
          <a href="#faq" class="nav-link highlight">常见问题</a>
          <a href="#contact" class="nav-link btn-primary">联系我们</a>
        </div>
      </div>
    </nav>

    <!-- Hero 区域 -->
    <section class="hero" id="home">
      <div class="hero-grid">
        <div class="hero-left">
          <div class="hero-tag">
            <span class="tag-dot"></span>
            <span>开源第一性原理计算平台</span>
          </div>
          <h1 class="hero-title">
            <span class="title-main">ABACUS</span>
            <span class="title-sub">原子算筹</span>
          </h1>
          <p class="hero-description">
            基于密度泛函理论，支持平面波、数值原子轨道等多种基组<br/>
            从材料模拟到量子化学，为科研提供强大计算引擎
          </p>
          <div class="hero-actions">
            <a href="#download" class="btn-hero-primary">
              <span>立即下载</span>
              <i class="fas fa-download"></i>
            </a>
            <a href="https://github.com/deepmodeling/abacus-develop" target="_blank" class="btn-hero-github">
              <i class="fab fa-github"></i>
              <span>Star on GitHub</span>
            </a>
          </div>
          <div class="hero-features">
            <div class="feature-badge">
              <i class="fas fa-bolt"></i>
              <span>高性能并行</span>
            </div>
            <div class="feature-badge">
              <i class="fas fa-cube"></i>
              <span>多基组支持</span>
            </div>
            <div class="feature-badge">
              <i class="fas fa-brain"></i>
              <span>AI集成</span>
            </div>
          </div>
        </div>
        <div class="hero-right">
          <div class="logo-container">
            <img src="../img/logo.svg" alt="ABACUS Logo" class="hero-logo">
            <div class="logo-glow"></div>
          </div>
        </div>
      </div>
    </section>

    <!-- 下载区域 -->
    <section class="download" id="download">
      <div class="container">
        <h2 class="section-title">下载 ABACUS</h2>
        <p class="section-description">多种下载渠道，选择最适合您的方式</p>
        
        <div class="download-grid">
          <div class="download-card featured">
            <div class="download-badge">推荐</div>
            <div class="download-icon">
              <i class="fab fa-github"></i>
            </div>
            <h3>GitHub (主仓库)</h3>
            <p>DeepModeling 社区维护，更新最快</p>
            <a href="https://github.com/deepmodeling/abacus-develop" target="_blank" class="btn btn-primary">
              访问 GitHub
            </a>
          </div>

          <div class="download-card">
            <div class="download-icon">
              <i class="fab fa-github"></i>
            </div>
            <h3>GitHub (镜像)</h3>
            <p>ABACUS Modeling 组织镜像仓库</p>
            <a href="https://github.com/abacusmodeling/abacus-develop" target="_blank" class="btn btn-outline">
              访问仓库
            </a>
          </div>

          <div class="download-card">
            <div class="download-icon">
              <i class="fas fa-flag"></i>
            </div>
            <h3>Gitee (国内)</h3>
            <p>国内访问速度更快的镜像</p>
            <a href="https://gitee.com/abacus_dft/abacus-develop" target="_blank" class="btn btn-outline">
              访问 Gitee
            </a>
          </div>
        </div>

        <!-- 更多安装方式 -->
        <h3 class="install-methods-title"><i class="fas fa-cogs"></i> 更多安装方式</h3>
        <div class="download-grid">
          <div class="download-card">
            <div class="download-icon">
              <i class="fas fa-cube"></i>
            </div>
            <h3>Conda 安装</h3>
            <p>通过 conda-forge 快速安装</p>
            <code class="install-code">conda install -c conda-forge abacus</code>
            <a href="https://anaconda.org/conda-forge/abacus" target="_blank" class="btn btn-outline">
              查看详情
            </a>
          </div>

          <div class="download-card">
            <div class="download-icon">
              <i class="fab fa-docker"></i>
            </div>
            <h3>Docker 镜像</h3>
            <p>开箱即用的容器化部署</p>
            <code class="install-code">docker pull ghcr.io/deepmodeling/abacus</code>
            <a href="https://github.com/deepmodeling/abacus-develop/pkgs/container/abacus" target="_blank" class="btn btn-outline">
              获取镜像
            </a>
          </div>

          <!-- <div class="download-card">
            <div class="download-icon">
              <i class="fas fa-box-open"></i>
            </div>
            <h3>DeepModeling 镜像源</h3>
            <p>官方合作的开源社区仓库</p>
            <a href="https://github.com/deepmodeling" target="_blank" class="btn btn-outline">
              访问社区
            </a>
          </div> -->
        </div>

        <div class="download-info">
          <h3><i class="fas fa-info-circle"></i> 下载说明</h3>
          <ul>
            <li><strong>稳定版本：</strong>建议生产环境使用 Release 版本</li>
            <li><strong>开发版本：</strong>包含最新功能，适合开发者和测试用户</li>
            <li><strong>ZIP下载：</strong>可直接下载代码压缩包，无需Git工具</li>
            <li><strong>Conda安装：</strong>推荐使用 conda-forge 渠道，便于依赖管理</li>
            <li><strong>Docker部署：</strong>适合快速部署和容器化环境使用</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- 文档资料 -->
    <section class="documentation" id="docs">
      <div class="container">
        <h2 class="section-title">文档资料</h2>
        <p class="section-description">全面的学习资源，从理论到实践</p>
        
        <div class="doc-categories">
          <!-- DFT理论 -->
          <div class="doc-category">
            <h3 class="doc-category-title">📖 DFT理论基础</h3>
            <div class="doc-list">
              <a href="#" class="doc-link-item">
                <span>密度泛函理论入门</span>
                <span class="arrow">→</span>
              </a>
              <a href="#" class="doc-link-item">
                <span>第一性原理计算方法</span>
                <span class="arrow">→</span>
              </a>
            </div>
          </div>

          <!-- 使用者文档 -->
          <div class="doc-category featured">
            <h3 class="doc-category-title">👤 使用者文档</h3>
            <div class="doc-list">
              <a href="https://abacus.deepmodeling.com/" target="_blank" class="doc-link-item">
                <span>📚 官方在线文档</span>
                <span class="arrow">→</span>
              </a>
              <a href="https://gitee.com/mcresearch/abacus-user-guide" target="_blank" class="doc-link-item">
                <span>📘 用户手册 (Gitee)</span>
                <span class="arrow">→</span>
              </a>
              <a href="#" class="doc-link-item">
                <span>💡 应用示例库</span>
                <span class="arrow">→</span>
              </a>
              <a href="#" class="doc-link-item">
                <span>🎥 视频教程</span>
                <span class="arrow">→</span>
              </a>
            </div>
          </div>

          <!-- 开发者文档 -->
          <div class="doc-category">
            <h3 class="doc-category-title">💻 开发者文档</h3>
            <div class="doc-list">
              <a href="#" class="doc-link-item">
                <span>开发者指南 v0.2</span>
                <span class="arrow">→</span>
              </a>
              <a href="#" class="doc-link-item">
                <span>API 参考文档</span>
                <span class="arrow">→</span>
              </a>
              <a href="https://github.com/deepmodeling/abacus-develop" target="_blank" class="doc-link-item">
                <span>贡献指南</span>
                <span class="arrow">→</span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ABACUS 生态系统 -->
    <section class="ecosystem" id="ecosystem">
      <div class="container">
        <h2 class="section-title">ABACUS 生态系统</h2>
        <p class="section-description">丰富的软件接口与集成工具</p>
        
        <!-- 核心工具 -->
        <div class="ecosystem-category">
          <h3 class="ecosystem-title">🔬 核心分析工具</h3>
          <div class="ecosystem-grid">
            <a href="#" target="_blank" class="ecosystem-card">
              <h4>PYATB</h4>
              <p>Python紧束缚模拟包</p>
              <span class="status online">在线</span>
            </a>

            <a href="#" target="_blank" class="ecosystem-card">
              <h4>PyKappa</h4>
              <p>热输运性质计算</p>
              <span class="status">工具</span>
            </a>

            <a href="#" target="_blank" class="ecosystem-card">
              <h4>LibRI</h4>
              <p>张量操作库</p>
              <span class="status">库</span>
            </a>
          </div>
        </div>

        <!-- 软件接口 -->
        <div class="ecosystem-category">
          <h3 class="ecosystem-title">🔗 软件接口</h3>
          <div class="ecosystem-grid">
            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>Phonopy</h4>
              <p>声子计算（谐振与准谐振）</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>Wannier90</h4>
              <p>最大局域化Wannier函数</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="http://atomkit.cn/" target="_blank" class="ecosystem-card">
              <h4>AtomKit</h4>
              <p>原子模拟工具包</p>
              <span class="status online">Web界面</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>ASE</h4>
              <p>原子模拟环境</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://github.com/QuantumMisaka/ATST-Tools" target="_blank" class="ecosystem-card">
              <h4>ATST-Tools</h4>
              <p>后处理工具集</p>
              <span class="status">GitHub</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>Hefei-NAMD</h4>
              <p>非绝热分子动力学</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>ShengBTE</h4>
              <p>声子玻尔兹曼输运方程求解器</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>CANDELA</h4>
              <p>MD轨迹分析工具</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card">
              <h4>TB2J</h4>
              <p>磁晶体磁相互作用自动计算</p>
              <span class="status online">在线文档</span>
            </a>
          </div>
        </div>

        <!-- 机器学习工具 -->
        <div class="ecosystem-category">
          <h3 class="ecosystem-title">🤖 机器学习集成</h3>
          <div class="ecosystem-grid">
            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card featured">
              <h4>DeePKS</h4>
              <p>机器学习辅助密度泛函模型</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card featured">
              <h4>DP-GEN</h4>
              <p>深度学习势函数生成包</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://abacus.deepmodeling.com/" target="_blank" class="ecosystem-card featured">
              <h4>DeepH</h4>
              <p>机器学习预测哈密顿量</p>
              <span class="status online">在线文档</span>
            </a>

            <a href="https://github.com/QuantumLab-ZY/HamGNN" target="_blank" class="ecosystem-card featured">
              <h4>HamGNN</h4>
              <p>E(3)等变图神经网络预测哈密顿量</p>
              <span class="status">GitHub</span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- 赝势与轨道 -->
    <section class="pseudopotentials" id="pseudopotentials">
      <div class="container">
        <h2 class="section-title">赝势与轨道文件</h2>
        <p class="section-description">高质量的赝势和数值原子轨道库</p>
        
        <div class="pseudo-grid">
          <div class="pseudo-card">
            <div class="pseudo-header">
              <h3>SG15</h3>
              <span class="pseudo-badge">ONCV</span>
            </div>
            <p>Optimized Norm-Conserving Vanderbilt 赝势</p>
            <div class="pseudo-links">
              <a href="http://www.quantum-simulation.org/potentials/sg15_oncv/" target="_blank" class="btn btn-small btn-outline">
                📥 下载赝势
              </a>
              <a href="#" class="btn btn-small btn-outline">
                🔧 下载轨道
              </a>
            </div>
          </div>

          <div class="pseudo-card">
            <div class="pseudo-header">
              <h3>DOJO</h3>
              <span class="pseudo-badge">精确</span>
            </div>
            <p>高精度赝势数据库</p>
            <div class="pseudo-links">
              <a href="https://www.pseudo-dojo.org/" target="_blank" class="btn btn-small btn-outline">
                📥 下载赝势
              </a>
              <a href="#" class="btn btn-small btn-outline">
                🔧 下载轨道
              </a>
            </div>
          </div>

          <div class="pseudo-card featured">
            <div class="pseudo-header">
              <h3>APNS</h3>
              <span class="pseudo-badge">推荐</span>
            </div>
            <p>ABACUS专用赝势与轨道库</p>
            <div class="pseudo-links">
              <a href="https://www.aissquare.com/datasets/detail?pageType=datasets&name=ABACUS-APNS-PPORBs-v1&id=326" target="_blank" class="btn btn-small btn-primary">
                📥 下载完整包
              </a>
            </div>
          </div>

          <div class="pseudo-card">
            <div class="pseudo-header">
              <h3>自生成工具</h3>
              <span class="pseudo-badge">高级</span>
            </div>
            <p>自定义赝势和轨道生成</p>
            <div class="pseudo-links">
              <a href="#" class="btn btn-small btn-outline">
                🔧 查看教程
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 在线工具集 -->
    <section class="online-tools" id="tools">
      <div class="container">
        <h2 class="section-title">在线工具集</h2>
        <p class="section-description">无需安装，在线使用各种便捷工具</p>
        
        <div class="tools-grid">
          <div class="tool-card">
            <div class="tool-icon">🔄</div>
            <h3>格式转换</h3>
            <p>输入文件格式在线转换工具</p>
            <a href="#" class="tool-link">使用工具 →</a>
          </div>

          <div class="tool-card">
            <div class="tool-icon">👁️</div>
            <h3>结构可视化</h3>
            <p>在线查看原子结构</p>
            <a href="#" class="tool-link">打开工具 →</a>
          </div>

          <div class="tool-card">
            <div class="tool-icon">📊</div>
            <h3>电荷密度可视化</h3>
            <p>电荷密度分布展示</p>
            <a href="#" class="tool-link">打开工具 →</a>
          </div>

          <div class="tool-card">
            <div class="tool-icon">🌊</div>
            <h3>波函数可视化</h3>
            <p>波函数三维展示</p>
            <a href="#" class="tool-link">打开工具 →</a>
          </div>
        </div>

        <div class="download-tools">
          <h3>📦 可下载工具</h3>
          <div class="download-tools-list">
            <div class="download-tool-item">
              <span class="tool-name">原子轨道基组生成器</span>
              <a href="#" class="btn btn-small btn-outline">下载</a>
            </div>
            <div class="download-tool-item">
              <span class="tool-name">ABACUS Test Suite</span>
              <a href="#" class="btn btn-small btn-outline">下载</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 算例展示 -->
    <section class="examples" id="examples">
      <div class="container">
        <h2 class="section-title">算例展示</h2>
        <p class="section-description">完整的计算示例，包含输入输出和可视化结果</p>
        
        <div class="example-grid">
          <div class="example-card">
            <div class="example-image">
              <div class="placeholder-image">🔬</div>
            </div>
            <h3>硅能带计算</h3>
            <p>完整的能带结构计算示例</p>
            <div class="example-tags">
              <span class="tag">能带</span>
              <span class="tag">半导体</span>
            </div>
            <a href="#" class="btn btn-small btn-outline">查看详情</a>
          </div>

          <div class="example-card">
            <div class="example-image">
              <div class="placeholder-image">⚛️</div>
            </div>
            <h3>石墨烯结构优化</h3>
            <p>二维材料结构优化流程</p>
            <div class="example-tags">
              <span class="tag">优化</span>
              <span class="tag">2D材料</span>
            </div>
            <a href="#" class="btn btn-small btn-outline">查看详情</a>
          </div>

          <div class="example-card">
            <div class="example-image">
              <div class="placeholder-image">💎</div>
            </div>
            <h3>金属态密度</h3>
            <p>过渡金属态密度分析</p>
            <div class="example-tags">
              <span class="tag">DOS</span>
              <span class="tag">金属</span>
            </div>
            <a href="#" class="btn btn-small btn-outline">查看详情</a>
          </div>
        </div>
      </div>
    </section>

    <!-- AI 智能体 -->
    <section class="ai-agents" id="ai-agents">
      <div class="container">
        <h2 class="section-title">AI 智能体</h2>
        <p class="section-description">通过AI助手体验 ABACUS 计算</p>
        
        <div class="ai-agent-grid">
          <div class="ai-agent-card featured">
            <div class="agent-badge">开源</div>
            <div class="agent-icon">🤖</div>
            <h3>ABACUS Agent Tools</h3>
            <p>开源的 ABACUS 智能体工具库</p>
            <div class="agent-features">
              <span>✓ 完全开源</span>
              <span>✓ 可自部署</span>
              <span>✓ Markdown知识库</span>
            </div>
            <a href="#" target="_blank" class="btn btn-primary">访问仓库</a>
          </div>

          <div class="ai-agent-card">
            <div class="agent-badge">支持 v3.10.0 LTS</div>
            <div class="agent-icon">🚀</div>
            <h3>GaliLeo 智能体</h3>
            <p>Sidereus AI平台的ABACUS智能体</p>
            <div class="agent-features">
              <span>✓ 在线使用</span>
              <span>✓ LTS版本</span>
            </div>
            <a href="https://sidereus-ai.com/" target="_blank" class="btn btn-outline">体验使用</a>
          </div>

          <div class="ai-agent-card">
            <div class="agent-badge">支持 v3.10.0 LTS</div>
            <div class="agent-icon">🔬</div>
            <h3>MatMaster 智能体</h3>
            <p>Bohrium平台的材料计算助手</p>
            <div class="agent-features">
              <span>✓ 在线使用</span>
              <span>✓ LTS版本</span>
            </div>
            <a href="https://scimaster.bohrium.com/matmaster/" target="_blank" class="btn btn-outline">体验使用</a>
          </div>
        </div>
      </div>
    </section>

    <!-- 超算部署 -->
    <section class="supercomputers" id="supercomputers">
      <div class="container">
        <h2 class="section-title">已部署超算中心</h2>
        <p class="section-description">ABACUS 已在多个超算中心部署并可直接使用</p>
        
        <div class="supercomputer-grid">
          <div class="supercomputer-card featured">
            <div class="sc-icon">🖥️</div>
            <h3>超算互联网</h3>
            <p>中国超算互联网平台</p>
            <div class="sc-info">
              <a href="https://www.scnet.cn" target="_blank" class="btn btn-small btn-primary">访问平台</a>
            </div>
          </div>

          <div class="supercomputer-card">
            <div class="sc-icon">🏫</div>
            <h3>中科大超算中心</h3>
            <p>USTC HPC</p>
            <div class="sc-info">
              <span class="sc-badge">使用方法</span>
              <span class="sc-badge">提交脚本</span>
            </div>
          </div>

          <div class="supercomputer-card">
            <div class="sc-icon">🏫</div>
            <h3>北京大学超算</h3>
            <p>PKU HPC</p>
            <div class="sc-info">
              <span class="sc-badge">使用方法</span>
              <span class="sc-badge">提交脚本</span>
            </div>
          </div>

          <div class="supercomputer-card">
            <div class="sc-icon">☁️</div>
            <h3>Bohrium 平台</h3>
            <p>云端超算平台</p>
            <div class="sc-info">
              <a href="#" target="_blank" class="btn btn-small btn-outline">了解更多</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 学术文章 -->
    <section class="publications" id="publications">
      <div class="container">
        <h2 class="section-title">学术文章</h2>
        <p class="section-description">ABACUS 相关研究成果</p>
        
        <div class="publication-categories">
          <div class="publication-category">
            <h3>📄 ABACUS 团队发表</h3>
            <div class="publication-tabs">
              <button class="pub-tab active">算法开发</button>
              <button class="pub-tab">应用研究</button>
              <button class="pub-tab">全部文章</button>
            </div>
            <div class="publication-list">
              <div class="publication-item">
                <div class="pub-info">
                  <h4>文章标题示例</h4>
                  <p class="pub-meta">期刊名称 | 2024 | DOI: 10.xxxx/xxxxx</p>
                  <div class="pub-links">
                    <a href="#" target="_blank">期刊链接</a>
                    <a href="#" target="_blank">arXiv</a>
                    <a href="#" target="_blank">原始数据</a>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="publication-category">
            <h3>🌟 用户使用 ABACUS 的文章</h3>
            <p class="pub-note">展示全球用户使用 ABACUS 发表的优秀研究成果</p>
            <div class="publication-highlight">
              <p>📚 <strong>100+</strong> 篇学术论文引用 ABACUS</p>
              <a href="#" class="btn btn-outline">查看完整列表</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 数据集 -->
    <section class="datasets" id="datasets">
      <div class="container">
        <h2 class="section-title">ABACUS 构造的数据集</h2>
        <p class="section-description">高质量的计算数据集，支持机器学习研究</p>
        
        <div class="dataset-grid">
          <a href="#" target="_blank" class="dataset-card">
            <div class="dataset-icon">📊</div>
            <h3>Atomly</h3>
            <p>大规模原子数据集</p>
            <div class="dataset-stats">
              <span>🔢 数据量大</span>
              <span>✓ 高质量</span>
            </div>
          </a>

          <a href="https://www.aissquare.com/" target="_blank" class="dataset-card">
            <div class="dataset-icon">🗄️</div>
            <h3>AIS Square</h3>
            <p>AI for Science 数据广场</p>
            <div class="dataset-stats">
              <span>🌐 开放平台</span>
              <span>✓ 多种数据集</span>
            </div>
          </a>
        </div>
      </div>
    </section>

    <!-- 新闻动态 -->
    <section class="news" id="news">
      <div class="container">
        <h2 class="section-title">新闻动态</h2>
        <p class="section-description">关注 ABACUS 最新进展</p>
        
        <div class="news-grid">
          <div class="news-card highlight">
            <div class="news-badge">大版本发布</div>
            <h3>ABACUS 3.10.0 LTS 版本发布</h3>
            <p>长期支持版本，包含重大功能更新和性能优化</p>
            <div class="news-meta">2024年11月</div>
          </div>

          <div class="news-card">
            <div class="news-badge">研究进展</div>
            <h3>最新研究成果</h3>
            <p>ABACUS在材料计算领域的最新应用和突破</p>
            <div class="news-meta">持续更新</div>
          </div>

          <div class="news-card">
            <div class="news-badge">开发者大会</div>
            <h3>ABACUS 开发者大会</h3>
            <p>汇聚开发者与用户，分享经验与技术</p>
            <div class="news-meta">年度活动</div>
          </div>
        </div>
      </div>
    </section>

    <!-- 官方渠道 -->
    <section class="channels" id="channels">
      <div class="container">
        <h2 class="section-title">官方渠道</h2>
        <p class="section-description">通过多种方式联系我们，获取最新动态</p>
        
        <div class="channels-grid">
          <a href="#" class="channel-card">
            <div class="channel-icon"><i class="fab fa-weixin"></i></div>
            <h3>微信公众号</h3>
            <p>关注获取最新资讯</p>
          </a>

          <a href="#" class="channel-card">
            <div class="channel-icon"><i class="fas fa-envelope"></i></div>
            <h3>邮件列表</h3>
            <p>订阅开发者动态</p>
          </a>

          <a href="#" class="channel-card">
            <div class="channel-icon"><i class="fas fa-comments"></i></div>
            <h3>官方论坛</h3>
            <p>技术交流与讨论</p>
          </a>

          <a href="#" class="channel-card">
            <div class="channel-icon"><i class="fab fa-zhihu"></i></div>
            <h3>知乎</h3>
            <p>深度技术文章</p>
          </a>

          <a href="#" class="channel-card">
            <div class="channel-icon"><i class="fab fa-bilibili"></i></div>
            <h3>Bilibili</h3>
            <p>视频教程与讲座</p>
          </a>
        </div>
      </div>
    </section>

    <!-- FAQ 区域 -->
    <section class="faq-highlight" id="faq">
      <div class="container">
        <div class="faq-banner">
          <div class="faq-icon">
            <i class="fas fa-circle-question"></i>
          </div>
          <div class="faq-content">
            <h2 class="faq-title">常见问题解答 (FAQ)</h2>
            <p class="faq-subtitle">快速找到您需要的答案</p>
          </div>
        </div>
        
        <div class="faq-grid">
          <div class="faq-category">
            <h3><i class="fas fa-rocket"></i> 快速开始</h3>
            <div class="faq-item">
              <div class="faq-question">如何安装 ABACUS？</div>
              <div class="faq-answer">请参考<a href="https://abacus.deepmodeling.com/en/latest/quick_start/easy_install.html" target="_blank">安装指南</a>，支持源码编译和容器安装两种方式。</div>
            </div>
            <div class="faq-item">
              <div class="faq-question">需要什么样的计算资源？</div>
              <div class="faq-answer">ABACUS支持从单核到大规模并行计算，可在个人电脑、工作站或超算上运行。</div>
            </div>
          </div>

          <div class="faq-category">
            <h3><i class="fas fa-book-open"></i> 使用问题</h3>
            <div class="faq-item">
              <div class="faq-question">支持哪些计算类型？</div>
              <div class="faq-answer">支持结构优化、分子动力学、能带计算、态密度分析、声子谱计算等多种功能。</div>
            </div>
            <div class="faq-item">
              <div class="faq-question">如何获取赝势和轨道文件？</div>
              <div class="faq-answer">可从<a href="#pseudopotentials">赝势库</a>下载SG15、DOJO、APNS等多种赝势和轨道文件。</div>
            </div>
          </div>

          <div class="faq-category">
            <h3><i class="fas fa-wrench"></i> 技术支持</h3>
            <div class="faq-item">
              <div class="faq-question">遇到问题如何寻求帮助？</div>
              <div class="faq-answer">可通过GitHub Issues、官方论坛、微信公众号或邮件列表获取技术支持。</div>
            </div>
            <div class="faq-item">
              <div class="faq-question">如何参与开发？</div>
              <div class="faq-answer">欢迎在GitHub上提交Pull Request，详见<a href="https://github.com/deepmodeling/abacus-develop" target="_blank">开发者文档</a>。</div>
            </div>
          </div>

          <div class="faq-category">
            <h3><i class="fas fa-globe"></i> 资源获取</h3>
            <div class="faq-item">
              <div class="faq-question">在哪里找学习资料？</div>
              <div class="faq-answer">提供DFT理论教程、用户手册、开发者文档、视频教程等多种学习资源。</div>
            </div>
            <div class="faq-item">
              <div class="faq-question">有算例可以参考吗？</div>
              <div class="faq-answer">提供完整的算例库，包含输入输出文件、结构图、能带图等详细资料。</div>
            </div>
          </div>
        </div>

        <div class="faq-cta">
          <p>没有找到答案？</p>
          <a href="#contact" class="btn btn-large btn-primary">联系我们获取帮助</a>
        </div>
      </div>
    </section>

    <!-- 联系我们 -->
    <section class="contact" id="contact">
      <div class="container">
        <h2 class="section-title">联系我们</h2>
        <p class="section-description">欢迎联系 ABACUS 团队</p>
        
        <div class="contact-grid">
          <div class="contact-card">
            <div class="contact-icon">💬</div>
            <h3>技术支持</h3>
            <p>遇到问题？查看FAQ或联系我们</p>
            <a href="#faq" class="btn btn-outline">查看FAQ</a>
          </div>

          <div class="contact-card">
            <div class="contact-icon">🐛</div>
            <h3>Bug 反馈</h3>
            <p>在 GitHub 上提交 Issue</p>
            <a href="https://github.com/deepmodeling/abacus-develop/issues" target="_blank" class="btn btn-outline">提交Issue</a>
          </div>

          <div class="contact-card">
            <div class="contact-icon">🤝</div>
            <h3>参与贡献</h3>
            <p>欢迎提交代码和文档</p>
            <a href="https://github.com/deepmodeling/abacus-develop" target="_blank" class="btn btn-outline">贡献代码</a>
          </div>
        </div>
      </div>
    </section>

    <!-- 页脚 -->
    <footer class="footer">
      <div class="container">
        <div class="footer-grid">
          <div class="footer-section">
            <h3>ABACUS</h3>
            <p>开源第一性原理计算软件包</p>
             <p class="footer-contributors">联合开发：中国科学技术大学 · 中科院物理所 · 北京大学 · AISI北京 · 合肥人工智能研究院</p>
          </div>
          <div class="footer-section">
            <h4>快速链接</h4>
            <a href="#download">下载</a>
            <a href="#docs">文档</a>
            <a href="#ecosystem">生态系统</a>
            <a href="#faq">常见问题</a>
          </div>
          <div class="footer-section">
            <h4>资源</h4>
            <a href="https://abacus.deepmodeling.com/" target="_blank">在线文档</a>
            <a href="https://github.com/deepmodeling/abacus-develop" target="_blank">GitHub</a>
            <a href="https://gitee.com/abacus_dft/abacus-develop" target="_blank">Gitee</a>
          </div>
          <div class="footer-section">
            <h4>社区</h4>
            <a href="#">微信公众号</a>
            <a href="#">官方论坛</a>
            <a href="#">知乎</a>
            <a href="#">Bilibili</a>
          </div>
        </div>
        <div class="footer-bottom">
          <p>&copy; 2025 ABACUS. All rights reserved. | 由中科院量子信息重点实验室何力新教授团队主导开发</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  mounted() {
    // 平滑滚动
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

    // 导航栏滚动效果
    window.addEventListener('scroll', () => {
      const navbar = document.querySelector('.navbar');
      if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
      } else {
        navbar.classList.remove('scrolled');
      }
    });

    // FAQ 项目展开/折叠
    document.querySelectorAll('.faq-question').forEach(question => {
      question.addEventListener('click', function() {
        const answer = this.nextElementSibling;
        const isOpen = answer.style.display === 'block';
        
        // 关闭所有答案
        document.querySelectorAll('.faq-answer').forEach(a => {
          a.style.display = 'none';
        });
        
        // 打开当前答案
        if (!isOpen) {
          answer.style.display = 'block';
        }
      });
    });
  }
}
</script>

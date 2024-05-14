<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div align="center" dir="auto">
<a target="_blank" rel="noopener noreferrer" href="/Alibaba-NLP/EcomGPT/blob/main/IMG/logo.jpg"><img src="/Alibaba-NLP/EcomGPT/raw/main/IMG/logo.jpg" width="55%" style="max-width: 100%;"></a>
</div>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">一种遵循指令的电子商务大型语言模型</font></font></h1><a id="user-content-an-instruction-following-large-language-model-for-e-commerce" class="anchor" aria-label="永久链接：一种遵循指令的电子商务大型语言模型" href="#an-instruction-following-large-language-model-for-e-commerce"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/5bdc188749a8bae8bc103cf5001d752b0291e66ecef49296b419068147516d2c/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f76657273696f6e2d312e302e302d626c7565"><img src="https://camo.githubusercontent.com/5bdc188749a8bae8bc103cf5001d752b0291e66ecef49296b419068147516d2c/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f76657273696f6e2d312e302e302d626c7565" alt="" data-canonical-src="https://img.shields.io/badge/version-1.0.0-blue" style="max-width: 100%;"></a><a href="https://pytorch.org/" rel="nofollow"><img src="https://camo.githubusercontent.com/d665e458b563f5eacc8d677897770efe0c1a0b13b7bffe283f74a3c9ce87dea5/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5079546f7263682d2532334545344332432e7376673f65266c6f676f3d5079546f726368266c6f676f436f6c6f723d7768697465" alt="火炬" data-canonical-src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?e&amp;logo=PyTorch&amp;logoColor=white" style="max-width: 100%;"></a><a href="https://arxiv.org/pdf/2308.06966.pdf" rel="nofollow"><img src="https://camo.githubusercontent.com/f96ce5818f4f3bdbc78f9c493e641b126067e630c1770bc9aeb294621b6cb7b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f61727869762d323330382e30363936362d726564" alt="arxiv 徽章" data-canonical-src="https://img.shields.io/badge/arxiv-2308.06966-red" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">EcomGPT的存储库</font></font><a href="https://arxiv.org/pdf/2308.06966" rel="nofollow"><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：使用电子商务任务链任务对大型语言模型进行指令调整</font></font></em></a></p>
<ul dir="auto">
<li><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们提出了第一个电商指令数据集EcomInstruct，共有250万条指令数据</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">EcomInstruct通过利用电商基本数据类型</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（例如产品信息、用户评论）</font><font style="vertical-align: inherit;">构建原子任务来扩展数据规模和任务多样性。</font><font style="vertical-align: inherit;">原子任务被定义为隐式参与解决最终任务的中间任务，我们也将其称为任务链任务。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们通过使用 EcomInstruct 训练骨干模型 BLOOMZ 来开发 EcomGPT。</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">受益于从 Chain-of-Task 任务中获得的基本语义理解能力，EcomGPT 表现出了出色的零样本泛化能力。</font></font></strong></li>
</ul>
<div align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer" href="/Alibaba-NLP/EcomGPT/blob/main/IMG/method.jpg"><img src="/Alibaba-NLP/EcomGPT/raw/main/IMG/method.jpg" width="60%" height="auto" style="max-width: 100%;"></a>
</div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">💡 性能</font></font></h2><a id="user-content--perfomance" class="anchor" aria-label="永久链接：💡性能" href="#-perfomance"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们使用 12 个电子商务保留的数据集对 EcomGPT 和 ChatGPT 进行人工评估。 EcomGPT 在 12 个数据集上优于或并列 ChatGPT。</font></font></p>
<div align="center" dir="auto">
<a target="_blank" rel="noopener noreferrer" href="/Alibaba-NLP/EcomGPT/blob/main/IMG/performance.jpg"><img src="/Alibaba-NLP/EcomGPT/raw/main/IMG/performance.jpg" width="300" style="max-width: 100%;"></a>
</div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🛠 依赖关系</font></font></h2><a id="user-content--dependencies" class="anchor" aria-label="永久链接：🛠 依赖关系" href="#-dependencies"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>pip install -r requirement.txt</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="pip install -r requirement.txt" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">细节</font></font></h4><a id="user-content-details" class="anchor" aria-label="永久链接：详细信息" href="#details"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Python (&gt;= 3.7)</font></font></li>
<li><a href="http://pytorch.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">PyTorch</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> (&gt;= 2.0.0)</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">麻木</font></font></li>
<li><a href="http://huggingface.co/transformers/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">变形金刚</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">(&gt;= 4.27.4)</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">塞克瓦尔</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胭脂</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">💻 型号</font></font></h2><a id="user-content--model" class="anchor" aria-label="永久链接：💻模型" href="#-model"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">EcomGPT (7b1) 可从</font></font><a href="https://www.modelscope.cn/models/damo/nlp_ecomgpt_multilingual-7B-ecom/summary" rel="nofollow"><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ModelScope</font></font></em></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">获取。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">📚 数据集（EcomInstruct）</font></font></h2><a id="user-content--dataset-ecominstruct" class="anchor" aria-label="永久链接：📚数据集（EcomInstruct）" href="#-dataset-ecominstruct"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们首先开源了 12 个评估数据集。为了保证评估效率，每个评估数据集仅采样 500 个实例。</font></font></p>
<table>
<thead>
<tr>
<th align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据集</font></font></th>
<th align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">郎.</font></font></th>
<th align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">任务</font></font></th>
<th align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">公制</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">联想</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CN</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">命名实体识别</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">联想</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CN</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实体跨度检测</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">红迪网</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CN</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提取式质量保证</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ABSA</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CN</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">回顾主题分类</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">梅帕夫</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">属性值识别</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">梅帕夫</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">属性值检测</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多重心肺复苏</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">产品选择</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多重心肺复苏</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">产品对齐</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开放BG</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">标题属性匹配</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开放BG</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">细粒度产品分类</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开放BG</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">粗粒度产品分类</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">F1，胭脂</font></font></td>
</tr>
<tr>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开放BG</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ZH</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">标题生成</font></font></td>
<td align="left"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">胭脂</font></font></td>
</tr>
</tbody>
</table>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据集文件</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">满足以下文件层次结构</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>.
├── [Dataset Name]
│   └── tasks
│       └── [task name]
│           ├── meta-info.json
│           └── test.json
...
└── Reddit_QA
    └── tasks
        └── EN-Reddit_QA-Extract-Extract_QA
            ├── meta-info.json
            └── test.json
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value=".
├── [Dataset Name]
│   └── tasks
│       └── [task name]
│           ├── meta-info.json
│           └── test.json
...
└── Reddit_QA
    └── tasks
        └── EN-Reddit_QA-Extract-Extract_QA
            ├── meta-info.json
            └── test.json" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🔍评价</font></font></h2><a id="user-content--evaluation" class="anchor" aria-label="永久链接：🔍评价" href="#-evaluation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可以使用以下命令评估EcomGPT的性能：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python eval.py -tf ./test_tasks.txt -m [model name or path] -sn [result file name] -bdd [base dataset dir]</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python eval.py -tf ./test_tasks.txt -m [model name or path] -sn [result file name] -bdd [base dataset dir]" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🔥 待办事项</font></font></h2><a id="user-content--todo" class="anchor" aria-label="永久链接：🔥 TODO" href="#-todo"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">EcomGPT 的开源权重 ✅</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">📄 引文</font></font></h2><a id="user-content--citation" class="anchor" aria-label="永久链接：📄 引文" href="#-citation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您发现这项工作有用，请考虑给这个存储库一颗星并引用我们的论文，如下所示：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre lang="bigquery" class="notranslate"><code>@article{li2023ecomgpt,
  title={EcomGPT: Instruction-tuning Large Language Models with Chain-of-Task Tasks for E-commerce},
  author={Li, Yangning and Ma, Shirong and Wang, Xiaobin and Huang, Shen and Jiang, Chengyue and Zheng, Hai-Tao and Xie, Pengjun and Huang, Fei and Jiang, Yong},
  journal={arXiv preprint arXiv:2308.06966},
  year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@article{li2023ecomgpt,
  title={EcomGPT: Instruction-tuning Large Language Models with Chain-of-Task Tasks for E-commerce},
  author={Li, Yangning and Ma, Shirong and Wang, Xiaobin and Huang, Shen and Jiang, Chengyue and Zheng, Hai-Tao and Xie, Pengjun and Huang, Fei and Jiang, Yong},
  journal={arXiv preprint arXiv:2308.06966},
  year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</article></div>

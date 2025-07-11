> **原文链接**: https://mp.weixin.qq.com/s?__biz=MjM5OTk4MDE2MA==&mid=2655284952&idx=1&sn=fcdc42a0a90e93fd49400e236d037a62

#  CISA & NSA：内存安全语言：减少现代软件开发中的漏洞  
原创 计算机与网络安全  计算机与网络安全   2025-06-26 23:57  
  
这份由美国国家安全局（NSA）和网络安全与基础设施安全局（CISA）联合发布的报告，强调了采用内存安全语言（Memory Safe Languages, MSLs）对于减少现代软件开发中漏洞、特别是内存安全漏洞的关键作用。报告指出，内存安全漏洞（如缓冲区溢出、释放后使用、数据竞争等）是导致大量安全事件（如Heartbleed、BadAlloc）的根本原因，在主流软件漏洞（如微软CVE、安卓漏洞）中占比极高，对国家安全和关键基础设施构成严重威胁。  
  
内存安全语言（如Ada, C#, Go, Java, Python, Rust, Swift等）通过在语言层面内置安全机制（如边界检查、自动内存管理/严格所有权模型、数据竞争预防），从根本上防止了这些漏洞的产生。相较于非MSL（如C/C++）依赖开发者遵循安全编码规范和事后分析工具，MSLs将安全负担从开发者转移到语言和开发环境本身，实现了“设计安全”（Secure by Design），能更有效地消除整类的内存安全漏洞。  
  
报告承认采用MSLs存在挑战，特别是对于拥有大型遗留代码库或关键任务系统的组织。挑战包括选择合适的语言（需权衡性能、并发性、学习曲线、生态成熟度、现有系统集成）、管理依赖项、处理紧耦合代码、潜在的运行时性能开销以及团队技能培训。报告强调，采用MSLs并不要求全面重写现有系统。Android的成功案例展示了优先在新代码中使用MSLs（Rust和Java），并通过明确定义的API与遗留代码互操作，可以显著降低内存安全漏洞比例（从76%降至24%），这是一种实用且高效的战略。  
  
报告提出了分阶段采用的策略：优先在新项目和功能开发中使用MSLs；对于现有系统，识别高风险组件（如网络服务、文件解析器）进行针对性重写，并将代码库模块化以便逐步替换。组织在采用过程中应制定内存安全路线图，投资于开发者培训（将内存安全作为核心内容）、工具链和必要的重构，并与安全最佳实践（如NIST SSDF）及行业标准保持一致。即使暂时无法采用MSLs，非MSL项目也可以通过启用边界检查、避免不安全函数、使用智能指针、优化编译器选项及静态/动态分析来增强安全性。  
  
报告指出学术界、美国政府（如NSF Safe-OSE, DARPA TRACTOR/V-SPELLS/SafeDocs项目）和产业界（如OpenSSF, Prossimo项目）在推动MSL意识、教育、工具发展和需求创造方面扮演着重要角色。同时，报告也提出了未来需要研究的开放性问题，包括不同场景下的MSL选择、资源受限环境中的挑战、非MSL的增强方案、培训资源完善、工具链成熟度、生态系统发展、软件供应链安全整合以及客户在推动安全需求中的作用等。  
  
结论部分重申，内存漏洞构成重大风险，MSLs提供了最全面的缓解方案。战略性采用MSLs是对安全软件未来的投资，通过制定路线图和引领最佳实践，组织能显著提升软件韧性，塑造更安全的数字环境。报告最后提供了NSA和CISA的联系方式以供反馈和报告相关事件。  
  
完整文件（中英文）已上传至星球。  
  
  
**扫码加入知识星球****：**  
**网络安全攻防（HVV）**  
  
**下载本篇和全套资料**  
  
****  
![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/VcRPEU1K2ocrickwS8jlJmx9dm99x7cetyLS8ib43IBlZ9GpKnpibU4QV0ictAFUD0sudSt5FvXkqhPcfWSU1DgOXA/640?wx_fmt=jpeg "")  

```


```

  
**|**  
 -  
  

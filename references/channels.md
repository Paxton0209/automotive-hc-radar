# 车企设计岗官方招聘渠道清单

监测扫描的数据源。按公司分类组织,每家标注:校招/实习入口、社招入口、招聘系统、公众号、检测提示。

**使用原则:** 优先访问官方入口判断开岗;大量招聘站是 JS 动态渲染,直接抓取看不到岗位列表时,按 [detection.md](detection.md) 的兜底搜索策略处理,不要空手放弃。标注"未验证"的 URL 是调研时最有把握的地址,访问失败时直接走兜底搜索。

**清单维护:** 部分公司(广汽、丰田、哈曼等)校招域名按届次更换(如 gacgroup2026 → gacgroup2027)。遇到 404 时,先按同样的命名规律猜下一届域名,再搜"公司名 + 届次 + 校园招聘"找新入口。

---

## 一 · OEM — 新能源/新势力

| 公司 | 校招/实习入口 | 社招入口 | 系统 | 公众号 | 检测提示 |
|---|---|---|---|---|---|
| 蔚来 NIO | https://campus.nio.com/ (含实习专区) | https://nio.jobs.feishu.cn/ | 自建+飞书招聘 | 蔚来招聘 | 岗位 JS 加载,静态抓不到列表 |
| 理想汽车 | https://www.lixiang.com/employ/campus.html | https://www.lixiang.com/job/list.html | 自建+飞书招聘 | 理想汽车招聘 | li.jobs.feishu.cn 直接访问 404,从官网跳转;岗位详情页 URL 形如 lixiang.com/employ/detail/xxxx.html |
| 小鹏汽车 | https://xiaopeng.jobs.feishu.cn/campus | https://xiaopeng.jobs.feishu.cn/ | 飞书招聘 | 小鹏汽车招聘 | 列表页支持 ?keywords=设计 参数;北京/上海/广州三地方向不同 |
| 小米汽车 | https://hr.xiaomi.com/campus | https://hr.xiaomi.com/ | 自建 | 小米招聘 | 汽车部与集团同库,站内搜"汽车 设计" |
| 极氪 Zeekr | https://campus.zeekrlife.com/#/jobs | https://app.mokahr.com/social-recruitment/geely/102003 | Moka(吉利租户) | ZEEKR极氪招聘 | 校招为 Moka 定制域名 |
| 零跑汽车 | https://leapmotor.zhiye.com/intern/jobs (实习);官网校招页 https://cn.leapmotor.com/join/campusRecruitment.html | https://cn.leapmotor.com/join/societyRecruitment.html | 北森 zhiye + 官网 | 零跑招聘 | 校招与实习生近年合并招募 |
| 阿维塔 | https://xcn5vbnquq58.jobs.feishu.cn/915151/ (飞书站) | https://talent.avatr.com/index | 飞书招聘+自建 | 阿维塔招聘 | 校招常经简章/公众号发布 |
| 智己汽车 | 无独立校招站,经公众号发布 | https://www.immotors.com/website/join_us | 未确认 | IM智己招聘号 | 监测靠公众号+实习僧/牛客搜索 |
| 岚图汽车 | https://app.mokahr.com/campus-recruitment/voyah/146293 | https://app.mokahr.com/social-recruitment/voyah/146292 | Moka(voyah 租户) | 岚图招聘 | — |
| 深蓝汽车 | 走长安集团统一校招 https://changan.zhiye.com/Campus | https://changan.zhiye.com/ | 北森 | 深蓝汽车招聘 | 站内按单位筛"深蓝" |
| 广汽埃安 | 走广汽集团校招 https://gacgroup2026.zhaopin.com/post/index.html | 智联企业页 | 智联定制站 | 广汽埃安招聘 | **域名按届次更换**(gacgroupXXXX) |
| 问界/赛力斯 | https://sokon.zhiye.com/campus | https://sokon.zhiye.com/ | 北森(sokon 租户) | 赛力斯集团招聘 | 体验规划/UX 岗 base 重庆为主 |

## 二 · OEM — 国央企/传统自主

| 公司 | 校招/实习入口 | 社招入口 | 系统 | 公众号 | 检测提示 |
|---|---|---|---|---|---|
| 比亚迪 | https://job.byd.com/portal/pc/ (校招社招同门户) | 同左 | 自建 | 比亚迪招聘 | 全球设计中心岗位在此发布;JS 加载 |
| 吉利汽车 | https://campus.geely.com/ (岗位路径形如 /campus-recruitment/geely/784xx/) | https://autojob.geely.com/ | 自建+Moka | GEELY吉利招聘 | 服务器 SSL 协议旧,抓取可能被拒,走兜底搜索 |
| 上汽集团 | https://saic-recruit.saicmotor.com | 同左 | 自建 | 上汽招聘 | 站内按单位筛(乘用车/研发总院/智己) |
| 上汽通用/泛亚 | https://sgm.zhiye.com/campus/jobs (支持 #KeyWords=设计) | https://sgm.zhiye.com/ | 北森 | 上汽通用汽车招聘 | 泛亚设计岗走此入口,不走 GM 全球站 |
| 广汽集团 | https://gacgroup2026.zhaopin.com/rpkj/index.html;研究院实习 https://gacrnd.zhiye.com/campus/jobs | https://gacrnd.zhiye.com | 智联定制+北森 | 广汽集团招聘 | **设计/HMI 岗主要挂广汽研究院(北森站)**;校招域名按届次换 |
| 广汽本田 | https://job.ghac.cn (校招路径 /Careers_Campus_Position) | 同左 | 自建 | 广汽本田招聘 | — |
| 长城汽车 | https://zhaopin.gwm.cn/ (校招社招同站) | 同左 | 大易/hotjob 定制 | 长城汽车招聘 | 座舱/HMI 在"技术中心/智能化"类目;base 保定为主 |
| 长安汽车 | https://changan.zhiye.com/Campus (支持 /jobs#KeyWords=设计) | https://changan.zhiye.com/Social | 北森 | 长安汽车招聘 | 含深蓝、长安系;base 重庆 |
| 一汽集团(红旗) | https://faw-zhaopin.hotjob.cn (岗位详情形如 /SU.../pb/posDetail.html) | https://faw.hotjob.cn/wt/FAW/web/index | hotjob(大易) | 中国一汽招聘 | 3D HMI 等岗 base 长春/天津 |
| 东飍汽车(含日产) | 集团 https://dfmc.hotjob.cn/;东风日产 https://www.dongfeng-nissan.com.cn/about/recruit/campus/ | https://dfmc.hotjob.cn/ | hotjob | 东风招聘 | 岚图单列(见上);注意 Moka 的 gufen 租户是"东风汽车股份"子公司 |
| 奇瑞汽车 | https://cheryholding.zhiye.com/campus | https://cheryholding.zhiye.com | 北森 | 奇瑞集团招聘 | 校招含"创意设计类"方向;base 芜湖 |
| 北汽集团(极狐) | https://baicgroup.zhiye.com/campus/jobs | https://baicgroup.zhiye.com/ | 北森 | 北汽集团招聘 | 站内按单位筛极狐 |

## 三 · OEM — 外资

外资普遍全年招实习,毕业生项目窗口各家不同。英文岗位关键词:UX / HMI / Interaction Design / Creative Design。

| 公司 | 校招/实习入口 | 社招/职位总入口 | 系统 | 公众号 | 检测提示 |
|---|---|---|---|---|---|
| 宝马中国(含 Designworks 上海) | https://careersite.tupu360.com/bmw/position;华晨宝马 https://careersite.tupu360.com/bmw-brilliance | https://www.bmwgroup.jobs/cn/en.html | 图谱 Tupu360+集团 jobfinder | BMW爱招人 | Designworks 岗位在全球 jobfinder 按 Location=Shanghai 筛;实习也常发实习僧 |
| 奔驰中国(上海研发/设计) | https://group.mercedes-benz.com/careers/ 选 Students & Graduates | https://jobs.mercedes-benz.com/en 筛 Location=China | 自建全球平台 | 梅赛德斯-奔驰招聘 | JS 渲染重,兜底走公众号+LinkedIn 搜索 |
| 沃尔沃(上海设计中心) | https://app.mokahr.com/campus_apply/volvocars/56034 | https://jobs.volvocars.com/ 筛 Shanghai | Moka(校招)+SuccessFactors | 沃尔沃汽车招聘 | 设计中心岗位常经 LinkedIn/内推,官网岗位少 |
| 通用 GM 中国/泛亚 | 泛亚走上汽通用入口(见上表);GM 自有岗位筛 Intern+China | https://search-careers.gm.com/en/jobs/?country=CN | Happydance+Workday | 泛亚汽车技术中心 | GM 站有 Creative Design 团队筛选项 |
| 大众中国(CARIAD/大众安徽) | http://campus.51job.com/vgc/;实习 https://volkswagengroupchina.com.cn/zh-cn/career/internship | https://volkswagengroupchina.jobs2web.sapsf.cn/?locale=zh_CN;CARIAD https://jobs.volkswagen-group.com/cariad/ | SuccessFactors | CARIAD China(有独立号) | 官网部分路径需浏览器访问 |
| 保时捷中国(上海研发) | https://jobs.porsche.com/ 筛 Internship+China | https://jobs.porsche.com/ 筛 Land=China | 自建 | 保时捷中国 | — |
| 丰田中国(IEM) | http://campus.51job.com/toyota2026 (**按届换 toyota+年份**) | https://www.toyota.com.cn/about/recruitment/ | 51job 托管+自建 | 丰田中国 | 官网重定向问题,优先 51job 站 |
| 奥迪中国 | https://volkswagengroupchina.jobs2web.sapsf.cn/audichina/?locale=zh_CN (实习项目全年) | 同左(社招) | SuccessFactors | 奥迪中国招聘 | 无常设校招,以实习转正为主;奥迪一汽 NEV 另有官网 |
| 福特中国 | https://app.mokahr.com/campus-recruitment/ford/43706 | Moka ford 租户社招站 | Moka | 福特招聘 | — |

## 四 · 供应商 — 科技大厂

| 公司 | 校招/实习入口 | 社招入口 | 系统 | 公众号 | 检测提示 |
|---|---|---|---|---|---|
| 华为(车BU/鸿蒙智行) | https://career.huawei.com/reccampportal/portal5/campus-recruitment.html (含实习频道) | https://career.huawei.com/reccampportal/portal5/social-recruitment.html | 自建 | 华为招聘 | 搜"智能座舱/HMI/HarmonyOS";部分岗位以"深圳引望"名义发布 |
| 百度(Apollo/IDG) | https://talent.baidu.com/jobs/list?recruitType=GRADUATE;实习 ?recruitType=INTERN | ?recruitType=SOCIAL | 自建 | 百度招聘 | 无业务线筛选,用关键词"智能驾驶/座舱" |
| 高德地图(阿里) | https://talent.amap.com/campus (岗位详情 /campus/position-detail?positionId=xxx) | https://talent.amap.com/ | 自建 | 高德招聘 | 车机/出行体验设计岗,AI 体验设计方向活跃 |
| 腾讯(智慧出行) | https://join.qq.com/ | https://careers.tencent.com/search.html 筛 CSIG | 自建 | 腾讯校招 | 关键词"智慧出行/智能座舱" |
| 大疆卓驭(智驾) | 牛客企业号 https://www.nowcoder.com/enterprise/245760;官网 https://www.zyt.com/zh/ | 猎聘/BOSS 官方账号 | 无独立门户 | — | 设计岗少,以算法为主;监测优先级低 |
| 地平线 | https://wecruit.hotjob.cn/SU6409ef49bef57c635fd390a6/pb/school.html | https://horizon.hotjob.cn/ | 北森 wecruit | 地平线HORIZON | 智驾方向 UX 岗存在(base 北京) |
| Momenta | https://momenta.jobs.feishu.cn/campus;实习 /intern | https://momenta.jobs.feishu.cn/ | 飞书招聘 | Momenta | 搜"HMI/交互/设计" |
| 科大讯飞(智能汽车) | https://iflytek.zhiye.com/ (实习 /intern/jobs) | https://sp.wintalent.cn/iflytek/index.html | 北森 | 科大讯飞招聘 | 按事业部筛"智能汽车" |
| 千里科技 | 无统一门户,牛客/高校就业网搜"千里智驾 千里智舱" | 猎聘/BOSS | 无 | — | 岗位以智驾算法为主;监测优先级低 |

## 五 · 供应商 — 外资

外资供应商基本全年开坑,设计岗集中在座舱/信息娱乐业务线。

| 公司 | 校招/实习入口 | 社招入口 | 系统 | 公众号 | 检测提示 |
|---|---|---|---|---|---|
| 博世中国 | https://app.mokahr.com/campus-recruitment/bosch/73873;实习 https://www.bosch.com.cn/careers/job-offers/internship/ | https://www.bosch.com.cn/careers/job-offers/professionals-recruitment/ | Moka+SmartRecruiters | 博世中国人才苑 | — |
| AUMOVIO(原大陆集团座舱业务) | https://aumovio.51job.com/ | https://www.aumovio.com/en/career/job-openings.html | 51job 专区+官网 | — | **座舱/HMI 业务 2025 年从大陆拆分为 AUMOVIO**,别再盯 continental 域名 |
| 法雷奥中国 | https://campus.51job.com/valeo2026/ (**按届换**) | https://valeo.gllue.com/portal | 谷露 Gllue+51job | 法雷奥招聘 | — |
| 佛瑞亚 FORVIA | http://ideal.51job.com/forvia/school.html | https://www.forvia.com/careers;BOSS"佛吉亚(中国)投资" | 51job+全球官网 | — | 座舱电子/内饰均有设计岗 |
| 哈曼 Harman | https://jobs.harman.com/ 搜 intern+China | https://jobs.harman.com/ 搜"UX HMI China" | SuccessFactors | — | 上海/深圳常年招座舱 UX/HMI;校招 51job 域名按届换 |
| 电装 Denso | http://denso.zhiye.com/ | 同左 | 北森 | — | 设计岗少,以工程为主;优先级低 |
| 安波福 Aptiv | http://aptiv.51job.com/ | https://jobs.aptiv.com/ | Phenom+51job | — | 座舱相关多在软件团队 |

## 六 · 供应商 — 国内

| 公司 | 校招/实习入口 | 社招入口 | 系统 | 公众号 | 检测提示 |
|---|---|---|---|---|---|
| 中科创达 | https://www.thundersoft.com/xiaozhao/ | https://thundersoft.jobs.feishu.cn/ | 飞书招聘 | 中科创达招聘 | 座舱 UI/HMI 是主营业务,常年有设计岗 |
| 德赛西威 | https://yesv-desaysv.jobs.feishu.cn/campus/ | https://yesv-desaysv.jobs.feishu.cn/ | 飞书招聘 | 德赛西威招聘 | 座舱 HMI 设计岗集中惠州/上海 |
| 亿咖通 ECARX | https://ecarxgroup.jobs.feishu.cn/career/ | 同左 | 飞书招聘 | ECARX亿咖通科技 | — |
| 斑马智行 | https://banma.zhiye.com/Campus | https://www.ebanma.com/joinus.html | 北森 | 斑马智行 | — |
| 博泰车联网 | https://www.pateo.com.cn/zh/career.html | https://www.pateo.com.cn/zh/career_2.html | 邮箱投递 HRZP@pateo.com.cn | — | 职位页明确有"HMI与交互中心"部门 |
| 东软集团(汽车电子) | https://career.neusoft.com/ | 同左 | 自建 | 东软集团招聘 | 含东软睿驰;大连/沈阳座舱团队 |
| 光庭信息 | http://www.kotei.com.cn "加入我们" | BOSS直聘搜"武汉光庭信息" | 无 ATS | 光庭信息 | 官方站不稳定,监测走 BOSS/兜底搜索 |
| faceui | 官网 http://www.faceui.com | BOSS直聘/站酷搜"FACEUI" | 无 ATS | — | 上海/成都 HMI 设计公司,招聘走 BOSS/站酷 |
| 阿尔特 IAT | http://www.iat-auto.com/job.php?lm=26 | 智联搜"阿尔特" | 智联 | — | 有座舱显示产品类岗位 |

## 七 · 通用兜底渠道

官方入口抓不到内容时,按顺序用这些渠道交叉验证:

1. **牛客网** — `site:nowcoder.com 公司名 设计 校招/实习`,企业号和讨论区时效性好,常有 HC 开关的一手消息
2. **实习僧** — `site:shixiseng.com 公司名 HMI/设计`,外资和新势力实习岗常发这里(宝马实习就走实习僧)
3. **高校就业网** — 搜 `公司名 2027届 校园招聘 就业网`,国央企简章几乎必发高校就业网,信息权威且带截止日期
4. **微信公众号文章** — 搜 `公司公众号名 + 校招/实习 + 开启`,搜狗微信搜索或直接 WebSearch
5. **小红书** — 搜"公司名 校招 设计",学生分享的 timeline 信息(笔试/面试进度)可辅助判断批次状态,但不作为开岗依据

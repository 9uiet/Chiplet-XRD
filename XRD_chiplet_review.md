# 晶体洞察：XRD表征测试技术综述及其在芯粒技术中的应用

## 摘要
X射线衍射（XRD）是揭示材料晶体结构的核心非破坏性表征技术。本文以《Insights Through Crystals: Exploring X-Ray Diffraction Techniques》为主要参考，结合五篇先进封装与残余应力调控文献，对XRD的物理原理、仪器体系、测试方法、数据解析与质量控制进行系统综述，并聚焦芯粒技术中的关键应用场景，包括系统级封装（SiP）与芯粒异质集成中的材料相鉴定、晶粒取向与织构分析、薄膜/互连残余应力评价及玻璃基板TGV可靠性评估。通过讨论多维X射线表征（XRR、X射线成像/层析等）与XRD的协同关系，提出面向芯粒技术的工程化测试流程与发展趋势。本文同时标注了来自六篇文献的图示来源，但不复制图像内容，需在获得版权授权后插入原图。

## 简介
芯粒（chiplet）与系统级封装推动了异质集成的规模化应用，器件结构日益三维化、互连密度持续提升，材料与结构的晶体学表征成为保障可靠性与性能的基础环节。XRD依托Bragg衍射原理，能够无损测量晶格常数、相组成、织构与应变，是先进封装与半导体制造中不可或缺的通用表征手段[1][4]。在系统级封装与芯粒集成中，封装材料组合复杂、工艺链长，电镀Cu互连、玻璃基板与TGV等关键结构的残余应力与晶粒组织直接影响失效模式与可靠性[2][3][5][6]。因此，系统化梳理XRD技术并讨论其在芯粒技术中的应用，对建立高可信度表征与质量控制体系具有重要意义。

## 正文

### 1. XRD技术原理与物理基础
XRD基于晶体中周期性晶面产生的衍射干涉，满足Bragg定律 nλ=2d sinθ。X射线在晶体内发生弹性散射并形成干涉条纹，衍射峰的位置、强度和形貌反映晶格间距、取向分布与晶体缺陷等信息[1]。衍射几何的核心在于晶面族与入射/出射波矢之间的关系，进而在倒易空间中形成可测的衍射条件。对芯粒封装材料而言，这意味着可以通过衍射峰偏移来量化应变，通过峰展宽或形状变化估计晶粒尺寸与微应变，进而评估互连材料与薄膜的工艺稳定性。

图1：Bragg定律与衍射几何示意（来源：文献[1] Fig.1）。

### 2. 仪器体系与测试配置
典型XRD系统由X射线源、准直与单色化组件、测角仪以及探测器组成[1]。X射线源常用Cu靶Kα辐射，配合滤波器或单色器降低Kβ与杂散背景；准直系统控制束斑尺寸与发散角；测角仪通过θ-2θ扫描获取粉末或多晶样品的衍射谱；探测器包括比例计数器、闪烁计数器或二维阵列探测器以提升效率。在先进封装中，为适配薄膜、微区或复杂几何结构，常采用掠入射XRD（GIXRD）、高分辨XRD（HRXRD）、面阵探测与微束扫描等配置以提高表面灵敏度与空间分辨率[4]。

图2：XRD仪器组成与光路示意（来源：文献[1] Fig.4）。

### 3. XRD表征方法与数据解析
XRD测试方法可按样品形态与信息维度分类：
（1）粉末衍射用于相鉴定与晶格常数测量，是材料库匹配与工艺一致性评估的基础手段；
（2）单晶衍射用于解析晶体结构与取向；
（3）薄膜与层状结构常采用GIXRD或HRXRD以抑制基底信号并提升薄膜灵敏度；
（4）织构分析通过极图或ODF量化晶粒取向分布；
（5）残余应力测试可采用sin^2ψ法，利用不同倾角下晶面间距变化求得面内应力；
（6）倒易空间映射（RSM）能分离应变、位错与弛豫程度；
（7）与XRR、X射线成像/层析、XRF等方法联用，实现多尺度结构与成分协同分析[4]。

数据解析方面，常用峰位拟合与背景扣除实现相鉴定与晶格参数求解；Scherrer公式可估计晶粒尺寸，Williamson–Hall或Rietveld精修可进一步分离尺寸效应与微应变[1]。对于芯粒封装材料，需特别关注样品制备的应力释放、表面粗糙度与取向偏置带来的系统误差，必要时通过标准样或对比样进行校准。

### 4. 半导体与先进封装中的XRD与多维X射线表征
半导体制造与先进封装强调结构缺陷、应变与界面质量的多维表征。Crystals综述指出，XRD、XRR、X射线成像与层析可覆盖从纳米到宏观尺度的多种对比机制，适用于薄膜密度、界面粗糙度、三维缺陷与晶格应变的综合评估[4]。例如，XRR可用于薄膜厚度与密度拟合；同步辐射微束XRD可在局部区域解析应变分布；相衬X射线层析在封装内部缺陷检测中具备非破坏优势。这些方法与XRD互补，有助于构建芯粒封装的多尺度结构数据链。

图3：X射线成像/层析典型配置示意（来源：文献[4] Figure 3）。

### 5. 芯粒技术中的应用场景与案例
芯粒集成通常依赖SiP与先进封装平台（如2.5D/3D集成、桥接互连或混合键合）实现高带宽互连与系统级优化[2]。在此背景下，XRD主要承担以下任务：
1）互连与电镀Cu组织控制：电镀Cu残余应力会导致开裂、翘曲或界面剥离，文献[3][5][6]通过调整电流密度、添加剂与晶粒特征来调控应力，XRD用于量化织构、取向与应力变化，是工艺优化的核心手段；
2）玻璃基板与TGV可靠性：玻璃基板具有低损耗与CTE匹配优势，但TGV电镀过程的应力集中易引起损伤[3][5]，XRD结合FIB/EBSD可揭示晶粒取向与残余应力的内在关联；
3）薄膜与界面应变：在混合键合、微凸点与RDL工艺中，XRD可检测薄膜应变与相变，为工艺窗口与退火条件提供量化依据；
4）失效分析与安全性评估：SiP中的失效分析可与X射线成像、层析技术联用[2][4]，实现结构缺陷与材料异常的无损诊断。

图4：不同电流密度下电镀Cu的XRD与残余应力结果（来源：文献[3] Fig.2）。
图5：电镀Cu晶粒组织变化与XRD谱/织构系数示意（来源：文献[6] Fig.4）。

### 6. 工程化测试流程与质量控制
针对芯粒封装，建议建立“样品制备—测试参数—数据解析—工艺反馈”的闭环流程：
（1）样品制备应减少机械加工导致的应力释放，薄膜样品需控制表面粗糙度与污染；
（2）测试参数需匹配材料体系与层厚，合理选择扫描步进、计数时间与倾角范围；
（3）数据解析应统一峰位拟合、背景扣除与应力模型，必要时使用标准样进行标定；
（4）与EBSD、SEM、XRR等手段交叉验证，提升对晶粒取向、晶界特征与应力分布的解释可信度；
（5）对关键结构（如TGV、电镀Cu或混合键合界面）建立XRD指标阈值，实现量产质量控制与失效预警。

## 讨论
XRD在芯粒封装中的优势在于非破坏、可量化与可与工艺参数直接关联，但也存在局限：其对非晶或极薄层的灵敏度有限；多层结构易产生衍射峰重叠；样品取向与表面粗糙度会带来系统误差。为弥补这些不足，可引入掠入射或同步辐射微束XRD，并与XRR、X射线层析或光谱技术协同[4]。此外，SiP与芯粒系统的安全与逆向分析研究表明，X射线成像和层析在失效诊断与结构验证中具有重要价值[2]，但其与XRD的联合数据建模仍需进一步标准化。未来，结合机器学习的峰形分解、快速Rietveld精修与在线监测，将推动XRD从离线表征向工艺过程监控演进。

## 结论
XRD作为晶体结构表征的基础技术，在芯粒与先进封装领域展现出广泛应用价值。本文系统梳理了XRD原理、仪器体系与典型测试方法，总结其在电镀Cu残余应力调控、玻璃基板TGV可靠性、薄膜应变评估与多维X射线表征协同中的关键作用。面向芯粒技术的高密度、三维化趋势，XRD将与多模态X射线技术和数据驱动分析深度融合，为结构可靠性与工艺优化提供更加精确、可量化的支撑。

## 参考文献
[1] Gauniya, P.; Chitra; Radheshyam; Semalty, A.; Gupta, M.; Sagdeo, A.; Semalty, M. Insights Through Crystals: Exploring X-Ray Diffraction Techniques. J. Mountain Res. 2024, 19(2), 533–544. DOI: 10.51220/jmr.v19-i2.55.
[2] Khan, M. S. M.; Xi, C.; Ul Haque, M. S.; Tehranipoor, M. M.; Asadizanjani, N. Exploring Advanced Packaging Technologies for Reverse Engineering a System-in-Package (SiP). IEEE Trans. Components, Packaging and Manufacturing Technology 2023, 13(9).
[3] Yang, G.; Li, L.; Chang, L.; Yang, W.; Zhang, G.; Zhang, Z.; Shi, T. Residual Stress Control Based on Electroplated Metal Grain Characteristics in Panel-Level Glass Advanced Packaging. Proc. 2024 25th International Conference on Electronic Packaging Technology (ICEPT).
[4] Jiang, Y.; Zhang, Z.; An, Z.; Pan, X.; Shi, X.; Wang, R.; Chen, C.; Cao, Z.; Xu, Y.; Wei, J.; Zhang, X.; Peng, Y. X-Ray Characterization of Semiconductor Materials and Advanced Packaging: A Perspective on Multidimensional Structural Analysis. Crystals 2026, 16, 265.
[5] Yang, G.; Shi, T.; Chang, L.; Zhu, H.; Tong, D.; Yang, W.; Li, Z.; Li, L. A Study on Regulating the Residual Stress of Electroplated Cu by Manipulating the Nanotwin Directions. Micromachines 2024, 15, 1370. https://doi.org/10.3390/mi15111370.
[6] Yang, G.; Yang, W.; Li, L.; Shi, T.; Chang, L.; Zhu, H.; Li, Y.; Tong, D. A Strategy for Regulating the Residual Stress of Electroplated Cu Film Based on Customized Grain Characteristics. Materials Chemistry and Physics 2025, 345, 131304.

### 文献[1]参考文献节摘录（原文顺序，轻度清理）
- Aguilar-Marín P, Angelats-Silva L, Noriega-Diaz E, Chavez-Bacilio M, Verde-Vera R (2020) the phenomenon of x-ray Understanding diffraction by crystals and related concepts. European Journal of Physics 41(4): 045501.
- Ali A, Chiang YW, Santos RM (2022) X-ray diffraction mineral techniques characterization: A review for engineers of the for fundamentals, directions. Minerals 12(2): 205. applications, and research application incorporated Başaran E (2017) Ocular of dirithromycin polymeric nanoparticles: An in vitro evaluation. Turkish Journal of Pharmaceutical Sciences,14(2): 191.
- Bayat M, Zargar M, Astarkhanova T, Pakina E, Ladan S, Lyashko M, Shkurkin SI (2021) Facile biogenic synthesis and characterization of seven metal-based nanoparticles conjugated with phytochemical bioactives using fragaria ananassa leaf extract. Molecules, 26(10): 3025.
- Bond AD (2016) Single-crystal X-ray diffraction. Analytical Techniques in the Pharmaceutical Sciences:315-37.
- Bunaciu AA, UdriŞTioiu EG, Aboul-Enein HY (2015) X-ray diffraction: Instrumentation and applications. Critical reviews in analytical chemistry 45(4): 289-99.
- Cain H (2020) X-ray Diffraction Techniques and instrumentation. Unified Theory and Practice: Polymer Adhesion, X-Ray Diffraction & X- Ray Florescence:207.
- Chala DB, Emire SA (2021) X-Ray Diffraction and Patterns: Diffraction Techniques Application for Food Quality Assurance in Bio-Food Industry.
- Journal of Emerging Science and Chatterjee SK (2010) X-ray diffraction: Its theory and applications. PHI Learning Pvt. Ltd.; ISBN-978-81-203-4194-4.
- Coulombwall A (2020) High-Resolution X-ray Diffraction. Advanced Lab Course Manual. TUM-Physik.
- Dowsett M, Wiesinger R, Adriaens M (2021) X-ray diffraction. In Spectroscopy, Diffraction, and Tomography in Art and Heritage Science.
- Elsevier :161-207 Eckert M (2012) Max von Laue and the discovery of X‐ray diffraction in 1912. Annalen der Physik, 524(5): A83-5.
- Epp J (2016) X-ray diffraction (XRD) techniques for In Materials characterization. materials using nondestructive (NDE) methods. Woodhead characterization evaluation Publishing, 81-124.
- Fewster PF (2014) A new theory for X-ray diffraction. Acta Crystallographical Section A: Foundations and Advances, 70(3): 257-82.
- Guinebretière R (2013) X-ray diffraction by polycrystalline materials.
- John Wiley & Sons, Hammond C (2015) The basics of crystallography and diffraction. Oxford University Press, USA.
- Ingham B (2015) X-ray scattering characterisation of nanoparticles. Crystallography Reviews, 21(4): 229-303.
- J (2015) The Braggs, X-Ray Crystallography, and Lawrence Bragg’s Sound- Ranging in World War I. Interdisciplinary Science Review, 40(3): 222-43.
- Jenkin Khan H, Yerramilli AS, D'Oliveira A, Alford TL, Boffito DC, Patience GS (2020) Experimental in chemical engineering: X‐ray methods diffraction spectroscopy—XRD. The Canadian J Chemical Eng, 98(6): 1255.
- Khondker A, Lakhani S (2015) X-ray diffraction: A comprehensive explanation for multipurpose research. Int. J. Interdiscip. Res. Innov 3: 60-4.
- Kulhari H, Pooja D, Shrivastava S, Naidu VG, Sistla (2014). Peptide conjugated polymeric R. nanoparticles as a carrier for targeted delivery of docetaxel Colloids and Surfaces B: Biointerfaces, 117: 166-73.
- Kumar VD, Verma PR, Singh SK (2015) Development and evaluation of biodegradable polymeric nanoparticles the effective delivery of quercetin using a quality by design approach. LWT-Food Science and Technology, 61(2): 330-8. for Lee M (2017) X-Ray diffraction for materials research: from fundamentals to applications. CRC Press. https://doi.org/10.1201/b19936 Lekshmi UM, Poovi G, Reddy PN (2012) In-vitro engineered observation polymeric nanoparticles. Digest Journal of Nanomaterials & Biostructures, (DJNB) 7(1). repaglinide of Li J, Sun J (2017) Application of X-ray diffraction and electron crystallography solving complex structure problems. Accounts of chemical research, 50(11): 2737-45. for Mathews JP, Campbell QP, Xu H, Halleck P (2017) A review of the application of X-ray computed tomography to the study of coal Fuel 209: 10- 24.
- Muthu MS, Singh S (2008) Studies on biodegradable polymeric nanoparticles of risperidone: in vitro and in vivo evaluation. Nanomedicine, 3(3): 305-19.
- Purohit SR, Jayachandran LE, Raj AS, Nayak D, Rao PS (2019). X-ray diffraction for food quality evaluation. In Evaluation technologies for food quality. Woodhead Publishing, 579- 594.
- Ramasamy T, Tran TH, Choi JY, Cho HJ, Kim JH, Yong CS, Choi HG, Kim JO (2014) Layer-by- layer coated lipid–polymer hybrid nanoparticles designed for use in anticancer drug delivery. Carbohydrate polymers, 102: 653-61.
- Saini BS, Kaur R (2021) X-ray diffraction. In Handbook of Modern Coating Technologies (pp85-141).
- Sayers Z, Avşar B, Cholak E, & Karmous I (2017) Application of advanced X-ray methods in life sciences. Biochimica et Biophysica Acta (BBA)- General Subjects 1861(1): 3671-3685. and Seeck OH, Murphy B (2015) Overview of X-ray and scattering techniques. diffraction: Modern Experimental Techniques: 1.
- Jenny Stanford Publishing, New York diffraction theory x-ray Segmiiller A (2012). Characterization Of Thin Films By X-ray Diffraction. Thin Films from Free Atoms and Particles:325. ISBN 0-12-410755-9 Semalty A. (2014). Cyclodextrin and phospholipid complexation in solubility and dissolution enhancement: A critical and meta-analysis. Expert Opin Drug Deliv. 11(8): 1255–1272. Semalty A, Semalty M, Singh D.
- Rawat MSM (2010). Preparation and characterization of phospholipid complexes of naringenin for effective drug delivery. J Incl Phenom Macrocycl Chem 67; 253–260.
- Shaker MA, Elbadawy HM, Al Thagfan SS, Shaker MA (2021) Enhancement of atorvastatin oral bioavailability via encapsulation in polymeric of International nanoparticles. Pharmaceutics, 592:120077.
- Journal Singh V, Shrivastava A, Wahi N (2015) Biosynthesis of silver nanoparticles by plants crude extracts and their characterization using UV, XRD, TEM and EDX. African Journal of Biotechnology, 14(33): 2554-2567. (2013). Bragg, microdiffraction and X-ray lasers. Acta Crystallographica Section A: Foundations of Crystallography;69(1):25-33.
- Lawrence JC Spence Suryanarayanan R and Rastogi S (2013) X-ray of diffractometry. Encyclopedia powder Pharmaceutical Technology.
- Tanner BK (2013) Characterization of crystal growth defects by X-ray methods. Springer Science Media; https://link.springer.com/book/10.1007/978-1- 4757-1126-4 Business & Younas M, Rizwan M, Zubair M, Inam A, Ali S (2021) Biological synthesis, characterization of three metal-based nanoparticles and their anticancer activities against hepatocellular carcinoma HepG2 cells. Ecotoxicology and Environmental Safety, 223: 112575.
- Yurtdaş-Kirimlioğlu G, Sinan ÖZ, Büyükköroğlu G, Yazan Y (2018) Formulation and in vitro evaluation of moxifloxacin hydrochloride- loaded polymeric nanoparticles for ocular application. Latin American Journal of Pharmacy, 37(9): 1850-62.
- Zolotoyabko E (2014) Basic concepts of X-ray diffraction. John Wiley & Sons; ISBN: 978-3- 527-68118-1.

### 文献[2]参考文献节摘录（原文顺序，轻度清理）
- [1] J. H. Lau, Chiplet Heterogeneous Integration. Singapore: Springer, 2021, pp. 413–439, doi: 10.1007/978-981-16-1376-0_9.
- [2] J. H. Lau, “Recent advances and trends in advanced packaging,” IEEE Trans. Compon., Packag., Manuf. Technol., vol. 12, no. 2, pp. 228–252, Feb. 2022.
- [3] T. Li, J. Hou, J. Yan, R. Liu, H. Yang, and Z. Sun, “Chiplet heteroge- neous integration technology-status and challenges,” Electronics, vol. 9, no. 4, p. 670, 2020.
- [4] T. Uhrmann, J. Burggraf, and M. Eibelhuber, “Heterogeneous integration by collective die-to-wafer bonding,” in Proc. Int. Wafer Level Packag. Conf. (IWLPC), Oct. 2018, pp. 1–7.
- [5] T. Trend, “From technologies to markets medical wearables: Market and technology trend,” Adv. Packag.: Strong Momentum Pushed Giants, Yole Group, Lyon, France, Tech. Rep., 2019.
- [6] M. Enamulquadir et al., “A survey on chip to system reverse engineer- ing,” ACM J. Emerg. Technol. Comput. Syst., vol. 13, pp. 1–34, 2016, doi: 10.1145/2755563.
- [7] S. M. Zulkifli, B. Zee, W. Qiu, and A. Gu, “High-res 3D X-ray microscopy for non-destructive failure analysis of chip-to-chip micro- bump interconnects in stacked die packages,” in Proc. IEEE 24th Int. Symp. Phys. Failure Anal. Integr. Circuits (IPFA), Jul. 2017, pp. 1–5.
- [8] S. Liebert, “Failure analysis from the back side of a die,” in Proc. 8th Int. Symp. Phys. Failure Anal. Integr. Circuits, 2001, pp. 187–194.
- [9] R. Torrance and D. James, “The state-of-the-art in IC reverse engi- neering,” in Cryptographic Hardware and Embedded Systems—CHES, C. Clavier and K. Gaj, Eds. Berlin, Germany: Springer, 2009, pp. 363–381.
- [10] N. Asadizanjani, M. Tehranipoor, and D. Forte, “PCB reverse engi- neering using nondestructive X-ray tomography and advanced image processing,” IEEE Trans. Compon., Packag., Manuf. Technol., vol. 7, no. 2, pp. 292–299, Feb. 2017.
- [11] W.-C. Chen et al., “Development of novel fine line 2.1 D package with organic interposer using advanced substrate-based process,” in Proc. IEEE 68th Electron. Compon. Technol. Conf. (ECTC), May 2018, pp. 601–606.
- [12] S. Y. Hou et al., “Wafer-level integration of an advanced logic-memory system through the second-generation CoWoS technology,” IEEE Trans. Electron Devices, vol. 64, no. 10, pp. 4071–4077, Oct. 2017.
- [13] R. Mahajan et al., “Embedded multi-die interconnect bridge (EMIB)— A high density, high bandwidth packaging interconnect,” in Proc. IEEE 66th Electron. Compon. Technol. Conf. (ECTC), May 2016, pp. 557–565.
- [14] D. B. Ingerly et al., “Foveros: 3D integration and the use of face-to-face chip stacking for logic devices,” in IEDM Tech. Dig., Dec. 2019, p. 19.
- [15] W.-Y. Wu, M.-J.-J. Wang, and C.-M. Liu, “Automated inspec- tion of printed circuit boards through machine vision,” Comput. Ind., vol. 28, no. 2, pp. 103–111, May 1996. [Online]. Available: https://www.sciencedirect.com/science/article/pii/0166361595000631
- [16] R. Che, S. Azmi, and R. Daud, “Morphological operation on printed cir- cuit board reverse engineering using MATLAB,” in Proc. Knowl. Manag. Int. Conf. Exhib. (KMICE), 2006, pp. 529–533. [Online]. Available: http://www.kmice.cms.net.my/ProcKMICe/KMICe2006/Pdf/529.pdf
- [17] N. Asadizanjani, S. Shahbazmohamadi, M. Tehranipoor, and D. Forte, “Non-destructive PCB reverse engineering using X-ray micro com- puted tomography,” in Proc. Int. Symp. Test. Failure Anal., Nov. 2015, pp. 164–172.
- [18] E.-P. Rührnschopf and K. Klingenbeck, “A general framework and review of scatter correction methods in X-ray cone-beam computerized tomography. Part 1: Scatter compensation approaches,” Med. Phys., vol. 38, no. 7, pp. 4296–4311, Jun. 2011.
- [19] L. Zhu, N. R. Bennett, and R. Fahrig, “Scatter correction method for X-ray CT using primary modulation: Theory and preliminary results,” IEEE Trans. Med. Imag., vol. 25, no. 12, pp. 1573–1587, Dec. 2006.
- [20] C. Reaño and F. Silla, “Performance evaluation of the NVIDIA Pascal GPU architecture: Early experiences,” in Proc. IEEE 18th Int. Conf. High Perform. Comput. Commun., IEEE 14th Int. Conf. Smart City, IEEE 2nd Int. Conf. Data Sci. Syst. (HPCC/SmartCity/DSS), Dec. 2016, pp. 1234–1235.
- [21] T. Farheen et al., “Proof of reverse engineering barrier: SEM image analysis on covert gates,” in Proc. Int. Symp. Test. Failure Anal., Oct. 2021, pp. 179–189.
- [22] H. Wang, Q. Shi, A. Nahiyan, D. Forte, and M. M. Tehranipoor, “A physical design flow against front-side probing attacks by internal shielding,” IEEE Trans. Comput.-Aided Design Integr. Circuits Syst., vol. 39, no. 10, pp. 2152–2165, 2020, doi: 10.1109/TCAD.2019.2952133.
- [23] M. S. M. Khan, C. Xi, A. A. Khan, M. T. Rahman, M. M. Tehranipoor, and N. Asadizanjani, “Secure interposer-based heterogeneous integra- tion,” IEEE Des. Test., vol. 39, no. 6, pp. 156–164, Dec. 2022.
- [24] T. Rahman, M. K. Bepary, M. S. Ul Haque, M. Tehranipoor, and F. Rahman, “Design and security-mitigation of custom and configurable hardware cryptosystems,” in Proc. IEEE 16th Dallas Circuits Syst. Conf. (DCAS), Apr. 2023, pp. 1–6.
- [25] J. Talukdar, A. Chaudhuri, J. Kim, S. K. Limt, and K. Chakrabarty, “Securing heterogeneous 2.5D ICs against IP theft through dynamic interposer obfuscation,” in Proc. Design, Autom. Test Eur. Conf. Exhib. (DATE), Apr. 2023, pp. 1–2. in electrical and electronic engineering from the currently the Ph.D. degree with the Electrical and Computer Engineering Department, University of Florida, Gainesville, FL, USA. security, hardware security and trust, and physical inspection and attacks. FL, USA, in 2020, where he is currently pursuing the Ph.D. degree with the Electrical and Computer Engineering Department. detection and prevention methods for integrated cir- cuit designs and packaging. sity of Engineering and Technology (BUET), Dhaka, Ph.D. degree in electrical and computer engineering USA. engineering, finding vulnerabilities, and root of trust verification in IC. Mark M. Tehranipoor (Fellow, IEEE) served as the Founding Director with the CHASE and CSI Centers, University of Connecticut, Storrs, CT, USA. inence Endowed Chair Professor of cybersecurity and the Chair of the ECE Department, University of Florida, Gainesville, FL, USA, where he is cur- rently serving as a Founding Director for Florida Institute for Cybersecurity Research (FICS). He has published more than 500 journal articles and ref- ereed conference papers and has delivered about 200 invited talks and keynote addresses. He has published 14 books. His current research projects include hardware security and trust, supply chain security, IoT security, VLSI design, testing, and reliability. ACM and ACM SIGDA. He serves on the program committee of more than a dozen leading conferences and workshops. He has also served as the Program Chair of a number of IEEE and ACM-sponsored conferences and workshops (HOST, ITC, DFT, D3T, DBT, and NATW). He served as the General Chair of HOST-2008 and HOST-2009. He co-founded the IEEE International serving as a founding EIC for the Journal on Hardware and Systems Security (HaSS). He was a recipient of the dozen best paper awards and nominations, as well as the 2008 IEEE Computer Society (CS) Meritorious Service Award, the 2012 IEEE CS Outstanding Contribution, the 2009 NSF CAREER Award, Florida Innovation of the Year award. He served as an Associate Editor for Journal of Electronic Testing: Theory and Applications, Journal of Low Power (VLSI) SYSTEMS, and ACM Transactions on Design Automation of Elec- tronic Systems. mechanical engineering from the University of Con- necticut, Storrs, CT, USA, in 2014. Electrical and Computer Engineering Department, involved with counterfeit detection and prevention, system- and chip-level reverse engineering, and antireverse engineering. This includes a wide range of products from electronic systems to devices. His inspection of electronics. ence. He is serving on the Technical Program Committee of several top conferences, including the International Symposium of Testing and Failure Analysis (ISTFA) and the IEEE Computing and Communication Workshop and Conference (CCWC). He has received and been nominated for several best paper awards from the International Symposium on Hardware-Oriented Security and Trust (HOST) and the International Symposium on Flexible Automation (ISFA). He was also the winner of the D.E. Crow Innovation Award from the University of Connecticut.

### 文献[3]参考文献节摘录（原文顺序，轻度清理）
- [1] Benali, A., et al. "Analytical and finite element modeling of through glass via thermal stress." Microelectronic Engineering 151 (2016): 12- 18.
- [2] Demir, Kaya, et al. "Reliability of copper through-package vias in bare glass interposers." IEEE Transactions on Components, Packaging and Manufacturing Technology 7.6 (2017): 829-837.
- [3] Okoro, Chukwudi, et al. "A detailed failure analysis examination of the effect of thermal cycling on Cu TSV reliability." IEEE Transactions on Electron Devices 61.1 (2013): 15-22.
- [4] Wei, Tiwei, et al. "Performance and reliability study of TGV interposer in 3D integration." 2014 IEEE 16th electronics packaging technology conference (EPTC). IEEE, 2014.
- [5] Feng, Xue, et al. "Study of internal stress on electroplating copper used in through silicon via filling." 2011 12th International Conference on Electronic Packaging Technology and High Density Packaging. IEEE, 2011.
- [6] Wang, Ju, et al. " Tuning Stress in Cu Thin Films by Developing Highly (111)-Oriented Nanotwinned Structure." Journal of Electronic Materials 49 (2020): 109-115.
- [7] Sun, Fu-Long, et al. "Electrodeposition and growth mechanism of preferentially orientated nanotwinned Cu on silicon wafer substrate." Journal of materials science & technology 34.10 (2018): 1885-1890.
- [8] Xu, Di, et al. "Nanotwin formation in copper thin films by stress/strain relaxation in pulse electrodeposition." Applied Physics Letters 91.25 (2007).
- [9] Chan, Tsung-Cheng, Yu-Lun Chueh, and Chien-Neng Liao. "Manipulating the crystallographic texture of nanotwinned Cu films by electrodeposition." Crystal growth & design 11.11 (2011): 4970-4974.
- [10] Kremmer, K., et al. "Interplay between the deposition mode and microstructure in electrochemically deposited Cu thin films." Thin Solid Films 515.17 (2007): 6698-6706.
- [11] Lu, Tien-Lin, et al. "Anisotropic grain growth in (111) nanotwinned Cu films by DC electrodeposition." Materials 13.1 (2019): 134. 2024 25th International Conference on Electronic Packaging Technology (ICEPT)

### 文献[4]参考文献节摘录（原文顺序，轻度清理）
1. Wu, F.; Tian, H.; Shen, Y.; Hou, Z.; Ren, J.; Gou, G.; Sun, Y.; Yang, Y.; Ren, T.-L. Vertical MoS2 Transistors with Sub-1-Nm Gate
2.
3.
4.
5.
6.
Lengths. Nature 2022, 603, 259–264. [CrossRef] [PubMed]
Breton, M.A.; Schmidt, D.; Greene, A.; Frougier, J.; Felix, N. Review of Nanosheet Metrology Opportunities for Technology
Readiness. J. Micro/Nanopatterning Mater. Metrol. 2022, 21, 021206. [CrossRef]
Karimi, K.; Fardoost, A.; Javanmard, M. Comprehensive Review of FinFET Technology: History, Structure, Challenges, Innova-
tions, and Emerging Sensing Applications. Micromachines 2024, 15, 1187. [CrossRef]
Praful, P.; Bailey, C. Warpage in Wafer-Level Packaging: A Review of Causes, Modelling, and Mitigation Strategies. Front. Electron.
2025, 5, 1515860. [CrossRef]
Lu, K.; Lin, P.; Chun, H.; Kim, B.; Nomura, M.; Park, J.; Lee, C. A Review of Through-Silicon Via Inspection and Metrology
Technology for Advanced Semiconductor Packaging. J. Manuf. Sci. Eng. 2025, 147, 121005. [CrossRef]
Raimondi, P.; Benabderrahmane, C.; Berkvens, P.; Biasci, J.C.; Borowiec, P.; Bouteille, J.-F.; Brochard, T.; Brookes, N.B.; Carmignani,
N.; Carver, L.R.; et al. The Extremely Brilliant Source Storage Ring of the European Synchrotron Radiation Facility. Commun. Phys.
2023, 6, 82. [CrossRef]
8.
7. Muthinti, G.R.; Loubet, N.; Chao, R.; De La Peña, A.A.; Li, J.; Guillorn, M.A.; Yamashita, T.; Kanakasabapathy, S.; Gaudiello, J.;
Cepler, A.J.; et al. Proceedings of the Materials Characterization for Process Integration of Multi-Channel Gate All around (GAA) Devices,
San Jose, CA, USA, 31 March 2017; Sanchez, M.I., Ukraintsev, V.A., Eds.; SPIE: Bellingham, WA, USA, 2017; p. 101451U.
Schulze, A.; Loo, R.; Ryan, P.; Wormington, M.; Favia, P.; Witters, L.; Collaert, N.; Bender, H.; Vandervorst, W.; Caymax, M.
Observation and Understanding of Anisotropic Strain Relaxation in Selectively Grown SiGe Fin Structures. Nanotechnology 2017,
28, 145703. [CrossRef]
Schmidt, D.; Durfee, C.; Li, J.; Loubet, N.; Cepler, A.; Neeman, L.; Meir, N.; Ofek, J.; Oren, Y.; Fishman, D. In-Line Raman
Spectroscopy for Gate-All-around Nanosheet Device Manufacturing. J. Micro/Nanopatterning Mater. Metrol. 2022, 21, 021203.
[CrossRef]
9.
10. Yao, Y.-J.; Yang, C.-R.; Tseng, T.-Y.; Chang, H.-J.; Lin, T.-J.; Luo, G.-L.; Hou, F.-J.; Wu, Y.-C.; Chang-Liao, K.-S. High-Performance P-
and N-Type SiGe/Si Strained Super-Lattice FinFET and CMOS Inverter: Comparison of Si and SiGe FinFET. Nanomaterials 2023,
13, 1310. [CrossRef]
11. Liu, H.; Zeng, F.; Tang, G.; Wang, G.; Song, C.; Pan, F. Significant Enhancement in Electromigration Resistance and Texture of
12.
13.
Aluminum Films Using an Ultrathin Titanium Underlayer. Acta Mater. 2013, 61, 4619–4624. [CrossRef]
Sun, J.-Y.; Lee, H.-R.; Hwan Oh, K. Columnar Grown Copper Films on Polyimides Strained beyond 100%. Sci. Rep. 2015, 5, 13791.
[CrossRef]
Feng, X.; Yu, N.; Hang, T.; Zhang, Y.; Li, M. Experimental and Theoretical Study on Self-Annealing Behavior of Copper Film
Electroplated with 2-Mercaptopyridine and 2-Aminobenzothiazole as Additives. J. Electrochem. Soc. 2016, 163, D57–D62.
[CrossRef]
14. Zhang, M.; Gao, L.-Y.; Wang, Y.-X.; Dong, W.; Zhao, N.; Liu, Z.-Q.; Sun, R. Thermal Stability of Electroplated Cu Films with
Different Microstructure by Annealing Treatment. In Proceedings of the 2022 23rd International Conference on Electronic Packaging
Technology (ICEPT), Dalian, China, 10 August 2022; IEEE: New York, NY, USA, 2022; pp. 1–5.
15. Zoellner, M.H.; Richard, M.-I.; Chahine, G.A.; Zaumseil, P.; Reich, C.; Capellini, G.; Montalenti, F.; Marzegalli, A.; Xie, Y.-H.;
Schülli, T.U.; et al. Imaging Structure and Composition Homogeneity of 300 Mm SiGe Virtual Substrates for Advanced CMOS
Applications by Scanning X-Ray Diffraction Microscopy. ACS Appl. Mater. Interfaces 2015, 7, 9031–9037. [CrossRef]
16. Wong, C.S.; Bennett, N.S.; Manessis, D.; Danilewsky, A.; McNally, P.J. Non-Destructive Laboratory-Based X-Ray Diffraction
Mapping of Warpage in Si Die Embedded in IC Packages. Microelectron. Eng. 2014, 117, 48–56. [CrossRef]
17. Mochizuki, S.; Murray, C.E.; Madan, A.; Pinto, T.; Wang, Y.-Y.; Li, J.; Weng, W.; Jagannathan, H.; Imai, Y.; Kimura, S.; et al.
Quantification of Local Strain Distributions in Nanoscale Strained SiGe FinFET Structures. J. Appl. Phys. 2017, 122, 135705.
[CrossRef]
Shida, K.; Takeuchi, S.; Tohei, T.; Imai, Y.; Kimura, S.; Schulze, A.; Caymax, M.; Sakai, A. Depth-Resolved Analysis of Lattice
Distortions in High-Ge-Content SiGe/Compositionally Graded SiGe Films Using Nanobeam X-Ray Diffraction. Semicond. Sci.
Technol. 2018, 33, 124005. [CrossRef]
18.
20.
19. Okoro, C.; Levine, L.E.; Xu, R.; Hummler, K.; Obeng, Y.S. Nondestructive Measurement of the Residual Stresses in Copper
Through-Silicon Vias Using Synchrotron-Based Microbeam X-Ray Diffraction. IEEE Trans. Electron. Devices 2014, 61, 2473–2479.
[CrossRef]
Jiang, T.; Wu, C.; Tamura, N.; Kunz, M.; Kim, B.G.; Son, H.-Y.; Suh, M.-S.; Im, J.; Huang, R.; Ho, P.S. Study of Stresses and Plasticity
in Through-Silicon Via Structures for 3D Interconnects by X-Ray Micro-Beam Diffraction. IEEE Trans. Device Mater. Reliab. 2014,
14, 698–703. [CrossRef]
Song, M.; Mundboth, K.R.; Szpunar, J.A.; Chen, L.; Feng, R. Characterization of Local Strain/Stress in Copper through-Silicon
via Structures Using Synchrotron X-Ray Microdiffraction, Electron Backscattered Diffraction and Nonlinear Thermomechanical
Model. J. Micromech. Microeng. 2015, 25, 085002. [CrossRef]
21.
22. McNally, P.J. B-Spline X-Ray Diffraction Imaging Techniques for Die Warpage and Stress Monitoring inside Fully Encapsulated
Packaged Chips. In Proceedings of the 2015 16th International Conference on Thermal, Mechanical and Multi-Physics Simulation and
Experiments in Microelectronics and Microsystems, Budapest, Hungary, 19–22 April 2015; IEEE: New York, NY, USA, 2015; pp. 1–3.
23. Cowley, A.; Ivankovic, A.; Wong, C.S.; Bennett, N.S.; Danilewsky, A.N.; Gonzalez, M.; Cherman, V.; Vandevelde, B.; De Wolf,
I.; McNally, P.J. B-Spline X-Ray Diffraction Imaging—Rapid Non-Destructive Measurement of Die Warpage in Ball Grid Array
Packages. Microelectron. Reliab. 2016, 59, 108–116. [CrossRef]
24. Kim, J.; Seo, O.; Song, C.; Hiroi, S.; Chen, Y.; Irokawa, Y.; Nabatame, T.; Koide, Y.; Sakata, O. Mapping of a Lattice-Plane Tilting in
a Ga N Wafer Using Energy-Resolved X-Ray Diffraction Topography. Phys. Rev. Appl. 2019, 11, 024072. [CrossRef]
25. Xiong, G.; Moutanabbir, O.; Reiche, M.; Harder, R.; Robinson, I. Coherent X-Ray Diffraction Imaging and Characterization of
Strain in Silicon-on-Insulator Nanostructures. Adv. Mater. 2014, 26, 7747–7763. [CrossRef]
26. Hruszkewycz, S.O.; Allain, M.; Holt, M.V.; Murray, C.E.; Holt, J.R.; Fuoss, P.H.; Chamard, V. High-Resolution Three-Dimensional
Structural Microscopy by Single-Angle Bragg Ptychography. Nat. Mater. 2017, 16, 244–251. [CrossRef]
27. Deng, J.; Hong, Y.P.; Chen, S.; Nashed, Y.S.G.; Peterka, T.; Levi, A.J.F.; Damoulakis, J.; Saha, S.; Eiles, T.; Jacobsen, C. Nanoscale
X-Ray Imaging of Circuit Features without Wafer Etching. Phys. Rev. B 2017, 95, 104111. [CrossRef]
28. Li, P.; Phillips, N.W.; Leake, S.; Allain, M.; Hofmann, F.; Chamard, V. Revealing Nano-Scale Lattice Distortions in Implanted
Material with 3D Bragg Ptychography. Nat. Commun. 2021, 12, 7059. [CrossRef]
29. Bachmann, F.; Bale, H.; Gueninchault, N.; Holzner, C.; Lauridsen, E.M. 3D Grain Reconstruction from Laboratory Diffraction
Contrast Tomography. J. Appl. Crystallogr. 2019, 52, 643–651. [CrossRef] [PubMed]
30. Bieler, T.R.; Wang, L.; Beaudoin, A.J.; Kenesei, P.; Lienert, U. In Situ Characterization of Twin Nucleation in Pure Ti Using 3D-XRD.
Met. Mater. Trans. A 2014, 45, 109–122. [CrossRef]
31. Heller, L.; Karafíto , I.; Petrich, L.; Pawlas, Z.; Shayanfard, P.; Beneš, V.; Schmidt, V.; Šittner, P. Numerical Microstructure Model
of NiTi Wire Reconstructed from 3D-XRD Data. Model. Simul. Mater. Sci. Eng. 2020, 28, 055007. [CrossRef]
32. Radamson, H.H.; Miao, Y.; Zhou, Z.; Wu, Z.; Kong, Z.; Gao, J.; Yang, H.; Ren, Y.; Zhang, Y.; Shi, J.; et al. CMOS Scaling for the
33.
34.
5 Nm Node and Beyond: Device, Process and Technology. Nanomaterials 2024, 14, 837. [CrossRef] [PubMed]
Jones, R.L.; Hu, T.; Lin, E.K.; Wu, W.-L.; Kolb, R.; Casa, D.M.; Bolton, P.J.; Barclay, G.G. Small Angle X-Ray Scattering for
Sub-100 Nm Pattern Characterization. Appl. Phys. Lett. 2003, 83, 4059–4061. [CrossRef]
Sasaki, K.; Hashimoto, T.; Kuo, Y.; Tsukada, H.; Tanizaki, H. Measurability Analysis of the HAR Structure in 3D Memory by
T-SAXS Simulation. In Proceedings of the Metrology, Inspection, and Process Control for Semiconductor Manufacturing XXXV, Online
Only, USA, 22 February 2021; Adan, O., Robinson, J.C., Eds.; SPIE: Bellingham, WA, USA, 2021; p. 25.
35. Tsuji, Y.; Kim, D.; Yoo, G.; Hwang, B.; Kim, K.; Lee, D.; Sasai, Y.; Yi, S.; Jeong, J.; Ihm, D.; et al. Small Angle X-Ray Scattering
(SAXS) and Q-Space Weighting Filter for ×3 CD-Extraction Accuracy Improvement. AIP Adv. 2021, 11, 065129. [CrossRef]
v́
36. Lin, Y.-Y.; Lee, T.-J.; Su, H.-F.; Liu, Y.-H.; Cheng, C.-Y.; Liman, C.; Chen, B.; Tan, Z.; Wu, M.-T.; Huang, M.-H.; et al. Global Tilt
Measurement on Irregular PIL Supporting Patterns in 3D NAND Memory. In Proceedings of the Metrology, Inspection, and Process
Control XXXVIII, San Jose, CA, USA, 10 April 2024; Sendelbach, M.J., Schuch, N.G., Eds.; SPIE: Bellingham, WA, USA, 2024; p. 106.
37. Lin, Y.-Y.; Lee, T.-J.; Su, H.-F.; Liu, Y.-H.; Cheng, C.-Y.; Liman, C.; Chen, B.; Tan, Z.; Chiu, Y.-C.; Huang, C.-K.; et al. Global
Tilt Extraction for BEOL Contact Landing Displacement Control. In Proceedings of the Metrology, Inspection, and Process Control
XXXVIII, San Jose, CA, USA, 10 April 2024; Sendelbach, M.J., Schuch, N.G., Eds.; SPIE: Bellingham, WA, USA, 2024; p. 109.
Fan, M.; Ranjit, R.; Thurber, A.; Engelhard, D. High Resolution Profiles of 3D NAND Pillars Using X-Ray Scattering Metrology. In
Proceedings of the Metrology, Inspection, and Process Control for Semiconductor Manufacturing XXXV, Online Only, USA, 22 February
2021; Adan, O., Robinson, J.C., Eds.; SPIE: Bellingham, WA, USA, 2021; p. 23.
Suenaga, R.; Ito, Y.; Goto, T.; Omote, K. Non-Destructive Sub-Nanometer Evaluation of Sidewall Coverage in Deep Holes by
Small-Angle x-Ray Scattering. In Proceedings of the Metrology, Inspection, and Process Control XXXIX, San Jose, CA, USA, 24 April
2025; Sendelbach, M.J., Schuch, N.G., Eds.; SPIE: Bellingham, WA, USA, 2025; p. 100.
39.
38.
40. Wu, W.; Joseph Kline, R.; Jones, R.L.; Lee, H.-J.; Lin, E.K.; Sunday, D.F.; Wang, C.; Hu, T.; Soles, C.L. Review of the Key Milestones
in the Development of Critical Dimension Small Angle X-Ray Scattering at National Institute of Standards and Technology. J.
Micro/Nanopatterning Mater. Metrol. 2023, 22, 031206. [CrossRef]
Institute of Electrical and Electronics Engineers. IEEE International Roadmap for Devices and Systems, “Metrology”; Institute of
Electrical and Electronics Engineers: New York, NY, USA, 2024.
41.
42. Wormington, M.; Ginsburg, A.; Reichental, I.; Dikopoltsev, A.; Krokhmal, A.; Vinshtein, Y.; Ryan, P.; Korlahalli, R.; Wong, F.;
Rabello, S.; et al. X-Ray Critical Dimension Metrology Solution for High Aspect Ratio Semiconductor Structures. In Proceedings of
the Metrology, Inspection, and Process Control for Semiconductor Manufacturing XXXV, Online Only, USA, 22 February 2021; Adan, O.,
Robinson, J.C., Eds.; SPIE: Bellingham, WA, USA, 2021; p. 27.
43. Dhungana, N.; Bryan, M.; Gergaud, P.; Quéméré, P.; Freychet, G. An Open-Source CD-SAXS Library Framework for Parallelized
Calculations to Facilitate the Modeling and Uncertainty Calculations of Complex Material Stacks. In Proceedings of the Metrology,
Inspection, and Process Control XXXIX, San Jose, CA, USA, 24 April 2025; Sendelbach, M.J., Schuch, N.G., Eds.; SPIE: Bellingham,
WA, USA, 2025; p. 31.
44. Baranovskiy, A.; Grinberg, I.; Greene, M.G.; Amasay, Y.; Wormington, M. Deep Learning for the Analysis of X-Ray Scattering
Data from High-Aspect Ratio Structures. In Proceedings of the Metrology, Inspection, and Process Control XXXVII, San Jose, CA, USA,
27 April 2023; Robinson, J.C., Sendelbach, M.J., Eds.; SPIE: Bellingham, WA, USA, 2023; p. 123.
45. Ekmekci, C.; Cetin, M. Uncertainty Quantification for Deep Unrolling-Based Computational Imaging. IEEE Trans. Comput.
Imaging 2022, 8, 1195–1209. [CrossRef]
46. Mahadevapuram, N.; Strzalka, J.; Stein, G.E. Grazing-incidence Transmission Small Angle X-ray Scattering from Thin Films of
Block Copolymers. J. Polym. Sci. B Polym. Phys. 2013, 51, 602–610. [CrossRef]
47. Hori, Y.; Gonda, S. Error Investigation for SI Traceable Pitch Calibration of One-Dimensional Grating by Grazing-Incidence
48.
Small-Angle X-Ray Scattering. Measurement 2024, 225, 114036. [CrossRef]
Freychet, G.; Rademaker, G.; Blancquaert, Y.; Gergaud, P. Reconstruction of the In-Depth Profile of Line Gratings with Critical
Dimension Grazing Incidence Small Angle x-Ray Scattering on Laboratory Equipment. J. Micro/Nanopatterning Mater. Metrol.
2023, 22, 031210. [CrossRef]
49. Hallstedt, J.; Espes, E.; Lundström, U.; Hallstedt, B.; Hemberg, O.; Otendal, M.; Tuohimaa, T.; Takman, P. METALJET Source for in
Situ SAXS Studies in the Home Laboratory. Acta Crystallogr. A Found. Adv. 2017, 73, C687. [CrossRef]
50. Zaumseil, P. X-Ray Reflectivity Characterisation of Thin-Film and Multilayer Structures. In Materials for Information Technology;
51.
Zschech, E., Whelan, C., Mikolajick, T., Eds.; Engineering Materials and Processes; Springer: London, UK, 2005; pp. 497–505.
Seth, A.; Kaushik, D.; Ghosh, S.K. X-Ray Scatterings to Probe the Structure and Assembly of Biomimetic Membranes. Eur. Phys. J.
Spec. Top. 2024, 233, 2941–2963. [CrossRef]
52. Pan, J. Synchrotron X-Ray Techniques for In Situ or Microscopic Study of Passive Films on Industrial Alloys: A Mini Review.
Corros. Mater. Degrad. 2025, 6, 56. [CrossRef]
53. Mezger, M.; Jérôme, B.; Kortright, J.B.; Valvidares, M.; Gullikson, E.M.; Giglia, A.; Mahne, N.; Nannarone, S. Molecular Orientation
in Soft Matter Thin Films Studied by Resonant Soft X-Ray Reflectivity. Phys. Rev. B 2011, 83, 155406. [CrossRef]
54. Bogdanowicz, J.; Mingardi, A.; Brissonneau, V.; Loo, R.; Shimura, Y.; Akula, A.; Gowda, P.P.; Zhou, D.; Horiguchi, N.; Biesemans,
S.; et al. Inline X-Ray Metrology for Complementary Field-Effect Transistors (CFET). In Proceedings of the Metrology, Inspection,
and Process Control XXXIX, San Jose, CA, USA, 24 April 2025; Sendelbach, M.J., Schuch, N.G., Eds.; SPIE: Bellingham, WA, USA,
2025; p. 48.
55. Pang, X.; Yu, P.; Shang, C.; Chen, B.; Yin, Y.; Chen, X.; Zhang, J.; Wong, T.; Li, Z.; Hong, F.; et al. Thin Film Metrology Techniques:
X-Ray Diffraction and x-Ray Reflectivity. In Proceedings of the Ninth International Workshop on Advanced Patterning Solutions (IWAPS
2025), Shenzhen, China, 3 December 2025; Ye, T., Wei, Y., Eds.; SPIE: Bellingham, WA, USA, 2025; p. 36.
56. Li, X.; Tang, H.; Zhao, J.; Li, F. Research Progress of Beyond Extreme Ultraviolet Multilayers at 6.X nm. Chin. J. Laser 2024,
51, 0701010. [CrossRef]
57. Perros, A.P.; Sippola, P.; Arduca, E.; Johansson, L.-S.; Lipsanen, H. Low Temperature and High Quality Atomic Layer Deposition
HfO2 Coatings. In Proceedings of the 2017 IMAPS Nordic Conference on Microelectronics Packaging (NordPac), Gothenburg, Sweden,
18–20 June 2017; IEEE: New York, NY, USA, 2017; pp. 182–185.
58. Paul, P.; Brusaterra, E.; Ostermay, I.; Bahat Treidel, E.; Brunner, F.; Mogilatenko, A.; Udas, K.; Boschker, J.; Hilt, O.; Krüger, O.
Plasma Enhanced Atomic Layer Deposition of HfO2—A Potential Gate Dielectric for GaN-Based Devices. J. Vac. Sci. Technol. A
2025, 43, 042406. [CrossRef]
59. Barman, A.; Saini, C.P.; Sarkar, P.K.; Roy, A.; Satpati, B.; Kanjilal, D.; Ghosh, S.K.; Dhar, S.; Kanjilal, A. Probing Electron Density
across Ar+ Irradiation-Induced Self-Organized TiO2−x Nanochannels for Memory Application. Appl. Phys. Lett. 2016, 108, 244104.
[CrossRef]
60. Gaudiello, J.; Emans, S.; Shifrin, M.; Etzioni, Y.; Urenski, R.; Lee, W.T.; Breton, M.; Chao, R.; Muthinti, G.R.; De La Pena, A.A.; et al.
Electrical Test Prediction Using Hybrid Metrology and Machine Learning. In Proceedings of the Metrology, Inspection, and Process
Control for Microlithography XXXI, San Jose, CA, USA, 12 April 2017; Sanchez, M.I., Ukraintsev, V.A., Eds.; SPIE: Bellingham, WA,
USA, 2017; p. 3.
61. Liao, S.; Mo, Z.; Zeng, M.; Wu, J.; Gu, Y.; Li, G.; Quan, G.; Lv, Y.; Liu, L.; Yang, C.; et al. Fast and Low-Dose Medical Imaging
Generation Empowered by Hybrid Deep-Learning and Iterative Reconstruction. Cell Rep. Med. 2023, 4, 101119. [CrossRef]
62. Pithan, L.; Starostin, V.; Mareˇcek, D.; Petersdorf, L.; Völter, C.; Munteanu, V.; Jankowski, M.; Konovalov, O.; Gerlach, A.;
Hinderhofer, A.; et al. Closing the Loop: Autonomous Experiments Enabled by Machine-Learning-Based Online Data Analysis in
Synchrotron Beamline Environments. J. Synchrotron Radiat. 2023, 30, 1064–1075. [CrossRef] [PubMed]
Schumi-Mareˇcek, D.; Bertram, F.; Mikulík, P.; Varshney, D.; Novák, J.; Kowarik, S. Millisecond X-Ray Reflectometry and Neural
Network Analysis: Unveiling Fast Processes in Spin Coating. J. Appl. Crystallogr. 2024, 57, 314–323. [CrossRef] [PubMed]
64. Carlton, H.D.; Elmer, J.W.; Li, Y.; Pacheco, M.; Goyal, D.; Parkinson, D.Y.; MacDowell, A.A. Using Synchrotron Radiation
Microtomography to Investigate Multi-Scale Three-Dimensional Microelectronic Packages. J. Vis. Exp. 2016, e53683. [CrossRef]
65. Gluch, J.; Löffler, M.; Meyendorf, N.; Oppermann, M.; Röllig, M.; Sättler, P.; Wolter, K.J.; Zschech, E. Multi-Scale Radiographic
63.
66.
Applications in Microelectronic Industry. AIP Conf. Proc. 2016, 1706, 020026. [CrossRef]
Scott, C.C.; Farrier, M.; Li, Y.; Laxer, S.; Ravi, P.; Kenesei, P.; Wojcik, M.J.; Miceli, A.; Karim, K.S. High-Energy Micrometre-Scale
Pixel Direct Conversion X-Ray Detector. J. Synchrotron Radiat. 2021, 28, 1081–1089. [CrossRef]
67. Rösner, B.; Finizio, S.; Koch, F.; Döring, F.; Guzenko, V.A.; Langer, M.; Kirk, E.; Watts, B.; Meyer, M.; Loroña Ornelas, J.; et al. Soft
X-Ray Microscopy with 7 Nm Resolution. Optica 2020, 7, 1602. [CrossRef]
68. Aidukas, T.; Phillips, N.W.; Diaz, A.; Poghosyan, E.; Müller, E.; Levi, A.F.J.; Aeppli, G.; Guizar-Sicairos, M.; Holler, M. High-
Performance 4-Nm-Resolution X-Ray Tomography Using Burst Ptychography. Nature 2024, 632, 81–88. [CrossRef]
69. Cesar Da Silva, J.; Pacureanu, A.; Yang, Y.; Bohic, S.; Morawe, C.; Barrett, R.; Cloetens, P. Efficient Concentration of High-Energy
X-Rays for Diffraction-Limited Imaging Resolution. Optica 2017, 4, 492. [CrossRef]
70. Yan, H.; Bouet, N.; Zhou, J.; Huang, X.; Nazaretski, E.; Xu, W.; Cocco, A.P.; Chiu, W.K.S.; Brinkman, K.S.; Chu, Y.S. Multimodal
Hard X-Ray Imaging with Resolution Approaching 10 Nm for Studies in Material Science. Nano Futures 2018, 2, 011001. [CrossRef]
71. Dreier, T.; Nilsson, D.; Hållstedt, J.; Hu, S. Improved Resolution in Advanced Packaging Metrology Through Advanced Nano-
Focus X-Ray Sources. In Proceedings of the 2024 25th International Conference on Electronic Packaging Technology (ICEPT),
Tianjin, China, 7–9 August 2024; pp. 1–3.
72. Bryant, K.; Eng, B. New X-Ray Tubes for Wafer Level Inspection. In Proceedings of the 2020 International Wafer Level Packaging
Conference (IWLPC), San Jose, CA, USA, 13–30 October 2020; pp. 1–6.
73. Lechowski, B.; Kutukova, K.; Grenzer, J.; Panchenko, I.; Krueger, P.; Clausner, A.; Zschech, E. Laboratory X-Ray Microscopy of 3D
Nanostructures in the Hard X-Ray Regime Enabled by a Combination of Multilayer X-Ray Optics. Nanomaterials 2024, 14, 233.
[CrossRef] [PubMed]
74. Kutukova, K.; Lechowski, B.; Grenzer, J.; Krueger, P.; Clausner, A.; Zschech, E. Laboratory High-Contrast X-Ray Microscopy of
Copper Nanostructures Enabled by a Liquid-Metal-Jet X-Ray Source. Nanomaterials 2024, 14, 448. [CrossRef] [PubMed]
75. Batey, D.J.; Van Assche, F.; Vanheule, S.; Boone, M.N.; Parnell, A.J.; Mykhaylyk, O.O.; Rau, C.; Cipiccia, S. X-Ray Ptychography
with a Laboratory Source. Phys. Rev. Lett. 2021, 126, 193902. [CrossRef]
76. Chen, Y. Recent Progress in Nanofabrication of High Resolution X-Ray Zone Plate Lenses by Electron Beam Lithography. Acta
Opt. Sin. 2022, 42, 1134005. [CrossRef]
77. Li, Y.; Lu, W.; Wang, S.; Yuan, Q.; Kong, X.; Han, L.; Xia, Y. Fabrication of Multilayer Fresnel Zone Plate for Hard X-Ray Microscopy
by Atomic Layer Deposition and Focused Ion Beam Milling. Vacuum 2023, 209, 111776. [CrossRef]
78. Lau, S.H.; Gul, S.; Zan, G.; Vine, D.; Lewis, S.; Yun, W. Defect Characterization of Advanced Packages Using Novel Phase and
Dark Field X-Ray Imaging. EDFA Tech. Artic. 2020, 22, 18–25. [CrossRef]
79. Gelb, J.; Gul, S.; Zheng, C.; Singh, V.; Adibhatla, A.; Lau, S.; Lewis, S.; Yun, W. Dual-Mode 3D X-Ray Imaging for Failure Analysis
of Complex Semiconductor Packages. In Proceedings of the International Symposium for Testing and Failure Analysis, Pasadena, CA,
USA, 16 November 2025; ASM International: Novelty, OH, USA, 2025; Volume 85212, pp. 335–342.
80. Lau, S.H.; Gelb, J.; Gul, S.; Rowland, D.; Qin, T.; Zheng, C.; Singh, V.; Lewis, S.; Yun, W. Next-Gen Failure Analysis: 3D X-Ray
Imaging at 350 Nm Meets Laminography. In Proceedings of the 2025 IEEE 32nd International Symposium on the Physical and Failure
Analysis of Integrated Circuits (IPFA), Bayan Lepas, Malaysia, 5–8 August 2025; IEEE: New York, NY, USA, 2025; pp. 1–6.
81. Nikitin, V.; Mittone, A.; Clark, S.J.; Fezzaa, K.; Wojcik, M.; Deriy, A.; Bean, S.; De Carlo, F. Nano-Laminography with a Transmission
X-Ray Microscope. J. Synchrotron Radiat. 2025, 32, 1452–1462. [CrossRef]
82. Khan, M.S.M.; Xi, C.; Haque, M.S.U.; Tehranipoor, M.M.; Asadizanjani, N. Exploring Advanced Packaging Technologies for
Reverse Engineering a System-in-Package (SiP). IEEE Trans. Compon. Packag. Manuf. Technol. 2023, 13, 1360–1370. [CrossRef]
83. Wen Lee, X.; Zulkifli, S.; Zee, B. Enabling Advanced Packaging Defect Inspection Using X-Ray Computed Laminography Imaging
Technique. In Proceedings of the 2025 IEEE 32nd International Symposium on the Physical and Failure Analysis of Integrated Circuits
(IPFA), Bayan Lepas, Malaysia, 5 August 2025; IEEE: New York, NY, USA, 2025; pp. 1–5.
84. Chery, E.; Duval, F.F.C.; Stucchi, M.; Slabbekoorn, J.; Croes, K.; Beyne, E. Reliability Study of Polymers Used in Sub-4-Mm Pitch
85.
RDL Applications. IEEE Trans. Compon. Packag. Manuf. Technol. 2021, 11, 1073–1080. [CrossRef]
Shafkat, M.; Khan, M.; Xi, C.; Varshney, N.; Khan, A.A.; Dalir, H.; Asadizanjani, N. Assessing Compatibility of Advanced IC
Packages to X-Ray Based Physical Inspection. EDFA Tech. Artic. 2024, 26, 14–24. [CrossRef]
86. Lin, Y.-S.; Liu, C.-H.; Wang, C.-C.; Hung, C.-P.; Kuo, C.-L.; Hung, C.-W. Novel Fault Isolation Methodology Applied on Nanoscale
Defect in Fine Line RDL for Advanced Fan-Out Package. In Proceedings of the 2025 IEEE 75th Electronic Components and Technology
Conference (ECTC), Dallas, TX, USA, 27 May 2025; IEEE: New York, NY, USA, 2025; pp. 1943–1947.
87. Liu, C.-H.; Chang, Y.-J.; Hsiao, Y.-H.; Lin, Y.-S. 3D X-Ray Microscope Applied on Fine-Line Inspection of Fan-Out Packages. In
Proceedings of the 2022 International Conference on Electronics Packaging (ICEP), Sapporo, Japan, 11 May 2022; IEEE: New York, NY,
USA, 2022; pp. 199–200.
88. Huang, C.-J.; Hsiao, Y.-H.; Lin, Y.-S.; Liu, C.-H. A Special Holding System for Large Package in 3D X-Ray Inspection. In Proceedings
of the 2024 International Conference on Electronics Packaging (ICEP), Toyama, Japan, 17 April 2024; IEEE: New York, NY, USA, 2024;
pp. 231–232.
89. Li, S.; Frame, J.; Madriaga-Berry, E.; Hulog, J.; Zhang, M.; Terada, M.; Gu, A.; Taraci, D. Detecting Wafer-Level Cu Pillar Defects
Using Advanced 3D X-Ray Microscopy (XRM) with Submicron Resolution. J. Fail. Anal. Prev. 2024, 24, 2232–2239. [CrossRef]
90. Dreier, T.; Nilsson, D.; Hållstedt, J. Fast and High-Resolution X-Ray Nano Tomography for Failure Analysis in Advanced
Packaging. Microelectron. Reliab. 2025, 168, 115694. [CrossRef]
91. Lin, T.-W.; Shie, K.-C.; Chen, C.; Tu, K.-N. Study of Electromigration of Solder Microbumps by 3D X-Ray Microscopy. In
Proceedings of the 2020 15th International Microsystems, Packaging, Assembly and Circuits Technology Conference (IMPACT), Taipei,
Taiwan, 21 October 2020; IEEE: New York, NY, USA, 2020; pp. 76–78.
Shie, K.-C.; Lin, T.-W.; Tu, K.N.; Chen, C. Non-Destructive Observation of Void Formation Due to Electromigration in Solder
Microbump by 3D Xray. In Proceedings of the 2021 IEEE 71st Electronic Components and Technology Conference (ECTC), San Diego, CA,
USA, 1–4 July 2021; IEEE: New York, NY, USA, 2021; pp. 925–930.
92.
93. Chen, Y.; Lai, P.; Huang, H.-Z.; Zhang, P.; Lin, X. Open Localization in 3D Package with TSV Daisy Chain Using Magnetic Field
Imaging and High-Resolution Three-Dimensional X-Ray Microscopy. Appl. Sci. 2021, 11, 8148. [CrossRef]
94. Wolz, B.C.; Jaremenko, C.; Vollnhals, F.; Kling, L.; Wrege, J.; Christiansen, S. X-ray Microscopy and Automatic Detection of Defects
in through Silicon Vias in Three-dimensional Integrated Circuits. Eng. Rep. 2022, 4, e12520. [CrossRef]
95. Wang, X.; Van Nhat Anh, T. High Aspect Ratio >10 TSV Design and Integration Challenges and Solutions for the Multi Memory
Stacking. In Proceedings of the 2024 IEEE 26th Electronics Packaging Technology Conference (EPTC), Singapore, 3 December 2024; IEEE:
New York, NY, USA, 2024; pp. 135–138.
96. Li, K.; Deng, B.; Zhang, H.; Yu, F.; Xue, Y.; Xie, C.; Ye, T.; Xiao, T. Comprehensive Characterization of TSV Etching Performance
with Phase-Contrast X-Ray Microtomography. J. Synchrotron Radiat. 2020, 27, 1023–1032. [CrossRef]
97. Holler, M.; Guizar-Sicairos, M.; Tsai, E.H.R.; Dinapoli, R.; Müller, E.; Bunk, O.; Raabe, J.; Aeppli, G. High-Resolution Non-
Destructive Three-Dimensional Imaging of Integrated Circuits. Nature 2017, 543, 402–406. [CrossRef]
98. Holler, M.; Odstrcil, M.; Guizar-Sicairos, M.; Lebugle, M.; Müller, E.; Finizio, S.; Tinti, G.; David, C.; Zusman, J.; Unglaub, W.; et al.
Three-Dimensional Imaging of Integrated Circuits with Macro- to Nanoscale Zoom. Nat. Electron. 2019, 2, 464–470. [CrossRef]
99. Holler, M.; Guizar-Sicairos, M.; Raabe, J. State-of-the-Art High-Resolution 3D X-Ray Microscopy for Imaging of Integrated
Circuits. EDFA Tech. Artic. 2021, 23, 13–19. [CrossRef]
100. Shimomura, K.; Hirose, M.; Takahashi, Y. Multislice Imaging of Integrated Circuits by Precession X-Ray Ptychography. Acta
Crystallogr. A Found. Adv. 2018, 74, 66–70. [CrossRef] [PubMed]
101. Kang, I.; Wu, Z.; Jiang, Y.; Yao, Y.; Deng, J.; Klug, J.; Vogt, S.; Barbastathis, G. Attentional Ptycho-Tomography (APT) for
Three-Dimensional Nanoscale X-Ray Imaging with Minimal Data Acquisition and Computation Time. Light. Sci. Appl. 2023,
12, 31. [CrossRef]
102. Kang, I.; Yao, Y.; Deng, J.; Klug, J.; Vogt, S.; Honig, S.; Barbastathis, G. Three-Dimensional Reconstruction of Integrated Circuits by
Single-Angle X-Ray Ptychography with Machine Learning. In Proceedings of the OSA Imaging and Applied Optics Congress 2021 (3D,
COSI, DH, ISA, pcAOP); Optica Publishing Group: Washington, DC, USA, 2021; p. CTu6A.4.
103. Guan, Z.; Tsai, E.; Huang, X.; Yager, K.; Qin, H. PtychoNet: Fast and High Quality Phase Retrieval for Ptychography. In
Proceedings of the 30th British Machine Vision Conference (BMVC 2019), Cardiff, UK, 9–12 September 2019.
104. Kang, I.; Jiang, Y.; Holler, M.; Guizar-Sicairos, M.; Levi, A.F.J.; Klug, J.; Vogt, S.; Barbastathis, G. Accelerated Deep Self-Supervised
Ptycho-Laminography for Three-Dimensional Nanoscale Imaging of Integrated Circuits. Optica 2023, 10, 1000. [CrossRef]
105. Pan, X.; Wang, S.; Zhou, Z.; Zhou, L.; Liu, P.; Li, C.; Wang, W.; Zhang, C.; Dong, Y.; Zhang, Y. An Efficient Ptychography
Reconstruction Strategy through Fine-Tuning of Large Pre-Trained Deep Learning Model. iScience 2023, 26, 108420. [CrossRef]
106. Nakahata, R.; Zaman, S.; Zhang, M.; Lu, F.; Chiu, K. PtychoFormer: A Transformer-Based Model for Ptychographic Phase
Retrieval. arXiv 2024, arXiv:2410.17377.
107. Masteghin, M.G.; Gervais, T.; Clowes, S.K.; Cox, D.C.; Zelyk, V.; Pattammattel, A.; Chu, Y.S.; Kolev, N.; Stock, T.J.Z.; Curson, N.J.;
et al. Benchmarking of X-Ray Fluorescence Microscopy with Ion Beam Implanted Samples Showing Detection Sensitivity of
Hundreds of Atoms. Small Methods 2024, 8, 2301610. [CrossRef] [PubMed]
108. An, S.; Krapohl, D.; Norlin, B.; Thungström, G. Full-Field X-Ray Fluorescence Imaging with a Straight Polycapillary X-Ray
Collimator. J. Instrum. 2020, 15, P12033. [CrossRef]
109. Sun, S.; Chen, Z.; Liu, Y.; Ouyang, X.; Li, X. Characterization of a Large-Area Full-Field X-Ray Fluorescence Imaging System
Based on a Commercial Full-Frame CMOS Camera. J. Instrum. 2021, 16, P10031. [CrossRef]
110. Soltau, J.; Meyer, P.; Hartmann, R.; Strüder, L.; Soltau, H.; Salditt, T. Full-Field x-Ray Fluorescence Imaging Using a Fresnel Zone
Plate Coded Aperture. Optica 2023, 10, 127. [CrossRef]
111. Wang, X.; Liao, S.; Chen, L.; Li, J.; Chen, L.; Hei, D. A Compact, Low-Power Total Reflection X-Ray Fluorescence (TXRF)
Spectrometer Designed for Surface Metal Contamination Analysis of Silicon Wafers. Spectrochim. Acta Part B At. Spectrosc. 2026,
235, 107388. [CrossRef]
112. Staeck, S.; Kayser, Y.; Baumann, J.; Jonas, A.; Mantouvalou, I.; Hartmann, R.; Kanngießer, B.; Stiel, H. Towards Soft X-Ray
Fluorescence Measurements in the Laboratory Using a Laser-Produced Plasma Source and a Complementary Metal-Oxide
Semiconductor Detector. J. Instrum. 2021, 16, P03033. [CrossRef]
113. Yim, V.; Mukhtarov, A.; Drogue, N.; Autillo, D.; Lardin, T.; Zussy, M.; Dechamp, J.; Truffier-Boutry, D. TXRF Capability of Metallic
Contamination Analysis on Rough Silicon Wafers. J. Mater. Res. 2024, 39, 2522–2530. [CrossRef]
114. Rotella, H.; Caby, B.; Ménesguen, Y.; Mazel, Y.; Valla, A.; Ingerle, D.; Detlefs, B.; Lépy, M.-C.; Novikova, A.; Rodriguez, G.; et al.
Elemental Depth Profiling in Transparent Conducting Oxide Thin Film by X-Ray Reflectivity and Grazing Incidence X-Ray
Fluorescence Combined Analysis. Spectrochim. Acta Part B At. Spectrosc. 2017, 135, 22–28. [CrossRef]
115. Melhem, S. Reference-Free Combined Analysis GIXRF-XRR for the Characterization of Thin Film Materials and Uncertainties
Calculation. Ph.D. Thesis, Université Paris-Saclay, Orsay, France, 2023.
116. Horiba, K.; Kamakura, N.; Yamamoto, K.; Kobayashi, K.; Shin, S. A High-Resolution Angle-Resolved Photoemission Spectrometer
Combined with Laser Molecular-Beam Epitaxy at SPring-8 BL17SU. J. Electron. Spectrosc. Relat. Phenom. 2005, 144–147, 1027–1030.
[CrossRef]
117. Szczepanik-Ciba, M.; Sobol, T.; Szade, J. PHELIX—A New Soft X-Ray Spectroscopy Beamline at SOLARIS Synchrotron. Nucl.
Instrum. Methods Phys. Res. Sect. B Beam Interact. Mater. At. 2021, 492, 49–55. [CrossRef]
118. Muro, T.; Senba, Y.; Ohashi, H.; Ohkochi, T.; Matsushita, T.; Kinoshita, T.; Shin, S. Soft X-Ray ARPES for Three-Dimensional
Crystals in the Micrometre Region. J. Synchrotron Radiat. 2021, 28, 1631–1638. [CrossRef] [PubMed]
119. Yamagami, K.; Yokoyama, Y.; Sumiya, Y.; Shouno, H.; Nakamura, T.; Mizumaki, M. Development of Ultra-High Efficiency
Soft X-Ray Angle-Resolved Photoemission Spectroscopy Equipped with Deep Prior-Based Denoising Method. arXiv 2025,
arXiv:2511.22909.
120. Spencer, B.F.; Church, S.A.; Thompson, P.; Cant, D.J.H.; Maniyarasu, S.; Theodosiou, A.; Jones, A.N.; Kappers, M.J.; Binks, D.J.;
Oliver, R.A.; et al. Characterization of Buried Interfaces Using Ga Kα Hard X-Ray Photoelectron Spectroscopy (HAXPES). Faraday
Discuss. 2022, 236, 311–337. [CrossRef]
121. Artyushkova, K.; Mann, J.; Zaccarine, S. Analysis of Thin Films and Buried Interfaces by Soft and Hard X-Ray Photoemission.
Microsc. Microanal. 2023, 29, 768. [CrossRef]
122. Thapa, S.; Paudel, R.; Blanchet, M.D.; Gemperline, P.T.; Comes, R.B. Probing Surfaces and Interfaces in Complex Oxide Films via
in Situ X-Ray Photoelectron Spectroscopy. J. Mater. Res. 2021, 36, 26–51. [CrossRef]
123. Huang, H.; Zhao, G.; Xing, S.; Mao, B.; Lv, X.; Liu, G.; Li, X.; Yang, W.; Yang, J. Investigation of Band Alignment at Two-
Dimensional ReS2/XSe2 (X=W, Mo) Heterojunctions Using x-Ray/Ultraviolet Photoelectron Spectroscopy. Phys. Lett. A 2022,
445, 128241. [CrossRef]
124. Henck, H.; Ben Aziza, Z.; Zill, O.; Pierucci, D.; Naylor, C.H.; Silly, M.G.; Gogneau, N.; Oehler, F.; Collin, S.; Brault, J.; et al. Interface
Dipole and Band Bending in the Hybrid p − n Heterojunction MoS2/GaN (0001). Phys. Rev. B 2017, 96, 115312. [CrossRef]
125. Budri, T.; Klatt, J.; Chung, J.; Clubb, A.; Mann, J.; Artyushkova, K. Semiconductor Film Stack Interface Investigation via DSIMS &
TOFSIMS Depth Profiling and HAXPES: Yield Enhancement/Learning. In Proceedings of the 2023 34th Annual SEMI Advanced
Semiconductor Manufacturing Conference (ASMC), Saratoga Springs, NY, USA, 1 May 2023; IEEE: New York, NY, USA, 2023; pp. 1–3.
126. Conti, G.; Perin Martins, H.; Cordova, I.A.; Ma, J.; Wojtecki, R.J.; Naulleau, P.P.; Nemsak, S. Sub-Nm Depth Characterization
of EUV Nanoscale Photoresist Films by Standing-Wave Photoemission Spectroscopy. In Proceedings of the Extreme Ultraviolet
Lithography 2020, Online Only, USA, 10 November 2020; Ronse, K.G., Gargini, P.A., Naulleau, P.P., Itani, T., Eds.; SPIE: Bellingham,
WA, USA, 2020; p. 15.
127. Conti, G.; Martins, H.P.; Cordova, I.A.; Ma, J.; Wojtecki, R.J.; Naulleau, P.; Nemšák, S. Chemical and Structural Characterization of
EUV Photoresists as a Function of Depth by Standing-Wave x-Ray Photoelectron Spectroscopy. J. Micro/Nanopatterning Mater.
Metrol. 2021, 20, 034603. [CrossRef]
128. Martin-Concepción, A.I.; Yubero, F.; Espinos, J.P.; Garcia-Lopez, J.; Tougaard, S. Determination of Amount of Substance for
Nanometre-thin Deposits: Consistency between XPS, RBS and XRF Quantification. Surf. Interface Anal. 2003, 35, 984–990.
[CrossRef]
129. L’Herron, B.; Chao, R.; Kim, K.; Lee, W.T.; Motoyama, K.; Deprospo, B.; Standaert, T.; Gaudiello, J.; Goldberg, C. Hybridization
of XRF/XPS and Scatterometry for Cu CMP Process Control. In Proceeding of the Metrology, Inspection, and Process Control for
Microlithography XXIX, San Jose, CA, USA, 19 March 2015; Cain, J.P., Sanchez, M.I., Eds.; SPIE: Bellingham, WA, USA, 2015;
p. 94241M.
130. Hossain, M.; Subramanian, G.; Triyoso, D.; Wahl, J.; Mcardle, T.; Vaid, A.; Bello, A.F.; Lee, W.T.; Klare, M.; Kwan, M.; et al. XPS-XRF
Hybrid Metrology Enabling FDSOI Process. In Proceeding of the Metrology, Inspection, and Process Control for Microlithography XXX,
San Jose, CA, USA, 24 March 2016; Sanchez, M.I., Ukraintsev, V.A., Eds.; SPIE: Bellingham, WA, USA, 2016; p. 97780N.
131. Kowalczyk, J.M.D.; Madey, J.M.J. Use of Etendue and Energy Spread to Assess Inverse-Compton X-Ray Sources for Applications.
In Proceedings of the High-Brightness Sources and Light-Driven Interactions; OSA: Long Beach, CA, USA, 2016; p. EM1A.1.
132. Turenhout, M.; Mutsaers, P.; Luiten, J. ICS-SAXS: Hard X-Ray Metrology Accelerated by an Inverse Compton Scattering Source.
In Proceedings of the International Symposium on Compact Synchrotron X-Ray Sources, Munchen, Germany, 24–26 June 2024.
133. Digraci, P.; Besacier, M.; Gergaud, P.; Rademaker, G.; Rêche, J. Multi-Branch Neural Network for Hybrid Metrology Improvement.
In Proceedings of the Metrology, Inspection, and Process Control XXXVI, San Jose, CA, USA, 26 May 2022; Robinson, J.C., Sendelbach,
M.J., Eds.; SPIE: Bellingham, WA, USA, 2022; p. 46.
134. Hönicke, P.; Detlefs, B.; Müller, M.; Darlatt, E.; Nolot, E.; Grampeix, H.; Beckhoff, B. Reference-Free, Depth-Dependent Characteri-
zation of Nanolayers and Gradient Systems with Advanced Grazing Incidence X-Ray Fluorescence Analysis: Characterization of
Nanolayers and Gradient Systems. Phys. Status Solidi A 2015, 212, 523–528. [CrossRef]
135. Nolot, E.; Pessoa, W.; Torrengo, S.; Mazel, Y.; Bernard, M.; Gergaud, P.; Ménesguen, Y.; Lépy, M.C.; Eichert, D. Grazing-Incidence
X-Ray Fluorescence Analysis of Thin Chalcogenide Materials Deposited on Bragg Mirrors. Spectrochim. Acta Part B At. Spectrosc.
2020, 168, 105864. [CrossRef]
136. Tiwari, A.; Fallica, R.; Ackermann, M.D.; Makhotkin, I.A. The Interface Study of Photoresist/Underlayer Using Hybrid X-Ray
Reflectivity and X-Ray Standing Wave Approach. In Proceedings of the Metrology, Inspection, and Process Control XXXVIII, San Jose,
CA, USA, 10 April 2024; Sendelbach, M.J., Schuch, N.G., Eds.; SPIE: Bellingham, WA, USA, 2024; p. 4.
137. Fauquier, L.; Pelissier, B.; Jalabert, D.; Pierre, F.; Hartmann, J.M.; Rozé, F.; Doloy, D.; Le Cunff, D.; Beitia, C.; Baron, T. Benefits of
XPS Nanocharacterization for Process Development and Industrial Control of Thin SiGe Channel Layers in Advanced CMOS
Technologies. Mater. Sci. Semicond. Process. 2017, 70, 105–110. [CrossRef]
138. Jang, Y.; Choi, D.; Song, J.K.; Lee, S.; Seong, T.; Lee, H.; Seo, S.; Song, C.; Lan, T.; Zhang, J.; et al. Study of Critical Dimension
Small-Angle X-Ray Scattering within-Spot Uniformity with Mass Critical Dimension Scanning Electron Microscope and 3D
Tomography. J. Micro/Nanopatterning Mater. Metrol. 2025, 24, 034004. [CrossRef]
139. Pasikatan, E.; Antonelli, G.A.; Keller, N.; Kal, S.; Rednor, M.; Tapily, K.; Hetzer, D.; Schaefer, M.; Kuhn, M.; Murakami, S.; et al.
Superlattice Effects and Limitations of Non-Destructive Measurement of Advanced Si/Si1−xGex Superlattice Structures Using
Mueller Matrix Scatterometry and High-Resolution X-Ray Diffraction. J. Micro/Nanopatterning Mater. Metrol. 2024, 23, 044004.
[CrossRef]
140. Deng, B.; Yang, Q.; Xie, H.-L.; Du, G.-H.; Xiao, T.-Q. First X-Ray Fluorescence CT Experimental Results at the SSRF X-Ray Imaging
Beamline. Chin. Phys. C 2011, 35, 402–404. [CrossRef]
141. Laforce, B.; Masschaele, B.; Boone, M.N.; Schaubroeck, D.; Dierick, M.; Vekemans, B.; Walgraeve, C.; Janssen, C.; Cnudde, V.; Van
Hoorebeke, L.; et al. Integrated Three-Dimensional Microanalysis Combining X-Ray Microtomography and X-Ray Fluorescence
Methodologies. Anal. Chem. 2017, 89, 10617–10624. [CrossRef] [PubMed]
142. Mandot, S.; Zannoni, E.M.; Cai, L.; Nie, X.; Rivière, P.J.L.; Wilson, M.D.; Meng, L.J. A High-Sensitivity Benchtop X-Ray
Fluorescence Emission Tomography (XFET) System With a Full-Ring of X-Ray Imaging-Spectrometers and a Compound-Eye
Collimation Aperture. IEEE Trans. Med. Imaging 2024, 43, 1782–1791. [CrossRef] [PubMed]
Disclaimer/Publisher’s Note: The statements, opinions and data contained in all publications are solely those of the individual
author(s) and contributor(s) and not of MDPI and/or the editor(s). MDPI and/or the editor(s) disclaim responsibility for any injury to
people or property resulting from any ideas, methods, instructions or products referred to in the content.

### 文献[5]参考文献节摘录（原文顺序，轻度清理）
1. Munoz, R. Furthering Moore’s Law Integration Benefits in the Chiplet Era. IEEE Des. Test 2024, 41, 81–90. [CrossRef]
2.
Tian, W.; Li, B.; Li, Z.; Cui, H.; Shi, J.; Wang, Y.; Zhao, J. Using Chiplet Encapsulation Technology to Achieve Processing-in-Memory
Functions. Micromachines 2022, 13, 1790. [CrossRef] [PubMed]
Lee, Y.G.; McInerney, M.; Joo, Y.C.; Choi, I.S.; Kim, S.E. Copper Bonding Technology in Heterogeneous Integration. Electron.
Mater. Lett. 2024, 20, 1–25. [CrossRef]
Lau, J.H. Recent Advances and Trends in Advanced Packaging. IEEE Trans. Compon. Packag. Manuf. Technol. 2022, 12, 228–252.
[CrossRef]
Ahmed, O.; Jalilvand, G.; Pollard, S.; Okoro, C.; Jiang, T. The Interfacial Reliability of Through-glass Vias for 2.5D Integrated
Circuits. Microelectron. Int. 2020, 37, 181–188. [CrossRef]
3.
4.
5.
7.
6. Wei, T.; Wang, Q.; Cai, J.; Chen, L.; Huang, J.; Wang, L.; Zhang, L.; Li, C. Performance and Reliability Study of TGV Interposer in
3D Integration. In Proceedings of the 2014 IEEE 16th Electronics Packaging Technology Conference, Singapore, 3–5 December
2014; pp. 601–605.
Okoro, C.; Jayaraman, S.; Pollard, S. Understanding and Eliminating Thermo-mechanically Induced Radial Cracks in Fully
Metallized Through-glass via (TGV) Substrates. Microelectron. Reliab. 2021, 120, 114092. [CrossRef]
Okoro, C.; Allowatt, T.; Pollard, S.; Soc, I.C. Resolving Thermo-Mechanically Induced Circumferential Crack Formation in Copper
Through-Glass Vias. In Proceedings of the 2021 IEEE 71st Electronic Components and Technology Conference, San Diego, CA,
USA, 1 June–4 July 2021; pp. 954–958.
8.
12 of 12
9.
Benali, A.; Faqir, M.; Bouya, M.; Benabdellah, A.; Ghogho, M. Analytical and Finite Element Modeling of Through Glass via
Thermal Stress. Microelectron. Eng. 2016, 151, 12–18. [CrossRef]
10. Demir, K.; Armutlulu, A.; Sundaram, V.; Raj, P.M.; Tummala, R.R. Reliability of Copper Through-Package Vias in Bare Glass
Interposers. IEEE Trans. Compon. Packag. Manuf. Technol. 2017, 7, 829–837. [CrossRef]
11. Vaz, R.F.; Garfias, A.; Albaladejo, V.; Sanchez, J.; Cano, I.G. How Increasing Cold Spray Coatings Thickness Affects Their Residual
12.
Stress and Properties. Surf. Coat. Technol. 2024, 485, 130867. [CrossRef]
Salmi, A.; Atzeni, E.; Iuliano, L.; Galati, M. Experimental analysis of residual stresses on AlSi10Mg parts produced by means of
selective laser melting (SLM). Procedia CIRP 2017, 62, 458–463. [CrossRef]
13. Over, V.; Donovan, J.; Lawrence Yao, Y. The effect of laser shock peening on back stress of additively manufactured stainless steel
parts. J. Manuf. Sci. Eng. 2023, 145, 041005. [CrossRef]
14. Xu, D.; Sriram, V.; Ozolins, V.; Yang, J.M.; Tu, K.N.; Stafford, G.R.; Beauchamp, C. In Situ Measurements of Stress Evolution for
Nanotwin Formation During Pulse Electrodeposition of Copper. J. Appl. Phys. 2009, 105, 023521. [CrossRef]
15. Lu, T.L.; Shen, Y.A.; Wu, J.A.; Chen, C. Anisotropic Grain Growth in (111) Nanotwinned Cu Films by DC Electrodeposition.
Materials 2020, 13, 134. [CrossRef] [PubMed]
16. Xu, D.; Sriram, V.; Ozolins, V.; Yang, J.M.; Tu, K.N.; Stafford, G.R.; Beauchamp, C.; Zienert, I.; Geisler, H.; Hofmann, P.; et al.
Nanotwin Formation and Its Physical Properties and Effect on Reliability of Copper Interconnects. Microelectron. Eng. 2008,
85, 2155–2158. [CrossRef]
17. Hasegawa, M.; Mieszala, M.; Zhang, Y.; Erni, R.; Michler, J.; Philippe, L. Orientation-controlled Nanotwinned Copper Prepared
18.
by Electrodeposition. Electrochim. Acta 2015, 178, 458–467. [CrossRef]
Scardi, P.; Polonioli, P.; Ferrari, S.J.T.S.F. Residual Stress in Stabilized Zirconia Thin Films Prepared by r.f. Magnetron Sputtering.
Thin Solid Film. 1994, 253, 349–355. [CrossRef]
19. Luo, Q.; Jones, A.H. High-precision Determination of Residual Stress of Polycrystalline Coatings Using Optimised XRD-sin2ψ
Technique. Surf. Coat. Technol. 2010, 205, 1403–1408. [CrossRef]
20. Wang, I.J.; Ku, C.S.; Tu, L.; Huang, E.W.; Tu, K.N.; Chen, C. Tuning Stress in Cu Thin Films by Developing Highly (111)-Oriented
Nanotwinned Structure. J. Electron. Mater. 2020, 49, 109–115. [CrossRef]
21. Lin, C.; Hu, C. The Ultrahigh-Rate Growth of Nanotwinned Copper Induced by Thiol Organic Additives. J. Electrochem. Soc. 2020,
167, 082505. [CrossRef]
22. Zhu, Q.; Zhang, X.; Li, S.; Chun, L.; Cai, L. Communication—Electrodeposition of Nano-twinned Cu in Void-free Filling for Blind
Microvia of High Density Interconnect. J. Electrochem. Soc. 2018, 166, D3097. [CrossRef]
23. Hsiao, H.Y.; Liu, C.M.; Lin, H.W.; Liu, T.C.; Lu, C.L.; Huang, Y.S.; Chen, C.; Tu, K.N. Unidirectional Growth of Microbumps on
(111)-Oriented and Nanotwinned Copper. Science 2012, 336, 1007–1010. [CrossRef] [PubMed]
24. Tseng, C.H.; Chen, C. Growth of Highly (111)-Oriented Nanotwinned Cu with the Addition of Sulfuric Acid in CuSO4 Based
Electrolyte. Cryst. Growth Des. 2019, 19, 81–89. [CrossRef]
25. Chan, T.C.; Chueh, Y.L.; Liao, C.N. Manipulating the Crystallographic Texture of Nanotwinned Cu Films by Electrodeposition.
Cryst. Growth Des. 2011, 11, 4970–4974. [CrossRef]
26. Liu, T.C.; Liu, C.M.; Hsiao, H.Y.; Lu, J.L.; Huang, Y.S.; Chen, C. Fabrication and Characterization of (111)-Oriented and
Nanotwinned Cu by Dc Electrodeposition. Cryst. Growth Des. 2012, 12, 5012–5016. [CrossRef]
27. Tseng, C.H.; Tseng, I.H.; Huang, Y.P.; Hsu, Y.T.; Leu, J.; Tu, K.N.; Chen, C. Kinetic Study of Grain Growth in Highly (111)-Preferred
Nanotwinned Copper films. Mater. Charact. 2020, 168, 110545. [CrossRef]
28. Chen, P.; Li, C.; Han, S.; Hang, T.; Ling, H.; Wu, Y.; Li, M. Abnormal Grain Growth of (110)-Oriented Perpendicular Nanotwinned
Copper into Ultra-large Grains at Low Temperatures. J. Mater. Sci. Technol. 2024, 203, 61–65. [CrossRef]
29. Cui, B.Z.; Han, K.; Xin, Y.; Waryoba, D.R.; Mbaruku, A.L. Highly Textured and Twinned Cu Films Fabricated by Pulsed
Electrodeposition. Acta Mater. 2007, 55, 4429–4438. [CrossRef]
Disclaimer/Publisher’s Note: The statements, opinions and data contained in all publications are solely those of the individual
author(s) and contributor(s) and not of MDPI and/or the editor(s). MDPI and/or the editor(s) disclaim responsibility for any injury to
people or property resulting from any ideas, methods, instructions or products referred to in the content.

### 文献[6]参考文献节摘录（原文顺序，轻度清理）
- [1] M.M. Waldrop, More than moore, Nature 530 (7589) (2016) 144–148.
- [2] T.N. Theis, H.S. Wong, The end of moore’s law: a new beginning for information technology, Comput. Sci. Eng. 19 (2) (2017) 41–50.
- [3] H.H. Radamson, Y. Miao, Z. Zhou, Z. Wu, Z. Kong, J. Gao, et al., CMOS scaling for the 5 nm node and beyond: device, process and technology, Nanomaterials 14 (10) (2024) 837.
- [4] J. Cai, Z. Wu, S. Peng, Y. Wei, Z. Tan, G. Shi, M. Gao, K. Ma, In gemini: mapping and architecture Co-exploration for large-scale DNN chiplet accelerators, in: 2024 IEEE International Symposium on High-Performance Computer Architecture (HPCA), IEEE, 2024, pp. 156–171.
- [5] S. Zhang, Z. Li, H. Zhou, R. Li, S. Wang, K.W. Paik, P. He, Challenges and Recent Prospectives of 3D Heterogeneous Integration, vol. 2, e-Prime, 2022 100052.
- [6] J.H. Lau, Chiplet Heterogeneous Integration in Semiconductor Advanced Packaging, Springer, 2021, pp. 413–439.
- [7] W.T. Beyene, Chiplet technology and heterogeneous integration, IEEE Electr. Packag. Soc. Newsletter (2022).
- [8] S.A. Chew, V.J. De, E. Beyne, Wafer-to-wafer hybrid bonding at 400-nm interconnect pitch, Nat. Rev. Electr. Eng. 1 (2) (2024) 71–72.
- [9] M. Calabretta, A. Sitta, S.M. Oliveri, G. Sequenzia, In analysis of warpage induced by thick copper metal on semiconductor device, in: Advances on Mechanics, Design Engineering and Manufacturing III: Proceedings of the International Joint Conference on Mechanics, Design Engineering & Advanced Manufacturing, JCM, 2020, June 2-4, pp. 55–60.
- [10] G.B. Shinn, V. Korthuis, A. Wilson, G. Grover, S. Fang, Chemical-mechanical Polish, in: Handbook of Semiconductor Manufacturing Technology, 2000, pp. 415–460.
- [11] C.H. Lee, C.O. Park, Residual stress effect on self-annealing of electroplated copper, Jpn. J. Appl. Phys. 42 (7R) (2003) 4484.
- [12] R. Schmidt, C. Schwarz, In optimization of the Cu microstructure to improve copper-to-copper direct bonding for 3D integration, in: 2023 IEEE 73rd Electronic Components and Technology Conference (ECTC), IEEE, 2023, pp. 2024–2028.
- [13] Y. Zhang, P. Dong, J. Wang, X. Zhang, K. Leyendecker, M. Herkommer, V. Wohlfarth, J. Liang, In all nanograined copper is not created equal, in: 2023 IEEE 73rd Electronic Components and Technology Conference (ECTC), IEEE, 2023, pp. 1124–1128. G. Yang et al. Materials Chemistry and Physics 345 (2025) 131304
- [14] A. Heryanto, K. Pey, Y. Lim, W. Liu, J. Wei, N. Raghavan, J. Tan, D. Sohn, In study of stress migration and electromigration interaction in copper/low-k interconnects, in: 2010 IEEE International Reliability Physics Symposium, IEEE, 2010, pp. 586–590.
- [15] E. Chason, A. Engwall, F. Pei, M. Lafouresse, U. Bertocci, G. Stafford, J. Murphy, C. Lenihan, D. Buckley, Understanding residual stress in electrodeposited Cu thin films, J. Electrochem. Soc. 160 (12) (2013) D3285.
- [16] Y.M. Ahn, Y.J. Ko, H.J. Kim, D.H. Lee, S. Lee, J.H. Lee, Effect of plating condition on the mechanical properties and residual stress of electroplated copper film, Adv. Mater. Res. 26 (2007) 637–640.
- [17] V. Agrawal, B. Mitra, Microengineering. Residual stress tuning in UV-LIGA fabricated microstructures using deposition temperature and reverse pulse plating, J. Micromech. Microeng. 33 (3) (2023) 034003.
- [18] X. Feng, W. Luo, M. Li, S. Wang, Effect of leveler on microstructure and stress of electroplated copper for TSV application, in: 2013 3rd IEEE CPMT Symposium Japan, 2013, pp. 1–4.
- [19] I. Wang, C. Ku, T. Lam, E. Huang, K. Tu, C. Chen, Tuning stress in Cu thin films by developing highly (111)-Oriented nanotwinned structure, J. Electron. Mater. 49 (2020) 109–115.
- [20] R. Vayrette, C. Rivero, S. Blayac, K. Inal, Thickness effect on microstructure and residual stress of annealed copper thin films, Mater. Sci. Forum 681 (2011) 139–144.
- [31] T.C. Chan, Y.L. Chueh, C. Liao, Manipulating the crystallographic texture of nanotwinned Cu films by electrodeposition, Cryst. Growth Des. 11 (11) (2011) 4970–4974.
- [32] P. Scardi, P. Polonioli, S. Ferrari, Residual stress in stabilized zirconia thin films prepared by r.f. magnetron sputtering, Thin Solid Films 253 (1–2) (1994) 349–355.
- [33] Q. Luo, A.H. Jones, High-precision determination of residual stress of polycrystalline coatings using optimised XRD-sin2ψ technique, Surf. Coat. Technol. 205 (5) (2010) 1403–1408.
- [34] Q. Zhu, X. Zhang, S. Li, C. Liu, C.F. Li, Communication—Electrodeposition of nano- twinned Cu in void-free filling for blind microvia of high density interconnect, J. Electrochem. Soc. 166 (1) (2019) D3097–D3099.
- [35] T.C. Liu, C.M. Liu, H.Y. Hsiao, J.L. Lu, Y.S. Huang, C. Chen, Fabrication and characterization of (111)-oriented and nanotwinned Cu by Dc electrodeposition, Cryst. Growth Des. 12 (10) (2012) 5012–5016.
- [36] S.H. Kim, H.J. Lee, T.M. Braun, T.P. Moffat, D. Josell, Effect of chloride on microstructure in Cu filled microscale through silicon vias, J. Electrochem. Soc. 11 (2021) 168.
- [37] X. Ma, C. Huang, J. Moering, M. Ruppert, H.W. Hoeppel, M. Goeken, J. Narayan, Y. Zhu, Mechanical properties of copper/bronze laminates: role of interfaces, Acta Mater. 116 (2016) 43–52.
- [38] W.D. Nix, H. Gao, Indentation size effects in crystalline materials: a law for strain gradient plasticity, J. Mech. Phys. Solid. 46 (1998) 411–425.
- [21] C.H. Tseng, C. Chen, Growth of highly (111)-oriented nanotwinned Cu with the
- [39] H. Gao, Y. Huang, W.D. Nix, J.W. Hutchinson, Mechanism-based strain gradient addition of sulfuric acid in CuSO4 based electrolyte, Cryst. Growth Des. 19 (1) (2018) 81–89.
- [22] L.C. Huang, J.M. Song, C. Chen, Effects of initial Cu grain size and impurity residues on the liquid phase reactions between molten solder and electroplated Cu, Mater. Char. 206 (2023) 113459.
- [23] G. Yang, L. Li, L. Chang, W. Yang, G. Zhang, Z. Zhang, T. Shi, In residual stress plasticity I, Theory, J. Mech. Phys. Solids 47 (1999) 1239–1263.
- [40] D.J. Steigmann, R.W. Ogden, A note on residual stress, lattice orientation and dislocation density in crystalline solids, J. Elasticity 109 (2) (2012) 275–283.
- [41] H.E. Lin, D.P. Tran, G.H. Lin, H.J. Chuang, C. Chen, Effects of residual stress and microstructure on extremely anisotropic grain growth in nanotwinned Cu films, Mater. Char. 211 (2024) 113891. control based on electroplated metal grain characteristics in panel-level glass advanced packaging, in: 2024 25th International Conference on Electronic Packaging Technology (ICEPT), IEEE, 2024, pp. 1–5.
- [42] D. Xu, V. Sriram, V. Ozolins, J.M. Yang, K.N. Tu, G.R. Stafford, C. Beauchamp, In situ measurements of stress evolution for nanotwin formation during pulse electrodeposition of copper, J. Phys. 105 (2) (2009) 023521.
- [24] S. Brongersma, E. Kerr, I. Vervoort, A. Saerens, K. Maex, Grain growth, stress, and
- [43] S. Mahajan, C. Pande, M. Imam, B.B. Rath, Formation of annealing twins in fcc impurities in electroplated copper, J. Mater. Res. 17 (2002) 582–589. crystals, Acta Mater. 45 (6) (1997) 2633–2638.
- [25] R. Huang, W. Robl, H. Ceric, T. Detzel, G. Dehm, Stress, sheet resistance, and microstructure evolution of electroplated Cu films during self-annealing, IEEE Trans. Device Mater. Reliab. 10 (1) (2009) 47–54.
- [44] B. Cui, K. Han, Y. Xin, D. Waryoba, A.L. Mbaruku, Highly textured and twinned Cu films fabricated by pulsed electrodeposition, Acta Mater. 55 (13) (2007) 4429–4438.
- [26] C. Okoro, J.W. Lau, F. Golshany, K. Hummler, Y. Obeng, A detailed failure analysis
- [45] Y.S. Huang, C.M. Liu, W.L. Chiu, C. Chen, Grain growth in electroplated (111)- examination of the effect of thermal cycling on Cu TSV reliability, IEEE Trans. Electron. Dev. 61 (1) (2013) 15–22.
- [27] T. Wei, Q. Wang, J. Cai, L. Chen, J. Huang, L. Wang, L. Zhang, C. Li, In performance and reliability study of TGV interposer in 3D integration, in: 2014 IEEE 16th Electronics Packaging Technology Conference (EPTC), IEEE, 2014, pp. 601–605. oriented nanotwinned Cu, Scr. Mater. 89 (2014) 5–8.
- [46] Y. Qing, Y. Yinhui, W. Shiyu, X. Gaoling, Q. Yu, L. Yacheng, Effect of Mn contents on microstructure evolution and recrystallization behavior of 18.5% Cr low-nickel type duplex stainless steel during multi-pass hot compression, Metall. Mater. Trans. A (8) (2024) 55A.
- [28] W. Zhang, A. Li, G. Ma, K. Yin, Y. Xia, Z. Liu, C. Chan, K. Cheung, M. Bayes, K. Yee,
- [47] K.K. Alaneme, E.A. Okotete, Recrystallization mechanisms and microstructure Interpretation of texture changes during self-annealing of electroplated copper, Microelectron. Eng. 87 (12) (2010) 2488–2494. development in emerging metallic materials: a review, J. Sci. Adv. Mater. Devices 4 (1) (2019) 19–33.
- [29] C.H. Tseng, I.H. Tseng, Y.P. Huang, T.H. Yun, L. Jihperng, K.N. Tu, C. Chih, Kinetic study of grain growth in highly (111)-preferred nanotwinned copper films, Mater. Char. 168 (2020) 110545.
- [30] I.H. Tseng, Y.T. Hsu, J. Leu, K.N. Tu, C. Chen, Effect of thermal stress on anisotropic grain growth in nano-twinned and un-twinned copper films, Acta Mater. 206 (80) (2021) 116637.
- [48] W. Min, D.M. John, J. Jun, R.W. Peter, J.W. Angus, Microstructural evolution of mechanically deformed polycrystalline silicon for kerfless photovoltaics, Phys. Status Solidi 216 (10) (2019) 1800578.

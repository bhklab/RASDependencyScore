# RASDS (RAS Dependency Score)

## Introduction
 * [Mottini et al. (PMID: 31492820)](./references/31492820.pdf) claimed,
   - Decitabine showed antitumor activity against PDAC-dependent tumors.
   - Decitabine + trametinib (MEKi) had significant synergistic effects in PDAC-dependent tumors.
 * How to define PDAC-dependent or -independent tumors?
   - Mottini and collegues reimplemented the method previously proposed to calculate KRAS dependency scores (S- and L-scores) from two lists of genes below and filtered for meaningful and measurable genes such as protein-coding genes, resulting in a total of 119 and 146 genes, respectively.
   - S-score: [Singh et al. (PMID: 19477428)](./references/19477428.pdf) introduced RAS dependency signature genes ([_N_=325](./references/19477428_Supple.pdf)) and a RAS dependency scoring method.
   - L-score: [Loboda et al. (PMID: 20591134)](./references/20591134.pdf) introduced RAS pathway-related genes ([_N_=147](./20591134_Supple.xls)) and a RAS signature scoring method. (_RFPL3S_ [RNA gene] was excluded in the L-scoring method).

## KRAS dependency score
 * Synopsis
   - The top KRAS-dependent genes were selected as **up**-regulated genes, and the top KRAS-independent genes were selected as **down**-regulated genes.
   - The KRAS signature scores are calculated by subtracting the average normalized expression of "down" genes from the average normalized expression of "up" genes.
 * S-score
   - **UP-genes** (_N_=79): _ACTR3C_, _ANKRD22_, _ATP2C2_, _B3GNT3_, _BSPRY_, _C11orf52_, _C1orf106_, _C1orf116_, _C1orf172_, _C1orf210_,  
_C1orf74_, _C6orf141_, _CDA_, _CDH1_, _CDS1_, _CEACAM6_, _CGNL1_, _CLDN4_, _CLDN7_, _DENND1C_,  
_DNAJA4_, _DPP4_, _DSC2_, _EFNB2_, _EHF_, _ELF3_, _EPCAM_, _EPN3_, _EPS8L1_, _ERBB3_,  
_ESRP1_, _ESRP2_, _F11R_, _FRK_, _GALNT3_, _GPR115_, _GRHL2_, _HS3ST1_, _INPP4B_, _IRF6_,  
_ITGB6_, _KRTCAP3_, _LAD1_, _LAMA3_, _MAL2_, _MAOA_, _MAPK13_, _MPZL2_, _MPZL3_, _MYO1D_,  
_OVOL2_, _PCDH1_, _PGM2L1_, _PLEKHA7_, _PPL_, _PPP1R14C_, _PROM2_, _RAB11FIP4_, _RAB17_, _RAB25_,  
_RALGPS2_, _S100A14_, _SCEL_, _SCIN_, _SCNN1A_, _SDR16C5_, _SPINT1_, _ST14_, _SYK_, _SYTL5_,   
_TGFA_, _TIAF1_, _TMEM154_, _TMEM30B_, _TMEM45B_, _TMPRSS4_, _TSPoAN1_, _TTC9_, _VSIG1_
   - **DOWN-genes** (_N_=40): _ABP1_, _ACTA2_, _ADRA2C_, _ANTXR1_, _ANXA6_, _APLN_, _DYRK3_, _EML1_, _FAR1_, _HNRNPA2B1_,  
_HSPA12A_, _HTRA1_, _IKBIP_, _KCTD15_, _LIX1L_, _LOC541471_, _MAGEE1_, _MPHOSPH9_, _MPPE1_, _MSRB3_,   
_NUDT11_, _OSTM1_, _PARVB_, _PAX6_, _PLCB4_, _PPARGC1B_, _PPP4R2_, _RECK_, _RHOT1_, _RYK_,  
_SLC1A3_, _SLC47A1_, _SMARCD3_, _SRGN_, _SYDE1_, _SYNGR1_, _TMEM237_, _TUB_, _TXNRD1_, _WDR35_
 * L-score
   - **UP-genes** (_N_=105): _ADAM8_, _ADRB2_, _ANGPTL4_, _ARNTL2_, _CALM2_, _CALU_, _CAPZA1_, _CCL20_, _CD274_, _CDCP1_,   
_CLCF1_, _CSNK1D_, _CXCL1_, _CXCL2_, _CXCL3_, _CXCL5_, _CXCL8_, _DENND2C_, _DUSP1_, _DUSP4_,   
_DUSP5_, _DUSP6_, _EFNB1_, _EGR1_, _EHD1_, _ELK3_, _EREG_, _FERMT1_, _FOS_, _FOXQ1_,   
_G0S2_, _GDF15_, _GLTP_, _HBEGF_, _IER3_, _IL13RA2_, _IL1A_, _IL1B_, _ITGA2_, _ITPR3_,   
_KCNK1_, _KCNN4_, _KLF5_, _KLF6_, _LAMA3_, _LDLR_, _LHFPL2_, _LIF_, _MALL_, _MAP1LC3B_,   
_MAP7D1_, _MAST4_, _MMP14_, _MXD1_, _MYDGF_, _NAMPT_, _NAV3_, _NDRG1_, _NFKBIZ_, _NIPAL1_,   
_NT5E_, _OXSR1_, _PHLDA1_, _PHLDA2_, _PI3_, _PIK3CD_, _PIM1_, _PLAUR_, _PNMA2_, _PPP1R15A_,   
_PRNP_, _PTGS2_, _PTHLH_, _PTPRE_, _PTX3_, _PVR_, _S100A6_, _SDC1_, _SDC4_, _SEMA4B_,   
_SERPINB1_, _SERPINB2_, _SERPINB5_, _SESN2_, _SFN_, _SLC16A3_, _SLC2A14_, _SLC2A3_, _SLC9A1_, _SPRY4_,   
_TFPI2_, _TGFA_, _TIMP1_, _TMEM45B_, _TNFRSF10A_, _TNFRSF10B_, _TNFRSF12A_, _TNS4_, _TOR1AIP1_, _TSC22D1_,   
_TUBA4A_, _UAP1_, _UPP1_, _VEGFA_, _ZFP36_
   - **DOWN-genes** (_N_=41): _ABCC5_, _ACAP2_, _ARMC8_, _ATPAF1_, _AUTS2_, _CCSAP_, _CELSR2_, _CEP57L1_, _COQ7_, _DRD4_,   
_ENAH_, _ERP44_, _GREB1L_, _HNRNPU_, _HTATSF1_, _ID4_, _ITSN1_, _KDM4C_, _MIB1_, _MRPS14_,   
_MSI1_, _MSI2_, _NUP133_, _OGN_, _PARP1_, _PIAS1_, _RASL10B_, _RTN3_, _SEC63_, _SH3GL2_,   
_SMAD9_, _STARD7_, _SUGP1_, _TBC1D24_, _TMEFF1_, _TTC28_, _ZNF292_, _ZNF441_, _ZNF493_, _ZNF669_,   
_ZNF672_

## Datasets
 * Celllines (ORCESTRA)
   - CCLE (https://doi.org/10.5281/zenodo.3905462)
   - GDSC2 (https://doi.org/10.5281/zenodo.3905481)
   - gCSI (https://doi.org/10.5281/zenodo.3905452)
 * Organoids
   - Pricess Margaret Living Biobank (Gemcitabine + Trametinib, https://www.livingbiobank.ca/)
 * Patient cohorts
   - PCSI (resected cases, https://doi.org/10.18129/B9.bioc.MetaGxPancreas)
   - COMPASS (advanced, prospective cohort)



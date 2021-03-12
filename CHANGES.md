# r20210311
- Added Siemens Vida protocol

# r20210225
- Fixed Siemens Skyra protocol ([issue #6](https://github.com/spine-generic/protocols/issues/6))

# r20201001
- Philips DWI: Number of b=0 images: 3 --> 5

# 2019-11-11 Philips (v6)
- ME-GRE: TR 625ms --> 600ms
- ME-GRE: TE(1) 2.1ms --> 7.2ms
- ME-GRE: Matrix 320x319 --> 448x448
- ME-GRE: FOV 160 --> 224
- ME-GRE: BW 241.1 --> 254.8
- ME-GRE: SENSE no --> yes (p2)

# 2019-03-26: Siemens/Verio (v2)
- T1w: Shim tuneup --> standard
- T2w: flip angle 180deg --> 120deg
- T2w: TR 2s --> 1.5s
- T2w: Shim tuneup --> standard
- GRE-MT1/MT0/T1w: Added pre-scan normalize

# 2019-03-25: Siemens/Skyra_VE11C_ZOOMit (v5), Siemens/Skyra_VE11C_no-ZOOMit (v2)
- T1w: Shim tuneup --> standard
- T2w: Shim tuneup --> standard
- DWI: TE: 60ms --> min
- DWI: Gradient: Normal --> Fast (2ms lower TE)

# 2019-03-22: Siemens/Prisma_VE11C_ZOOMit (v8)
- DWI: TE: 60ms --> min
- GRE-MT1/MT0/T1w: FFT Img Scale: 10 --> 5 (to avoid saturation)

# 2019-03-22: Siemens/Prisma_VE11C_no-ZOOMit (v3)
- DWI: TE: 56ms --> min
- GRE-MT1/MT0/T1w: FFT Img Scale: 10 --> 5 (to avoid saturation)

# 2019-03-22: Siemens/Prisma_VE11C_ZOOMit (v7)
- T1w: Shim tuneup --> standard
- T2w: Shim tuneup --> standard
- DWI: Increase TE to be compatible with SH05 (rise time limitation): 60ms --> 61ms
- DWI no-ZOOMit: TE 60ms --> 56ms
- DWI: Added pre-scan normalize
- GRE-MT1/MT0/T1w: Added pre-scan normalize
- Updated pdfs

# 2019-03-08: Siemens/Prisma_VE11B (v2)
- Added protocol for VE11B platforms
- DWI: Added pre-scan normalize
- GRE-MT1/MT0/T1w: Added pre-scan normalize

# 2019-02-25: Siemens (v1)
- Merged all VE11 Prisma/Skyra ZOOMit/non-ZOOMit into a single importable file under: Prisma-Skyra_VE11/
- Note that this protocol is also compatible with VE11B sites.
- UPDATE 2019-03-22: This folder has now been removed due to inconsistencies and burden to maintain (depends on Siemens for generating it via simulator).

# 2019-02-12: SOP (v16)
- Laser marking below the chin --> below the nose

# 2019-02-05: SOP (v15)
- GE, MTS protocol: rhimsize, rhrcxres and rhrcyres were wrong. It is now fixed.

# 2019-01-31 GE_750_no-FOCUS (v1)
- Created protocol specific for no-FOCUS 750 systems
- Added cardiac gating, with 5 concatenation.
- GRE-MT1: Changed TR: 62ms-->35ms
- GRE-MT0: Changed TR: 62ms-->35ms
- ME-GRE: Added an anterior saturation band  (coronal, 100mm thick, +100mm towards anterior direction from FOV center) for better WM/GM contrast.
- Removed the SNR_sag scan.
- Generated and uploaded a protocol.tar file that matches the pdf/html protocol files (currently not the case).

# 2019-01-14 spineGeneric_multiSubjects (v2)
- Added: sherbrooke (n=7), milan (n=6), unf (n=2).
- Total: 31 subjects

# 2019-01-11 Philips (v5)
- T1w and T2w are now using two different "geo names" to prevent confusion about FOV placement.

# 2019-01-10 SOP (v14)
- T2w: Text was wrong: "Adjust the FOV so as to enclose the whole head"-->"Center the FOV at C3-C4 level as shown in the figure below".

# 2018-12-21 spineGeneric_multiSubjects (v1)
- Added: barcelona (n=6)
- Removed .DS_Store and other ugly OSX files
- Total: 16 subjects

# 2018-12-21 SOP (v13)
- Added Numbering for figures.
- Adjusted FOV and shim box on Fig_DWI.

# 2018-12-07 spineGeneric_multiSubjects (v0)
- First version of multi-subject public dataset (2 centers: ucl, unf.
- Total: 10 subjects

# 2018-12-07 SOP (v12)
- Subject preparation: added blurb about PulseOx
- DWI: Added coronal view to explain how to position shim box
- GRE-ME: Added picture to explain how to position shim box

# 2018-12-07 Siemens-Prisma-non-ZOOMit (v0)
- DWI: Made protocol withouth ZoomIT license

# 2018-12-06 Siemens-Skyra-non-ZOOMit (v0)
- DWI: Made protocol withouth ZoomIT license

# 2018-12-06 Siemens-Skyra-ZOOMit (v4)
- GRE-ME: Added anterior sat band for better WM/GM contrast

# 2018-12-05 Siemens-Prisma (v5)
- GRE-ME: Added anterior sat band for better WM/GM contrast

# 2018-12-04 Philips (v4)
- GRE-ME: PhaseEncode RL-->AP (to match other vendors)

# 2018-11-30 SOP (v11)
- DWI: Clarified A-P sat band positioning
- For GE scanners: make optional the use of CVs for resampling to the effective resolution (too complicated).

# 2018-10-19 Siemens-Skyra (v3)
- DWI: changed resolution 1.3-->0.9mm

# 2018-05-31 SOP (v10)
- Clarified figures for DWI

# 2018-05-27 SOP (v9)
- Added coil information

# 2018-05-27 Philips (v3)
- T1w: FOV: 256x256->320x260
- GRE-ME: PNS mode high->moderate to reduce "twitching" in abdomen (only +0.1ms TE)
- Added _R53 suffix to explicit that this sequence could not be imported in older versions.

# 2018-05-24 SOP (v8)
- Minor fix on T2w figure

# 2018-05-16 SOP (v7)
- Fixed missing figures

# 2018-05-16 GE (v3)
- T1w: Slight improvement.
- T2w: Adjusted echo train and parallel imaging factor.
- MT: Implemented older version of the 3D-SPGR sequence for compatibility with DV25.1 versions.

# 2018-05-16 SOP (v6)

# 2018-02-07 Siemens-Prisma (v4)
- exar file was from a wrong protocol. Now fixed it.

# 2018-01-25 GE (v2)
- T1w: use fast SPGR instead of BRAVO (see ADNI3_Basic_GE_25x)
- DWI: 1x1mm --> 0.9x0.9mm in plane
- DWI: Added protocol for FOCUS excitation pulse
- GRE-MT: removed fat sat.
- GRE-MT: removed sat band.

# 2017-12-22 Siemens-Prisma (v3)
- MT: Removed water excitation

# 2017-12-21 Siemens-Skyra (v2)
- MT: Removed water excitation
- T2w (no change): Cannot do 180-120-120 --> 180-160-160 because of SAR issues

# 2017-12-04 Philips (v2)
- T1w: Flip angle 8 --> 9
- T1w: Explicit TR/TE in pdf protocol. Should be close to 2000/3.72
- T1w: filter normal --> weak
- T2w: 0.9mm --> 0.8mm
- T2w: Flip refocus: 180-160-160... (no change)
- T2w: filter normal --> weak
- DWI: move after T2w
- GRE-MT: Matrix/FOV[mm] 192/172 --> 230/256 to match Siemens/GE
- GRE-MT: Phase encoding: A-P
- GRE-MT: TR[ms] 51 --> 57 (min for 50kg subject).
- GRE-MT: do not use Proset
- GRE-T1w: flip angle 11 --> 15
- Tried protocol with 50 kg (wrt. SAR)

# 2017-12-01 Siemens_Trio_VB17 (v2)
- Added comment about what coil to use
- Localizer: Cor+Cor --> Cor+Sag
- DWI: Added 4 b=0 to the protocol: DWI_b0
- DWI: Mode: REF --> ISO
- T2w: VFL refocusing flip: 120 --> 180
- T2w: Slice turbo factor 2 --> 1
- T2w: Set refocusing to 180 and increase TR (set subject weight to 50kg)
- MT: Remove water excitation (because if poor shim, it suppressed water signal)

# 2017-11-27 Siemens_Trio_VB17 (v1)
- First version uploaded (few modifs to do)

# 2017-11-23 Siemens_Skyra_VE11C (v1)
- DWI: change from Prisma: Gradient mode fast --> normal
- Protocol set up for 20ch head, but works equally well with the 64ch coil

# 2017-11-17 Siemens_Prisma_VE11C (v2)
- SAR: protocol tested at subject weight of 50kg
- T2w: TurboFact/EchoTrainDur[ms]/TA 88/287/4:33 --> 100/311/4:02
- GRE-MT: TR[ms]/TE[ms] 30/2.7 --> 35/2.62
- GRE-MT: PhaseEnc R-L --> A-P
- GRE-MT: Matrix/FOV[mm] 192/172 --> 256/230 (prevent A-P aliasing)
- GRE-MT: SliceOversampling[%] 0 --> 18.2 (prevent S-I aliasing)
- GRE-ME: Slices 18 --> 15 (to match DWI)
- GRE-ME: SliceThickness[mm] 3 --> 5 (to match DWI & MT)
- GRE-ME: SatBand: Anterior --> none
- GRE-ME: Matrix/FOV[mm] 128/256 --> 224/448 (prevent A-P aliasing
- GRE-ME: TR[ms]/TE[ms] 625/15 --> 600/14
- GRE-ME: NEx 3 --> 2

# 2017-11-07 Siemens_Prisma_VE11C (v1)
- DWI: 64dir --> 30dir to match Philips

# 2017-10-26 Siemens_Prisma_VE11C (beta)
- Changed order: put DWI before GRE (if pulseOx is defective after some time, better to do it faster)
- DWI: 30dir --> 64dir to match GE
- GRE-ME: matrix 256 --> 320 to match GE
- GRE-ME: phEnc: RL --> AP to avoid shoulders issue
- GRE-ME: use one sat band instead of two
- GRE-ME: BW 240Hz --> 260Hz
- GRE-ME: FOV 160mm --> 128mm
- GRE-ME: 15slc --> 18slc
- GRE-ME: nex 2 --> 3
- GRE-ME: TA 3:51min --> 4:24min

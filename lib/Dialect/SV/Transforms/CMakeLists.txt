add_circt_dialect_library(CIRCTSVTransforms
  GeneratorCallout.cpp
  HWCleanup.cpp
  HWStubExternalModules.cpp
  HWLegalizeModules.cpp
  PrettifyVerilog.cpp
  SVExtractTestCode.cpp
  HWExportModuleHierarchy.cpp
  SVTraceIVerilog.cpp
  HWEliminateInOutPorts.cpp

  DEPENDS
  CIRCTSVTransformsIncGen

  LINK_LIBS PUBLIC
  CIRCTComb
  CIRCTEmit
  CIRCTHW
  CIRCTSeq
  CIRCTSupport
  CIRCTSV
  MLIRIR
  MLIRPass
  MLIRTransformUtils
)

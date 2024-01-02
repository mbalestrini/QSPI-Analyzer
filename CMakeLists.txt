
set (ANALYZER_SDK_ROOT "${PROJECT_SOURCE_DIR}/SaleaeAnalyzerSDK")


set(QSPI_ANALYZER_SOURCES
    src/QSpiAnalyzer.cpp
    src/QSpiAnalyzer.h
    src/QSpiAnalyzerResults.cpp
    src/QSpiAnalyzerResults.h
    src/QSpiAnalyzerSettings.cpp
    src/QSpiAnalyzerSettings.h
    src/QSpiDataChannelManager.cpp
    src/QSpiDataChannelManager.h
    src/QSpiSimulationDataGenerator.cpp
    src/QSpiSimulationDataGenerator.h
    src/QspiTypes.h
    src/QSpiUtil.h
)

add_library(QSPIAnalyzer SHARED ${QSPI_ANALYZER_SOURCES})

#target_include_directories(QSPIAnalyzer PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_include_directories(QSPIAnalyzer PUBLIC ${ANALYZER_SDK_ROOT}/include)


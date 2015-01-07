cmake_minimum_required(VERSION 2.8)

set(CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/cmake)

project(latexCMakeExample NONE)
include(${CMAKE_SOURCE_DIR}/cmake/UseLATEX.cmake)
add_latex_document(latexCMake.tex
    INPUTS src/source1.tex
    BIBFILES bib/latexCMake.bib
    IMAGE_DIRS img
    DEFAULT_PDF)


#
# set up library 
#
set(LIBRARY_SOURCES
  Verbs.cpp
)
add_library(MemoryExperiments
  ${LIBRARY_SOURCES}
)
target_link_libraries(MemoryExperiments ${MEMORY_EXPERIMENT_LIBS} ${VERBS_LIB})
add_dependencies(MemoryExperiments all-third-party)





add_memory_application(helloworld.exe "helloworld.cpp")
add_memory_application(experiments.exe "experiments.cpp")

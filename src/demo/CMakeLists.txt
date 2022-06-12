set(WORKFLOW_LIB_DIR /home/zz/code/opensource/workflow/_lib)
link_directories(${WORKFLOW_LIB_DIR})

set(WORKFLOW_LIB workflow pthread OpenSSL::SSL OpenSSL::Crypto ${LIBRT})

add_executable(first1 first.cc)
target_link_libraries(first1 ${WORKFLOW_LIB})
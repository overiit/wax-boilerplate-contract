project(demopro)

set(EOSIO_WASM_OLD_BEHAVIOR "Off")
find_package(eosio.cdt)

add_contract( demopro demopro demopro.cpp )
target_include_directories( demopro PUBLIC ${CMAKE_SOURCE_DIR}/../include )
target_ricardian_directory( demopro ${CMAKE_SOURCE_DIR}/../ricardian )
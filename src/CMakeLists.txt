### CMake Postgres project: only for libpq external library.

###set(gen_errorcodes_depend
###	${PROJECT_SOURCE_DIR}/src/backend/utils/errcodes.txt
###	${PROJECT_SOURCE_DIR}/src/backend/utils/generate-errcodes.pl
###)
###set(gen_errorcodes_output
###	${PROJECT_SOURCE_DIR}/src/include/utils/errcodes.h
###)

###add_custom_command(
###	MAIN_DEPENDENCY ${gen_errorcodes_depend}
###	OUTPUT ${gen_errorcodes_output}
###	COMMAND ${PERL_EXECUTABLE} generate-errcodes.pl errcodes.txt > ${gen_errorcodes_output}
###	WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/src/backend/utils
###)

###add_custom_target(gen_errorcodes DEPENDS ${gen_errorcodes_output})

###add_subdirectory(include)
###add_subdirectory(port)
###add_subdirectory(common)
add_subdirectory(interfaces/libpq)

###add_subdirectory(backend)
###add_subdirectory(timezone)
###add_subdirectory(test/regress)
###add_subdirectory(test/isolation)

###add_subdirectory(pl/plpgsql/src)
###if(PYTHONINTERP_FOUND AND PYTHONLIBS_FOUND)
###	add_subdirectory(pl/plpython)
###endif()
###if(PERLLIBS_FOUND)
###	add_subdirectory(pl/plperl)
###endif()
###if(TCL_FOUND)
###	add_subdirectory(pl/tcl)
###endif()

###add_subdirectory(bin/initdb)
###add_subdirectory(bin/pg_archivecleanup)
###add_subdirectory(bin/pg_basebackup)
###add_subdirectory(bin/pg_config)
###add_subdirectory(bin/pg_controldata)
###add_subdirectory(bin/pg_ctl)
###add_subdirectory(bin/pg_dump)
###add_subdirectory(bin/pg_resetxlog)
###add_subdirectory(bin/pg_rewind)
###add_subdirectory(bin/pg_test_fsync)
###add_subdirectory(bin/pg_test_timing)
###add_subdirectory(bin/pg_upgrade)
###add_subdirectory(bin/pg_xlogdump)
###add_subdirectory(bin/pgbench)
###add_subdirectory(bin/psql)
###add_subdirectory(bin/scripts)

any_project_var_to_parent_scope()

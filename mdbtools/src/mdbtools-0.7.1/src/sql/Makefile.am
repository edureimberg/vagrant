lib_LTLIBRARIES	=	libmdbsql.la
libmdbsql_la_SOURCES=	mdbsql.c parser.y lexer.l 
libmdbsql_la_LDFLAGS = -version-info 2:0:0 -export-symbols-regex '^mdb_sql_'
CLEANFILES = parser.c parser.h lexer.c
AM_CFLAGS	=	-I$(top_srcdir)/include $(GLIB_CFLAGS)
LIBS	=	$(GLIB_LIBS)
libmdbsql_la_LIBADD =	../libmdb/libmdb.la
YACC = @YACC@ -d

AM_CFLAGS = -g -pg -Wall -DLIBCRANGE_FUNCDIR=\"$(pkglibdir)\" -DLIBCRANGE_CONF=\"/etc/libcrange.conf\" -DDEFAULT_SQLITE_DB=\"/var/range.sqlite\" -DLIBCRANGE_YAML_DIR=\"/var/range/\" -I../src @PCRE_CFLAGS@ @APR_CFLAGS@
AM_LDFLAGS = -module -L../src -L/tmp/install/lib64 -lcrange -lyaml -lsqlite3 @PCRE_LIBS@ @APR_LIBS@ -lmdbm 

pkglib_LTLIBRARIES = yst-ip-list.la ip.la nodescf.la yamlfile.la sqlite.la sqlite_mdbm.la

sqlite_la_SOURCES = sqlite.c
sqlite_mdbm_la_SOURCES = sqlite_mdbm.c
nodescf_la_SOURCES = nodescf.c
yamlfile_la_SOURCES = yamlfile.c
yst_ip_list_la_SOURCES = yst-ip-list.c netblock.c tinydns_ip.c \
                         hosts-netblocks.c
ip_la_SOURCES = ip.c tinydns_ip.c




ifndef TPC_VERSION
$(error TPC_VERSION not set)
endif

plugin.so:	foo-plugin.go
	docker run --rm -v $$PWD:/plugin-source tykio/tyk-plugin-compiler:$(TPC_VERSION) $@

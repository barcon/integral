# Alternative GNU Make workspace makefile autogenerated by Premake

ifndef config
  config=debug
endif

ifndef verbose
  SILENT = @
endif

ifeq ($(config),debug)
  quadrature_config = debug

else ifeq ($(config),release)
  quadrature_config = release

else
  $(error "invalid configuration $(config)")
endif

PROJECTS := quadrature

.PHONY: all clean help $(PROJECTS) 

all: $(PROJECTS)

quadrature:
ifneq (,$(quadrature_config))
	@echo "==== Building quadrature ($(quadrature_config)) ===="
	@${MAKE} --no-print-directory -C . -f quadrature.make config=$(quadrature_config)
endif

clean:
	@${MAKE} --no-print-directory -C . -f quadrature.make clean

help:
	@echo "Usage: make [config=name] [target]"
	@echo ""
	@echo "CONFIGURATIONS:"
	@echo "  debug"
	@echo "  release"
	@echo ""
	@echo "TARGETS:"
	@echo "   all (default)"
	@echo "   clean"
	@echo "   quadrature"
	@echo ""
	@echo "For more information, see https://github.com/premake/premake-core/wiki"
#
# Templet for Lua.
# Copyright © 2012 Peter Colberg.
# Distributed under the MIT license. (See accompanying file LICENSE.)
#

LUA = lua

ifdef LUA_PATH
LUA_PATH := $(CURDIR)/../?.lua;$(CURDIR)/../?/init.lua;$(LUA_PATH)
else
LUA_PATH := $(CURDIR)/../?.lua;$(CURDIR)/../?/init.lua;;
endif
export LUA_PATH

TESTS = templet

all: $(TESTS)

$(TESTS):
	$(LUA) $@.lua

.PHONY: $(TESTS)

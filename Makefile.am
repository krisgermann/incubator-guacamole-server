#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
# KIND, either express or implied.  See the License for the
# specific language governing permissions and limitations
# under the License.
#

ACLOCAL_AMFLAGS = -I m4

# Subprojects
DIST_SUBDIRS =           \
    src/libguac          \
    src/common           \
    src/common-ssh       \
    src/terminal         \
    src/guacd            \
    src/guacenc          \
    src/protocols/rdp    \
    src/protocols/ssh    \
    src/protocols/telnet \
    src/protocols/vnc    \
    tests

SUBDIRS =       \
    src/libguac \
    src/common  \
    tests

if ENABLE_COMMON_SSH
SUBDIRS += src/common-ssh
endif

if ENABLE_TERMINAL
SUBDIRS += src/terminal
endif

if ENABLE_RDP
SUBDIRS += src/protocols/rdp
endif

if ENABLE_SSH
SUBDIRS += src/protocols/ssh
endif

if ENABLE_TELNET
SUBDIRS += src/protocols/telnet
endif

if ENABLE_VNC
SUBDIRS += src/protocols/vnc
endif

if ENABLE_GUACD
SUBDIRS += src/guacd
endif

if ENABLE_GUACENC
SUBDIRS += src/guacenc
endif

EXTRA_DIST =     \
    LICENSE      \
    bin/guacctl  \
    doc/Doxyfile


# Copyright (c) 2015 Cisco and/or its affiliates.
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at:
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
AUTOMAKE_OPTIONS = foreign subdir-objects

AM_CPPFLAGS = -Wall @VEC64@ # -Werror

if WITH_UNIX
  lib_LTLIBRARIES = libvppinfra.la
endif

lib_LIBRARIES =

TESTS	=  test_bihash_template \
	   test_elog \
	   test_elf \
	   test_fifo \
	   test_format \
	   test_hash \
	   test_heap \
	   test_longjmp \
	   test_macros \
	   test_md5 \
	   test_mheap \
	   test_pfhash \
	   test_phash \
	   test_pool_iterate \
	   test_qhash \
	   test_random \
	   test_random_isaac \
	   test_serialize \
	   test_slist \
	   test_socket \
	   test_time \
	   test_timing_wheel \
	   test_vec \
	   test_zvec 

noinst_PROGRAMS = $(TESTS)
check_PROGRAMS	= $(TESTS)

test_bihash_template_SOURCES = vppinfra/test_bihash_template.c
test_elog_SOURCES = vppinfra/test_elog.c
test_elf_SOURCES = vppinfra/test_elf.c
test_fifo_SOURCES = vppinfra/test_fifo.c
test_format_SOURCES = vppinfra/test_format.c
test_hash_SOURCES = vppinfra/test_hash.c
test_heap_SOURCES = vppinfra/test_heap.c
test_longjmp_SOURCES = vppinfra/test_longjmp.c
test_macros_SOURCES = vppinfra/test_macros.c
test_md5_SOURCES = vppinfra/test_md5.c
test_mheap_SOURCES = vppinfra/test_mheap.c
test_pfhash_SOURCES = vppinfra/test_pfhash.c
test_phash_SOURCES = vppinfra/test_phash.c
test_pool_iterate_SOURCES = vppinfra/test_pool_iterate.c
test_qhash_SOURCES = vppinfra/test_qhash.c
test_random_SOURCES = vppinfra/test_random.c
test_random_isaac_SOURCES = vppinfra/test_random_isaac.c
test_serialize_SOURCES = vppinfra/test_serialize.c
test_slist_SOURCES = vppinfra/test_slist.c
test_socket_SOURCES = vppinfra/test_socket.c
test_time_SOURCES = vppinfra/test_time.c
test_timing_wheel_SOURCES = vppinfra/test_timing_wheel.c
test_vec_SOURCES = vppinfra/test_vec.c
test_zvec_SOURCES = vppinfra/test_zvec.c

# All unit tests use ASSERT for failure
# So we'll need -DDEBUG to enable ASSERTs
test_bihash_template_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_elog_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_elf_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_fifo_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_format_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_hash_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_heap_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_longjmp_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_macros_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_md5_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_mheap_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_pfhash_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_phash_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_pool_iterate_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_qhash_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_random_CPPFLAGS = $(AM_CPPFLAGS) -DCLIB_DEBUG
test_random_isaac_CPPFLAGS = $(AM_CPPFLAGS) -DCLIB_DEBUG
test_socket_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_serialize_CPPFLAGS = $(AM_CPPFLAGS) -DCLIB_DEBUG
test_slist_CPPFLAGS = $(AM_CPPFLAGS) -DCLIB_DEBUG
test_time_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_timing_wheel_CPPFLAGS = $(AM_CPPFLAGS) -DCLIB_DEBUG
test_vec_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG
test_zvec_CPPFLAGS =	$(AM_CPPFLAGS) -DCLIB_DEBUG

test_bihash_template_LDADD =	libvppinfra.la
test_elog_LDADD =	libvppinfra.la
test_elf_LDADD =	libvppinfra.la
test_fifo_LDADD =	libvppinfra.la
test_format_LDADD =	libvppinfra.la
test_hash_LDADD =	libvppinfra.la
test_heap_LDADD =	libvppinfra.la
test_longjmp_LDADD =	libvppinfra.la
test_macros_LDADD =	libvppinfra.la
test_md5_LDADD =	libvppinfra.la
test_mheap_LDADD =	libvppinfra.la
test_pfhash_LDADD =	libvppinfra.la
test_phash_LDADD =	libvppinfra.la
test_pool_iterate_LDADD =	libvppinfra.la
test_qhash_LDADD =	libvppinfra.la
test_random_LDADD =	libvppinfra.la
test_random_isaac_LDADD =	libvppinfra.la
test_serialize_LDADD =	libvppinfra.la
test_slist_LDADD =	libvppinfra.la
test_socket_LDADD =	libvppinfra.la
test_time_LDADD =	libvppinfra.la -lm
test_timing_wheel_LDADD =	libvppinfra.la -lm
test_vec_LDADD =	libvppinfra.la
test_zvec_LDADD =	libvppinfra.la

test_bihash_template_LDFLAGS = -static
test_elog_LDFLAGS = -static
test_elf_LDFLAGS = -static
test_fifo_LDFLAGS = -static
test_format_LDFLAGS = -static
test_hash_LDFLAGS = -static
test_heap_LDFLAGS = -static
test_longjmp_LDFLAGS = -static
test_macros_LDFLAGS = -static
test_md5_LDFLAGS = -static
test_mheap_LDFLAGS = -static
test_pfhash_LDFLAGS = -static
test_phash_LDFLAGS = -static
test_pool_iterate_LDFLAGS = -static
test_qhash_LDFLAGS = -static
test_random_LDFLAGS = -static
test_random_isaac_LDFLAGS = -static
test_serialize_LDFLAGS = -static
test_slist_LDFLAGS = -static
test_socket_LDFLAGS = -static
test_time_LDFLAGS = -static
test_timing_wheel_LDFLAGS = -static
test_vec_LDFLAGS = -static
test_zvec_LDFLAGS = -static

# noinst_PROGRAMS += test_vhash
# test_vhash_SOURCES = vppinfra/test_vhash.c vppinfra/vhash.c
# test_vhash_CPPFLAGS = $(AM_CPPFLAGS) -DCLIB_DEBUG
# test_vhash_LDADD = libvppinfra.la
# test_vhash_LDFLAGS = -static

nobase_include_HEADERS = \
  vppinfra/asm_mips.h \
  vppinfra/asm_x86.h \
  vppinfra/bihash_8_8.h \
  vppinfra/bihash_24_8.h \
  vppinfra/bihash_template.h \
  vppinfra/bihash_template.c \
  vppinfra/bitmap.h \
  vppinfra/bitops.h \
  vppinfra/byte_order.h \
  vppinfra/cache.h \
  vppinfra/clib.h \
  vppinfra/elf.h \
  vppinfra/elf_clib.h \
  vppinfra/elog.h \
  vppinfra/fheap.h \
  vppinfra/error.h \
  vppinfra/error_bootstrap.h \
  vppinfra/fifo.h \
  vppinfra/format.h \
  vppinfra/graph.h \
  vppinfra/hash.h \
  vppinfra/heap.h \
  vppinfra/longjmp.h \
  vppinfra/macros.h \
  vppinfra/math.h \
  vppinfra/md5.h \
  vppinfra/mem.h \
  vppinfra/mhash.h \
  vppinfra/mheap.h \
  vppinfra/mheap_bootstrap.h \
  vppinfra/os.h \
  vppinfra/pfhash.h \
  vppinfra/phash.h \
  vppinfra/pipeline.h \
  vppinfra/pool.h \
  vppinfra/qhash.h \
  vppinfra/random.h \
  vppinfra/random_buffer.h \
  vppinfra/random_isaac.h \
  vppinfra/serialize.h \
  vppinfra/slist.h \
  vppinfra/smp.h \
  vppinfra/smp_fifo.h \
  vppinfra/socket.h \
  vppinfra/sparse_vec.h \
  vppinfra/string.h \
  vppinfra/time.h \
  vppinfra/timing_wheel.h \
  vppinfra/timer.h \
  vppinfra/types.h \
  vppinfra/unix.h \
  vppinfra/vec.h \
  vppinfra/vec_bootstrap.h \
  vppinfra/vector.h \
  vppinfra/vector_altivec.h \
  vppinfra/vector_funcs.h \
  vppinfra/vector_iwmmxt.h \
  vppinfra/vector_sse2.h \
  vppinfra/valgrind.h \
  vppinfra/vm_unix.h \
  vppinfra/xxhash.h \
  vppinfra/xy.h \
  vppinfra/zvec.h

CLIB_CORE = \
  vppinfra/asm_x86.c \
  vppinfra/backtrace.c \
  vppinfra/elf.c \
  vppinfra/elog.c \
  vppinfra/error.c \
  vppinfra/fifo.c \
  vppinfra/fheap.c \
  vppinfra/format.c \
  vppinfra/graph.c \
  vppinfra/hash.c \
  vppinfra/heap.c \
  vppinfra/longjmp.S \
  vppinfra/macros.c \
  vppinfra/mhash.c \
  vppinfra/mheap.c \
  vppinfra/md5.c \
  vppinfra/mem_mheap.c \
  vppinfra/pfhash.c \
  vppinfra/phash.c \
  vppinfra/qhash.c \
  vppinfra/random.c \
  vppinfra/random_buffer.c \
  vppinfra/random_isaac.c \
  vppinfra/serialize.c \
  vppinfra/slist.c \
  vppinfra/smp.c \
  vppinfra/smp_fifo.c \
  vppinfra/std-formats.c \
  vppinfra/string.c \
  vppinfra/time.c \
  vppinfra/timing_wheel.c \
  vppinfra/unformat.c \
  vppinfra/vec.c \
  vppinfra/vector.c \
  vppinfra/zvec.c

# Core plus Unix additions
libvppinfra_la_SOURCES =			\
  $(CLIB_CORE)					\
  vppinfra/elf_clib.c				\
  vppinfra/socket.c				\
  vppinfra/timer.c				\
  vppinfra/unix-formats.c			\
  vppinfra/unix-misc.c

bin_PROGRAMS = elftool

elftool_SOURCES = tools/elftool.c
elftool_CPPFLAGS = -Wall
elftool_LDADD = libvppinfra.la -lpthread -lrt -lm

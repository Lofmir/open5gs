# Copyright (C) 2019 by Sukchan Lee <acetcom@gmail.com>

# This file is part of Open5GS.

# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.

testunit_sources = files('''
    abts-main.c
    s1ap-message-test.c
    nas-message-test.c
    gtp-message-test.c
    security-test.c
    crash-test.c
'''.split())

testunit_exe = executable('unit',
    sources : testunit_sources,
    c_args : testcore_cc_flags,
    dependencies : libtestapp_dep)

test('unit', testunit_exe, is_parallel : false, suite: 'unit')

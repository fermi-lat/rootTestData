# -*- python -*-
# @file SConscript
# @brief build info
#
# $Id: SConscript,v 1.2 2009/01/23 00:07:52 ecephas Exp $
# Authors: Heather Kelly <heather@milkyway.gsfc.nasa.gov>,David Chamont <chamont@poly.in2p3.fr>
# Version: rootTestData-04-02-00
Import('baseEnv')
Import('listFiles')
progEnv = baseEnv.Clone()

progEnv.Tool('registerTargets', 
             package = 'rootTestData',
             data = listFiles(['data/*'],recursive=True))
	






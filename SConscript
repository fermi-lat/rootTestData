# -*- python -*-
# @file SConscript
# @brief build info
#
# $Id: SConscript,v 1.3 2009/08/27 18:08:26 jrb Exp $
# Authors: Heather Kelly <heather@milkyway.gsfc.nasa.gov>,David Chamont <chamont@poly.in2p3.fr>
# Version: rootTestData-04-02-01
Import('baseEnv')
Import('listFiles')
progEnv = baseEnv.Clone()

progEnv.Tool('registerTargets', 
             package = 'rootTestData',
             data = listFiles(['data/*'],recursive=True))
	






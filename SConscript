# -*- python -*-
# @file SConscript
# @brief build info
#
# $Id: SConscript,v 1.4 2009/11/10 01:29:54 jrb Exp $
# Authors: Heather Kelly <heather@milkyway.gsfc.nasa.gov>,David Chamont <chamont@poly.in2p3.fr>
# Version: rootTestData-04-03-00
Import('baseEnv')
Import('listFiles')
progEnv = baseEnv.Clone()

progEnv.Tool('registerTargets', 
             package = 'rootTestData',
             data = listFiles(['data/*'],recursive=True))
	






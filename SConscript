# -*- python -*-
# @file SConscript
# @brief build info
#
# $Id: SConscript,v 1.6 2010/06/11 00:48:34 jrb Exp $
# Authors: Heather Kelly <heather@milkyway.gsfc.nasa.gov>,David Chamont <chamont@poly.in2p3.fr>
# Version: rootTestData-04-03-01
Import('baseEnv')
Import('listFiles')
progEnv = baseEnv.Clone()

jofiles = listFiles(['src/gamma_5_gev_normal/*.txt']) + listFiles(['src/default/*.txt'])
jofiles.append('src/vertical_surface_muons/redoRecon.txt')
jofiles.append('src/vertical_surface_muons/redoDigi.txt')
jofiles.append('src/vertical_surface_muons/jobOptions.txt')
                    

progEnv.Tool('registerTargets', 
             package = 'rootTestData',
             data = listFiles(['data/*'],recursive=True),
             jo= jofiles)
	






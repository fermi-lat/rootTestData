# -*- python -*-
# @file SConscript
# @brief build info
#
# $Id: SConscript,v 1.10 2013/02/11 06:42:01 heather Exp $
# Authors: Heather Kelly <heather@slac.stanford.edu>,Leon Rochester <lsrea@slac.stanford.edu>
# Version: rootTestData-04-06-01
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
             jo= jofiles,
             xml = listFiles(['xml/*'], recursive=True))
	






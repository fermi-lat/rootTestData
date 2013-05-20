# -*- python -*-
# @file SConscript
# @brief build info
#
# $Id: SConscript,v 1.14 2013/05/19 01:42:09 lsrea Exp $
# Authors: Heather Kelly <heather@slac.stanford.edu>,Leon Rochester <lsrea@slac.stanford.edu>
# Version: rootTestData-04-06-05
Import('baseEnv')
Import('listFiles')
progEnv = baseEnv.Clone()

jofiles = listFiles(['src/gamma_5_gev_normal/*.txt']) + listFiles(['src/default/*.txt'])
jofiles.append('src/vertical_surface_muons/redoRecon.txt')
jofiles.append('src/vertical_surface_muons/redoDigi.txt')
jofiles.append('src/vertical_surface_muons/jobOptions.txt')
jofiles.append('src/cal/jobOptions.txt')
                    

progEnv.Tool('registerTargets', 
             package = 'rootTestData',
             data = listFiles(['data/*'],recursive=True),
             jo= jofiles,
             xml = listFiles(['xml/*'], recursive=True))
	






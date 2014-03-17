mediaServer
============

nodejs platinum module

Install:
Download PlatinumKit, extract to node_modules/Platinum
Don't install gyp
Go to Platinum/Platinum
Change scons: -fPIC
 vim Build/Tools/SCons/gcc-generic.py
	After the line:    if gcc_stop_on_warning == None: gcc_stop_on_warning = env['stop_on_warning']
	Add:
	    env.AppendUnique(CCFLAGS = '-fPIC')

Go to Platinum/Platinum, build Platinum with scons
sudo npm install -g node-gyp

./build.sh

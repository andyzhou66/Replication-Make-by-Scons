print('Hi A test of Scons')
import os
# env = Environment(ENV=os.environ.copy(),opt="")
# print(env['ENV']['PATH'])

# env=Environment(BUILDERS={'Python':Builder(action='Scripts\python.exe $SOURCES $opt $TARGET')})


env=Environment(BUILDERS={'Python':Builder(action='python $SOURCES $opt $TARGET')},ENV=os.environ.copy(),\
                opt='')

env.Python('results.txt',['testzipf.py', 'isles.dat'],opt=">")
env.Python('isles.dat',['countwords.py', 'books/isles.txt'])


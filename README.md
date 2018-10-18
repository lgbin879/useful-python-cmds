# useful-python-cmds

#获取文件夹下所有文件名

for root, dirs, files in os.walk('.'):
  print(root) #当前目录路径
  print(dirs) #当前路径下所有子目录
  print(files) #当前路径下所有非目录子文件

#如果文件大小为0，删除此文件

for file in files:
  if os.path.getsize(file) == 0:
  print('delete ', file)
  os.system('rm -rf '+file)




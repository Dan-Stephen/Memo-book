# System module:

  sys.path 表示 Python 搜索模块的路径和查找顺序：

  sys.platform 显示当前操作系统信息：

  sys.version python version information

  sys.exc_info() 可以显示 Exception 的信息

# OS module

*文件路径操作
  os.getcwd() 当前目录
  os.listdir(os.curdir) 当前目录下的文件
  产生文件：f = open("test.file", "w")
  重命名文件：os.rename("test.file", "test.new.file")
  删除文件： os.remove("test.new.file")
* 系统常量
  当前操作系统的换行符：os.linesep
  当前操作系统的路径分隔符：os.sep
* os.path 模块
  测试
    os.path.isfile(path) ：检测一个路径是否为普通文件
    os.path.isdir(path)：检测一个路径是否为文件夹
    os.path.exists(path)：检测路径是否存在
    os.path.isabs(path)：检测路径是否为绝对路径
  split 和 join
    os.path.split(path)：拆分一个路径为 (head, tail) 两部分
    os.path.join(a, *p)：使用系统的路径分隔符，将各个部分合成一个路径
  其他

# 修饰符

  修饰符是这样的一种函数，它接受一个函数作为输入，通常输出也是一个函数

  用 @ 来使用修饰符：
    Python 使用 @ 符号来将某个函数替换为修饰符之后的函数

  修饰器工厂：
    decorators factories 是返回修饰器的函数；
    它的作用在于产生一个可以接受参数的修饰器。
    
  应用：
    @classmethod 将一个对象方法转换了类方法
    @property (只读)模仿 Java 的getters 和 setters 的方法，调用方法时可以省去括号
    Numpy 的 @vectorize 修饰符： 将一个函数转换为 ufunc

# OOP
  

用gulp自动化根据传入参数自动化创建文件夹

命令行： gulp create --fn xxx 或者 gulp create (默认不传参数文件夹命名为base)

主要思路：
创建模板文件夹 template -> template_idx.html
                          template_idx_bkmmdd.html
                          
gulp创建create方法，引入minimist处理命令行参数，rename替换template为传入参数名，mmdd替换当天日期。

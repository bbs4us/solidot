Slashcode 中文版的服务器及数据库安装设置说明

请按照 INSTALL 文件里的说明进行安装，这里特别提示的是如果你的服务器已经安装的有 Apache, 要把Apache 卸载重新手工编译安装，不能使用 RPM 或 debian apt-get 安装包进行安装，安装包安装的 Apache 下，Slashcode 将不能正常工作。

其他软件比如 Perl, Mod\_perl 等要与 INSTALL 里列出的软件版本相符，MySQL 要用 4.1.x 版本，这要与Solidot 现在的数据保持一致。

如果将来的数据库管理要用 phpMyAdmin 的话，编译 Apache 时要考虑加载 PHP，应该加载 Apache DSO 模块，让 Mod\_perl 和 PHP 以 DSO 动态模块运行。Slashcode 是支持 Mod\_perl 作为 DSO 运行的。

整个安装过程如果顺利的话大约需要3个小时左右，其中安装 Perl 模块（Bundler Slash）这一过程最耗时间，需要坐下来倒杯水喝着让它慢慢进行，这个过程根据网速不同可能需要 1-2个小时。

网站的编码使用 UTF8, 从服务器设置，到 MySQL, 到数据库校勘编码等都要设置为 UTF8.


Jesse Lee
2006-12-26
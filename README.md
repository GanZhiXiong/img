

## 驱动程序无法通过使用安全套接字层(SSL)加密与 SQL Server 建立安全连接。

![](https://ppoffice.github.io/hexo-theme-icarus/gallery/screenshots/disqus-get-shortname.png)

在添加 Data Sources 界面，驱动选择 Microsoft SQL Server，输入连接配置信息后，点击 `Test Connection`，报错如下：

```basic
[08S01] 驱动程序无法通过使用安全套接字层(SSL)加密与 SQL Server 建立安全连接。错误:“PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target”。 ClientConnectionId:16497bc5-424b-4395-ac01-e2439eb66a14 unable to find valid certification path to requested target.
```

该问题一般是驱动的问题，我这里换成 9.4.0 的版本就没有问题了。

![](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202204221221714.png)

## Inconsistent language: It is recommended to use Azure SQL Database dialect instead of Microsoft SQL Server Use Azure SQL Database

![](https://cdn.jsdelivr.net/gh/ganzhixiong/img/blog/202204221224784.png)

翻来过来就是：

> 语言不一致：建议使用 Azure SQL 数据库方言，而不是 Microsoft SQL Server 使用 Azure SQL 数据库

我将 Driver 选择 Azure SQL Database，尝试了改驱动的前四个版本，都会报如下错误。

```basic
[08S01] 驱动程序无法通过使用安全套接字层(SSL)加密与 SQL Server 建立安全连接。错误:“PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target”。 ClientConnectionId:f71345e9-2855-4fd3-b8b7-57f0a62a9f1e unable to find valid certification path to requested target.
```

估计还是驱动问题。这个问题就先放着，反正用 Microsoft SQL Server 驱动能用。

# img
## img
### img
#### img

| 硬件           | Mac  Studio                     | MBP 16 2021                       | MBP 15 2018                                             | 比较   |
| -------------- | ------------------------------- | --------------------------------- | ------------------------------------------------------- | ------ |
| 💰 Price        | 19499-1950（教育优惠）=17549 ￥ | 18999 - 1500（教育优惠）= 17499 ¥ | 19200 ¥                                                 | 1701   |
| CPU            | M1 Max 10 Cores 3.22 GHz        | M1 Pro 10 Cores 3.22 GHz          | Intel Core i7 6 Cores 2.2 GHz                           |        |
| 💯 Multi-core   | 12669                           | 12441                             | 5343                                                    | 2.3 倍 |
| 💯 Single-core  | 1782                            | 1761                              | 979                                                     | 1.8 倍 |
| GPU            | M1 Pro 24 Cores                 | M1 Pro 16 Cores                   | Radeon Pro 555X 4 GB<br/>Intel UHD Graphics 630 1536 MB |        |
| 💯 GPU (OpenCL) | 51244                           | 37495                             | 14687                                                   | 2.6 倍 |
| 💯 GPU (Metal)  | 61670                           | 4 万多                            | 15448                                                   |        |
| Memory         | 64 GB                           | 16 GB                             | 32 GB                                                   |        |
| SSD            | 1 T                             | 512 GB                            | 512 GB                                                  |        |
| 💯 Write Speed  | 5335 MB/s                       | 5423 MB/s                         | 2545 MB/s                                               | 2 倍   |
| 💯 Read Speed   | 5300 MB/s                       | 4021 MB/s                         | 1869 MB/s                                               | 2 倍   |


SQL Server 实例的下列级别**支持**设置排序**规则**：

- [服务器级排序规则](https://docs.microsoft.com/zh-cn/sql/relational-databases/collations/collation-and-unicode-support?view=sql-server-ver15#Server-level-collations)
- [数据库级排序规则](https://docs.microsoft.com/zh-cn/sql/relational-databases/collations/collation-and-unicode-support?view=sql-server-ver15#Database-level-collations)
- [列级排序规则](https://docs.microsoft.com/zh-cn/sql/relational-databases/collations/collation-and-unicode-support?view=sql-server-ver15#Column-level-collations)
- [表达式级排序规则](


朋友买了一台 M1 PRO 的 MBP 16 2021，那就比较下这个新款和我的 2.2 GHz Intel Core i7 的 MBP 15 2018 的性能吧。

**总体来说，性能高 2 倍多，且性价比高出太多，如果没有 MBP 的非常值得购买。但是我已经有了，所以我还是等明年春季的 Mac mini 吧，期待能上 M2。**


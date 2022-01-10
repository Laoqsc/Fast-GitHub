# FAST-GitHub

# 简介

国内 Github 下载很慢，用上了这个插件后，下载速度嗖嗖嗖的~！ 

[![Page Views Count](https://badges.toozhao.com/badges/01EH1R0YMQANV1ACQXTEBK7JCN/green.svg)](https://badges.toozhao.com/badges/01EH1R0YMQANV1ACQXTEBK7JCN/green.svg "Get your own page views count badge on badges.toozhao.com")



# 下载插件

因Chrome开发者账号中的一个插件出现问题，导致所有插件被下架。

现在另外一个账号申请上线，目前审核中，上线后会更新Chrome插件的地址。

很抱歉给大家带来的不便。

<table>
<tbody>
<tr>
<td>
<a href="#" target="_blank">
        <img src="https://i.loli.net/2021/04/23/IqpU7COKQvzrcyG.png" />
      </a>
</td>
<td><a href="https://apps.apple.com/cn/app/fastgithub/id1564025982?mt=12" target="_blank">
        <img src="https://i.loli.net/2021/04/23/SKsywoGWg1HvEja.png" />
      </a></td>
<td>
<a href="https://microsoftedge.microsoft.com/addons/detail/github%E5%8A%A0%E9%80%9F/alhnbdjjbokpmilgemopoomnldpejihb" target="_blank">
        <img src="https://i.loli.net/2021/04/23/EnS3eDi4I86Yv2N.png" />
      </a>
</td>
<td><a href="https://addons.mozilla.org/en-US/firefox/addon/fastgithub/" target="_blank">
        <img src="https://i.loli.net/2021/04/23/4wGaRTisEdcBnIt.png" />
      </a></td>
</tr>
</tbody>
</table>

# 预览

![MNOt8347RDGmnjo](https://i.loli.net/2021/04/23/MNOt8347RDGmnjo.png)

![9UPXkGsHzw5hiru](https://i.loli.net/2021/04/23/9UPXkGsHzw5hiru.png)


# 如何使用 SSH 通道

配置用户配置文件 (`~/.ssh/config`)

```bash
Host github.com
	HostName github.com
	User git
	IdentityFile 指定密钥认证使用的私钥文件路径
# 新增如下内容
Host git.zhlh6.cn
	HostName git.zhlh6.cn
	User git
	IdentityFile 使用github.com的秘钥
```

测试 SSH 连接

```bash
ssh -T git@git.zhlh6.cn

# 成功
You've successfully authenticated, but GitHub does not provide shell access
```
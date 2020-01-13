# 路由器
在路由器方面的学习总结


首先非常感谢前辈们的分享。

# 个人的路由器硬件设备
- 斐讯 K2P A2 无 USB 端口

# 杂谈
- 听说 padavan 固件比较好，个人也刷过潘多拉、高恪、官改等固件，由于各种原因，个人都不太满意。
- 也曾刷过 hobby 的 padavan 固件，但对我来说过于臃肿，所以就有了下面我的尝试。

# 个人的需求
- v2ray
- get 到 padavan 粉色的路由指示灯（*- 老夫的少女心呀 -*）

# 资料准备
- 搭建 v2ray 【https://github.com/233boy/v2ray/wiki】
- padavan-nano 固件 【https://github.com/hanwckf/rt-n56u/releases】
- v2ray 插件 【https://github.com/ntgeralt/v2ray-for-padavan】

# 注意事项
- ntgeralt 前辈的 v2ray 插件如其 readme 说明，不太适用我的情况。我已经提交 issue 给前辈。【https://github.com/ntgeralt/v2ray-for-padavan/issues/1】

# 杂谈
- 嫌麻烦的伙伴儿可以直接将我修改后的 v2ray 插件，修改 /etc/storage/v2ray/config.json 文件，然后上传到自己的路由器中。
- chmod 775 -R /etc/storage/v2ray/
- 在自定义设置 -> 脚本 -> '在防火墙规则启动后执行下' 粘贴 sh /etc/storage/v2ray/sh-whitelist.sh
- 如果不想重启，便手动输入命令便可以了：sh /etc/storage/v2ray/sh-whitelist.sh

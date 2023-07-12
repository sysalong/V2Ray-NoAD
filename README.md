下载文件 .dat 域名文件放到 V2Ray 的资源目录中，域名文件的标签及标签对应的域名见同名文件夹下的文件，在 V2Ray 配置中按标签设定路由规则，所有的域名均以子域名的形式进行匹配。

rules :
{
    "type": "field",
    "domain": ["ext:geosite.dat:reject"],	//广告域名屏蔽
    "outboundTag": "blocked"
},{
    "type": "field",
    "domain": ["ext:geosite.dat:proxy"],
    "outboundTag": "proxy"
},{
    "type": "field",
    "domain": ["ext:geosite.dat:proxyjp"],
    "outboundTag": "proxyjp"
},{
    "type": "field",
    "domain": ["ext:geosite.dat:direct"],
    "outboundTag": "direct"
},{
    "type": "field",
    "domain": ["ext:geosite.dat:cn"],
    "outboundTag": "direct"
},


因为我本人主要用它过滤广告，所以一般我只用上面的过滤广告的规则，具体的请直接下载dat文件放入v2ray目录即可。然后更改config配置，加入广告屏蔽规则。

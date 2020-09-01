# 部署

### p2p引导节点的部署

    1.编译future/cmd/boot
    2.在服务器上启动该程序，
        -k 指定私钥文件
        -p 私钥文件密码
        
        例：
        ./boot -k ../wallet/keystore/FMYDoqLnsVz3QSLjFh5isbcSCgY7N9Gh3SY.json -p 1
       
    3.如果需要链接该引导节点，可以在配置文件的boot项中配置该引导节点的地址信息
       
        例：
        ```
        Boot="/ip4/8.210.100.179/tcp/19100/ipfs/16Uiu2HAmCrUCC6zyvqteHnokLcBEsMVz6FsXmskLzipXMTLTVg4N"
        ```
### 超级节点的部署

    部署超级节点需要在配置文件中配置超级节点的地址的私钥文件和私钥文件的解密密码
       
        例：
        # If it is a block generating node, it needs to be configured
        # Json file address of the address private key
        KeyFile = "../wallet/keystore/FMizWwybDdxE9wWtbeiukj4ixcnMGLaT5La.json"
        # Password to decrypt the private key json file
        KeyPass = "1"
        
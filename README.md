# ZAMA
# 区块链无隐私项目

这是一个简单的区块链实现，专注于透明性和不可篡改特性，所有交易都是公开可见的。

## 项目特点

- 完整的区块链核心实现
- 工作量证明共识机制
- 分布式节点网络
- 交易广播和验证
- 链冲突解决

## 技术实现

- 使用Python实现
- Flask框架构建API
- SHA-256哈希算法
- JSON数据格式

## 运行方式

1. 安装依赖pip install flask requests
2. 启动节点python node.py
3. 可以通过修改`node.py`中的端口号启动多个节点，形成分布式网络

## API接口

- `GET /mine` - 挖矿新块
- `POST /transactions/new` - 添加新交易
- `GET /chain` - 获取完整区块链
- `POST /nodes/register` - 注册新节点
- `GET /nodes/resolve` - 执行共识算法

## 使用示例

1. 添加交易curl -X POST -H "Content-Type: application/json" -d '{
    "sender": "Alice",
    "recipient": "Bob",
    "amount": 10
}' "http://localhost:5000/transactions/new"
2. 挖矿curl "http://localhost:5000/mine"
3. 获取区块链curl "http://localhost:5000/chain"
## 贡献

欢迎对本项目提出改进建议或提交Pull Request
    

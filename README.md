# BlockChain_Basic
Khái quát cơ bản về cơ chế thực hiện một giao dịch của block và cách hoạt động của các máy đào

Nói đến blockchain thì không thể bỏ qua từ khóa "phân tán và cơ chế đồng thuận"

Hình "Pow-trong-bitcoin.jpg" sẽ mô tả cách thức hoạt động của chuỗi block.
<img src="https://github.com/LongHuu100/BlockChain_Basic/blob/main/Pow-trong-bitcoin.jpg" />

Hình "cryptocurrency-blockchain-terminal-image-two.jpe" kết quả mô phỏng code js để chứng minh tính nhất quán của chuỗi.
<img src="https://github.com/LongHuu100/BlockChain_Basic/blob/main/cryptocurrency-blockchain-terminal-image-one.jpeg" />

Trong kết quả của hình "2.cryptocurrency-blockchain-terminal-image-two.jpeg" thì thấy các nonce cho chuỗi 1 là 175413, chuỗi 2 là: 76998.
<img src="https://github.com/LongHuu100/BlockChain_Basic/blob/main/2.cryptocurrency-blockchain-terminal-image-two.jpeg" />

# Máy đào (minner)
Để giải mã cho chuỗi 1 trong ví dụ trên thì các máy đào sẽ phải thực hiện tối đa 1 triệu lần tính toán mã hash và so sánh cho đến khi nào gặp số 175413 thì mới xác thực xong một giao dịch.


# Năng lượng và tiền bạc
Đế xác minh được một giao dịch như trên thì hằng trăm máy đào cũng thực hiện giải mã, mỗi máy tối đa 1triêu lần thì năng lượng tiêu hao quả thực khủng khiếp để có được một giao dịch thành công, mỗi lần xác mình thành công thì máy đào sẽ được thường một khoản nho nhỏ tùy theo cơ chế của đồng coin

# A Peer-to-Peer Electronic Cash System
https://bitcoin.org/bitcoin.pdf


# Step By Step

The steps to run the network are as follows:

1) New transactions are broadcast to all nodes.
2) Each node collects new transactions into a block.
3) Each node works on finding a difficult proof-of-work for its block.
4) When a node finds a proof-of-work, it broadcasts the block to all nodes.
5) Nodes accept the block only if all transactions in it are valid and not already spent.
6) Nodes express their acceptance of the block by working on creating the next block in the
chain, using the hash of the accepted block as the previous hash.

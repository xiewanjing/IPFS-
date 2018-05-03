#IPFS-入门

#IPFS Overview

•	IPFS Types

•	API Transports

•	API Commands

•	Implementing bindings for the HTTP API

其中已有部分被开发的可以直接用于IPFS的库，如下：

自描述性合约/格式

•	multiaddr

•	multihash

•	multicodec

•	multistream

IPFS Types

密碼雜湊函式（Cryptographic hash function），又譯為加密雜湊函式、密碼雜湊函式、加密雜湊函式，是雜湊函式的一種。

它被認為是一種單向函式，也就是說極其難以由雜湊函式輸出的結果，回推輸入的資料是什麼。

這種雜湊函式的輸入資料，通常被稱為訊息（message），而它的輸出結果，經常被稱為訊息摘要（message digest）或摘要（digest）。

許多重要的應用，都使用了密碼雜湊函式來實作，例如數位簽章，訊息鑑別碼。
 
 ![image](https://github.com/xiewanjing/IPFS-/blob/master/sha.png)
 
 图中为描述不同加密哈希函数下生成的64位哈希数
 
  ![image](https://github.com/xiewanjing/IPFS-/blob/master/sha2-256.png)
 
 图中为用于区分不同加密哈希函数的头4位，1120为sha2-256，11为函数类型，20指函数长度

•<ipfs-path> is a unix-style path, beginning with /ipfs/<hash>/... or /ipns/<hash>/... or /ipns/<domain>/....

•	<hash> is a base58 encoded multihash (there are many implementations). It is usually the hash of an ipfs object (or merkle dag node).

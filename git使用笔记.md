# 关于git reset的3种方式

1. --hard
   
   使用git reset --hard <commited ID>后，工作区，暂存区，本地仓的内容，都会恢复到<commited ID>对应节点的历史版本，并且之前<commited ID>后面的所有<commited ID>都会被删除，所以在很明确地知道某些修改不需要的情况下，就使用--hard。

2. --soft
   
   使用git reset --soft <commit ID>后，工作区和暂存区的内容都不会被修改，只是将本地库回退到<commited ID>对应节点的历史版本。

3. -- mixed
   
   使用git reset --mixed <commit ID>后，暂存区和本地库会被回退到<commited ID>对应节点的历史版本，但是工作区不会被修改。

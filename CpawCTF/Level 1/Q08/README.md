## 問題文
Q8.[Misc] Can you open this file ?

このファイルを開きたいが拡張子がないので、どのような種類のファイルで、どのアプリケーションで開けば良いかわからない。

どうにかして、この拡張子がないこのファイルの種類を特定し、どのアプリケーションで開くか調べてくれ。

問題ファイル： open_me

## 解答
ファイルに拡張子がなかったため、ファイル形式をfileコマンドで調査、「Document File V2 Document」形式のファイルであることを確認した。

```
% file open_me
Composite Document File V2 Document, Little Endian, Os: Windows, Version 10.0, Code page: 932, Author: ?v??, Template: Normal.dotm, Last Saved By: ?v??, Revision Number: 1, Name of Creating Application: Microsoft Office Word, Total Editing Time: 28:00, Create Time/Date: Mon Oct 12 04:27:00 2015, Last Saved Time/Date: Mon Oct 12 04:55:00 2015, Number of Pages: 1, Number of Words: 3, Number of Characters: 23, Security: 0
```

「open_me」に拡張子.docを追加してLibraOfficeで開くことができ、flagをゲットした

cpaw{Th1s_f1le_c0uld_be_0p3n3d}

## 参考
Document File開封方法：
* https://ja.ojit.com/so/linux/435748
* https://social.technet.microsoft.com/Forums/en-US/ecc38456-e18a-458b-a093-0223da69c108/what-is-composite-document-file-v2-document?forum=Offtopic


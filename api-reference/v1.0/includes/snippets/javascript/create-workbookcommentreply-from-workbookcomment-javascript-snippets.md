---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d575bcaa2c2f59e6a8f552822b6b0a096b2f9ba4
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookCommentReply = {
  content: "This is my reply to the comment.",
  contentType: "plain"
};

let res = await client.api('/drive/root/workbook/comments/{id}/replies')
    .post(workbookCommentReply);

```
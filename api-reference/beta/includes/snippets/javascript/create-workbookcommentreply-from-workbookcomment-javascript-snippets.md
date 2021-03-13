---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b44f87581f10c16e6add8190d473b959d1155ce9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookCommentReply = {
  content: 'This is my reply to the comment.',
  contentType: 'plain'
};

await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .version('beta')
    .post(workbookCommentReply);

```
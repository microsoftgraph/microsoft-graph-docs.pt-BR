---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd03abe46038ced06eacd82dc63ddabeb1310c0dacbcccb49e71301e63927417
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275209"
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
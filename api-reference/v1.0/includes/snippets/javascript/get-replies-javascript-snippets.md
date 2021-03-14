---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f76b983ddb408e77bb5695ec9b1e4331ec49911a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c114be258d66c520dd75e4aeedf241ec4e93ead6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/attachments/{id}')
    .delete();

```
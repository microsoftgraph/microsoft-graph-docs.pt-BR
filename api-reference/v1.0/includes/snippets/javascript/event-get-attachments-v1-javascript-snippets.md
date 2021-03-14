---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6152b146e7f2ad6081a9a9a2f408d107848f823f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/events/{id}/attachments')
    .get();

```
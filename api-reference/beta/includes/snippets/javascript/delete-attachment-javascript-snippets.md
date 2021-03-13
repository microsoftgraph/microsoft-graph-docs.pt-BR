---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e899f137bf0d5fbb7c83b4add188399154739fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/attachments/{id}')
    .version('beta')
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de164929c16eb3b2a398dd8bc70744225e76f796
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/dismissReminder')
    .version('beta')
    .post();

```
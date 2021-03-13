---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa2c9b24b357c52483b1b3147552f7de26c1008f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/events/{id}/attachments')
    .version('beta')
    .get();

```
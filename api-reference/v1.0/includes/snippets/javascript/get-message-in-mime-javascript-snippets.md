---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aabbd551bd7a1c61fb4eac8a6784c47646be9692
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/messages/4aade2547798441eab5188a7a2436bc1/$value')
    .get();

```
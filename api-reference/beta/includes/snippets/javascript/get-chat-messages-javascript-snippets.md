---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f0e06ec330f67fa9c8178cf4cac33d1f541b9a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/chats/{id}/messages')
    .version('beta')
    .get();

```
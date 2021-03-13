---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6c1912211ce1faaf524e24aad8f74f4ef26df90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPatent = await client.api('/me/profile/patents/{id}')
    .version('beta')
    .get();

```
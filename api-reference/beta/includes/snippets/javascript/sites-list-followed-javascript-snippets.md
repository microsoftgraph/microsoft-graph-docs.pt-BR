---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0d0a92a742c0f27d4fa677ed3da95d12c6e526f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let followedSites = await client.api('/me/followedSites')
    .version('beta')
    .get();

```
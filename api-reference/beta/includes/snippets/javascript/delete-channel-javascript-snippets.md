---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3407e2219087cb7e0c730a68ea1ca6cb04310d3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .delete();

```
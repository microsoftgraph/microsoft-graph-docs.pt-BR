---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2169316169ea17d4c5421a4fffc97fa2e17fc00e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredOwners/{id}/$ref')
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 866cfd9d57d18135fa80ed9277933308de6e92ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryRoles/{role-objectId}/members/{user-id}/$ref')
    .delete();

```
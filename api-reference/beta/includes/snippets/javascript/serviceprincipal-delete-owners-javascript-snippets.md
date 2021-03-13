---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39cf6e2bb6a03b082b37b9b8049750f3876617b8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794815"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/owners/{id}/$ref')
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4642a4e3491824b24bb6bcd711bdb377f3c92699
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/servicePrincipals/{id}/transitiveMemberOf')
    .get();

```
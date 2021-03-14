---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19e118f6a1bec67277ce8ea25ec2a20a7e47ca29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bd6f6fb12c982781a71c14f3e6049acac205e3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .version('beta')
    .get();

```
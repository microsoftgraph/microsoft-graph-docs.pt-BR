---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6175e9d00f5b5a2e9efbb3e4cc95bd9e0837af0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/servicePrincipals/{id}/owners')
    .version('beta')
    .get();

```
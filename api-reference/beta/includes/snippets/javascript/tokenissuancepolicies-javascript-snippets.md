---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 627bfd54fa9c1ee896f4de9d177eaadcf92e1253
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/policies/tokenIssuancePolicies')
    .version('beta')
    .get();

```
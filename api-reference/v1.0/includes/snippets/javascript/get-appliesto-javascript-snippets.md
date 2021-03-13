---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50dd131b6725bfc8b818072ad66533a3bf7275b2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/claimsMappingPolicies/{id}/appliesTo')
    .get();

```
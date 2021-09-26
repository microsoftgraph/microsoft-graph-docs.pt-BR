---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89bbd521ac6aed8f5c187edc64e236ddef77957e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59929118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
    displayName: 'UpdateClaimsPolicy'
};

await client.api('/policies/claimsMappingPolicies/{id}')
    .update(claimsMappingPolicy);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4057d5a93811f2c4aebde910be1dda1967e2587d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/homeRealmDiscoveryPolicies/6c6f154f-cb39-4ff9-bf5b-62d5ad585cde/appliesTo')
    .version('beta')
    .get();

```
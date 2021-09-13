---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a85bcbc0956d9a8271daa2e035c19c81b11ac553108fada932d85035485c408a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    conditions: {
        signInRiskLevels: [
            'high',
            'medium',
            'low',
        ]
    }
};

await client.api('/identity/conditionalAccess/policies/{id}')
    .update(conditionalAccessPolicy);

```
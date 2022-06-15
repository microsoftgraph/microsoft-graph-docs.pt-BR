---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38574ed9e90c1ca6757d543fde39a9224147f53d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/eDiscoveryCases/061b9a92-8926-4bd9-b41d-abf35edc7583/close')
    .version('beta')
    .post();

```
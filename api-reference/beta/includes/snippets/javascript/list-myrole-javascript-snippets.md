---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15336aba171bf37095304054d610dd9d8ca1f7ba
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let myRoles = await client.api('/tenantRelationships/managedTenants/myRoles')
    .version('beta')
    .get();

```
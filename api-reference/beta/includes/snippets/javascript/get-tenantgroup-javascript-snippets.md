---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a85aefb2555042482ca313ea318b3f7658050f074cba010792affef02142908
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273310"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantGroup = await client.api('/tenantRelationships/managedTenants/tenantGroups/{tenantGroupId}')
    .version('beta')
    .get();

```
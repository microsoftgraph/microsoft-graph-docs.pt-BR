---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2576042a2bb74561330da9c9917e2c4d622d4097f951dfc07338580c4a37c599
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenants = await client.api('/tenantRelationships/managedTenants/tenants')
    .version('beta')
    .get();

```
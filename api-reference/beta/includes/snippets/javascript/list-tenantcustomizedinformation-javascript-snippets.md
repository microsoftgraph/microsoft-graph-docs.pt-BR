---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4b46fca2b4e68e84ba9584203cdc085e46a101b625989728632827dd2f31d19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantsCustomizedInformation = await client.api('/tenantRelationships/managedTenants/tenantsCustomizedInformation')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c4a44a3da153cdb0a7d4d648d0268a0063796a4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440629"
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
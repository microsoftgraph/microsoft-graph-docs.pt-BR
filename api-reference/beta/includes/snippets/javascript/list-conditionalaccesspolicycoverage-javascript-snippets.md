---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28e8a0c12148772b1b7d6fa36b87a26bc0bce84c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicyCoverages = await client.api('/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages')
    .version('beta')
    .get();

```
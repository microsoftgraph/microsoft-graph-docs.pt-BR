---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be563f1769cedadb55635ff2ac312d500bd8bcd4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementAction = await client.api('/tenantRelationships/managedTenants/managementActions/{managementActionId}')
    .version('beta')
    .get();

```
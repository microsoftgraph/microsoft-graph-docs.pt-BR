---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad6c7918c60862f56c34c53924cb7342d8d61be7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementTemplates = await client.api('/tenantRelationships/managedTenants/managementTemplates')
    .version('beta')
    .get();

```
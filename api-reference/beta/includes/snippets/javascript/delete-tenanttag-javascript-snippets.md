---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fca7111f5e02c4c19f521c6c6d6627543a630e91aaf602f517608b16cb6241f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}')
    .version('beta')
    .delete();

```
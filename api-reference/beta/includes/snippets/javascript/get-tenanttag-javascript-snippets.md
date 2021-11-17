---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0be4f2227f3298b0e6eeb9aa2e0fa74b310b44976e5a6b14522f3c4b968ef3ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantTag = await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}')
    .version('beta')
    .get();

```
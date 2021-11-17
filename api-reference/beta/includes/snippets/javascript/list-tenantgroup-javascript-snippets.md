---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c4e47e6b494e75cec5c8c680556177eafee81bc31131028be3170930612ceaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantGroups = await client.api('/tenantRelationships/managedTenants/tenantGroups')
    .version('beta')
    .get();

```
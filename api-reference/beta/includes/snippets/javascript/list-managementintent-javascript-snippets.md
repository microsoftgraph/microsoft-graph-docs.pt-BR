---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f023e1d149667f690ab22406ea82e20b965ba79d0d85756d2e49e3ba7267b41a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementIntents = await client.api('/tenantRelationships/managedTenants/managementIntents')
    .version('beta')
    .get();

```
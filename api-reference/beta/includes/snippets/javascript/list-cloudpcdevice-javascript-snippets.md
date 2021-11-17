---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7770e18f826f4feae5879ed1ece78bed3d05dafa3be2b6aac6218f27145c6800
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcDevices = await client.api('/tenantRelationships/managedTenants/cloudPcDevices')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b04ec9462ffa4f31e2d103335f5fda9521799e114f4e90f2eebf320bb031636d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName: 'Connected organization new name',
  description: 'Connected organization new description',
  state: 'configured'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .update(connectedOrganization);

```
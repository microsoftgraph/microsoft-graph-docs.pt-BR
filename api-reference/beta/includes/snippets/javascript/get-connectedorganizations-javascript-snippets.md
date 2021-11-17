---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa65fee96941f8279e266019031e9505fb9aaea4b599f4fb193c2610ce630e11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100512"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectedOrganizations = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations')
    .version('beta')
    .get();

```
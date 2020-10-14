---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11671c282c48c89d43e16d85459aac1ad9acd7f3
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: "delegated",
  clientApplicationsFromVerifiedPublisherOnly: true
};

let res = await client.api('/policies/permissionGrantPolicies/{id}/includes')
    .version('beta')
    .post(permissionGrantConditionSet);

```
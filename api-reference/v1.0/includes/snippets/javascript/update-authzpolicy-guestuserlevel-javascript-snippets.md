---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2eae8131596086e13e5cacb08ee9782f2f3bd18
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
  allowEmailVerifiedUsersToJoinOrganization: false
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```
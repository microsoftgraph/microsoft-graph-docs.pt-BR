---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76a34e2ad25fee0350dc506c2530336484ff2667
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const delegatedPermissionClassifications = {
  permissionId: "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  permissionName: "User.Read",
  classification: "low"
};

let res = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .version('beta')
    .post(delegatedPermissionClassifications);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72580c7cebb5027daea80f862e043d6130199380
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principalId}')
    .delete();

```
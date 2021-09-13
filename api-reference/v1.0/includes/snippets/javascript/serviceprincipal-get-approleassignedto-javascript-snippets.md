---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b11ca7c1a87db09b5be39214047a6063ed5b2506438c06adad11327df3b84742
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignedTo = await client.api('/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo')
    .get();

```
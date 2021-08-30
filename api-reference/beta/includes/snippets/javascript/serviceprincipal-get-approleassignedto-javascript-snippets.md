---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 326744d383bfb017c02c1b82abfc0b9f8da66749e102120f10383c8fa916ba18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignedTo = await client.api('/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo')
    .version('beta')
    .get();

```
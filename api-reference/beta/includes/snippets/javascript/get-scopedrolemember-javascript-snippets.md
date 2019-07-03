---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8624245f53816e7a2bfda41e4248ea4eb496a56
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476078"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .get();

```
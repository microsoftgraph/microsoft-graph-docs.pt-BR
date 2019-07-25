---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8624245f53816e7a2bfda41e4248ea4eb496a56
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710682"
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
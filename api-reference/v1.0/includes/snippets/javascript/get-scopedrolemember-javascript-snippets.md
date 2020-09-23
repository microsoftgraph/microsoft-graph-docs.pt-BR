---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4c504a0c236513351e61183d51d30ca1970d131
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223507"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers')
    .get();

```
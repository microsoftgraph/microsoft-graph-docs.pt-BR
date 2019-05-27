---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c84f402880447fcd45871f924ea56908cec1f58f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473936"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignments')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b21bb58d2b5e9a26644efc44535ec0bf247995a0
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipal = await client.api('/groups/3802e9bb-0951-4e18-b9eb-f934b4241194/members/microsoft.graph.servicePrincipal')
    .version('beta')
    .get();

```
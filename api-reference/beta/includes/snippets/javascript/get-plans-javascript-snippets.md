---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb351828c8bfde1c6f21aa44b77dc73c98ccda91
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans')
    .version('beta')
    .get();

```
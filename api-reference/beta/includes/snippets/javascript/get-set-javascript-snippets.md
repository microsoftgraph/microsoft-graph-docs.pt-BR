---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96504bfb69693a459e98dc9a78c33fb32f64e950
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/groups/{groupId}/sets')
    .version('beta')
    .get();

```
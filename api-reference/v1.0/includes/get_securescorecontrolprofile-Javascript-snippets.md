---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdcb54069667118af908b12f588d7344d38c2967
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles/{id}')
    .version('beta')
    .get();

```
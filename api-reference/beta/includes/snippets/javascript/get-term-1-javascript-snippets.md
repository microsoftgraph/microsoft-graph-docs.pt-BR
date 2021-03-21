---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1291ebc246000abce5a0ed0ca8db12a741c1bb91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let term = await client.api('/termStore/groups/{groupId}/sets/{setId}/terms/{termId}')
    .version('beta')
    .get();

```
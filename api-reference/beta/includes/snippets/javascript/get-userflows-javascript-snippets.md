---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9db1bdd8d732f7cbc61b44bd3f115fc9d36dd1b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/userFlows')
    .version('beta')
    .get();

```
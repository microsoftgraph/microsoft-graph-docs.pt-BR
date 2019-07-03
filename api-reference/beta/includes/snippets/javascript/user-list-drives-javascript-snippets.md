---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bea2a492f342ff0c0003eea147f7c90d90942982
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/drives')
    .version('beta')
    .get();

```
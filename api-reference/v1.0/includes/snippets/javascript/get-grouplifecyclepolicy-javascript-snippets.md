---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63a3f59d6dd4323d7ec3ddf81a84a9967d4e7824
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies')
    .get();

```
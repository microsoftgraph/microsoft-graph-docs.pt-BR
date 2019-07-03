---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e11c9c0108e8a2d266fd78b31c78782e6e25c586
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions/{id}')
    .get();

```
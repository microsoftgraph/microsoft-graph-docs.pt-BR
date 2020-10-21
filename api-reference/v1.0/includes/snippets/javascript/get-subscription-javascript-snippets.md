---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e11c9c0108e8a2d266fd78b31c78782e6e25c586
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions/{id}')
    .get();

```
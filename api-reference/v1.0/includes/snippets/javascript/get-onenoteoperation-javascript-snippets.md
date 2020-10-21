---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79c9a7ea97011b26f0dde23a02a8e99a8a730860
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/operations/{id}')
    .get();

```
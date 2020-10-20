---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66255c8734ce710555129cfb5b3a8253c4c7d41d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/operations/{id}')
    .version('beta')
    .get();

```
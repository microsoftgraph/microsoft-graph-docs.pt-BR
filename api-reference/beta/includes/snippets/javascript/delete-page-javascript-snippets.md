---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c994f0260f61a4bf213b34b063d5c208cd2cb63f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .version('beta')
    .delete();

```
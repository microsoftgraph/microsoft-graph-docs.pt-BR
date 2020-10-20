---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462b6fe2c91155e0a849710e8da766385b52ca26
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/recent')
    .version('beta')
    .get();

```
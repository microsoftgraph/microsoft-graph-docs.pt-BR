---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d82df24336f40a7f0c89218aeb3c9acee14fb6c8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}')
    .delete();

```
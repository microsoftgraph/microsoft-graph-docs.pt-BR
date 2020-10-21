---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b3c24aa119cec9f63e8cb2c4b902d0e4ec5822a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .delete();

```
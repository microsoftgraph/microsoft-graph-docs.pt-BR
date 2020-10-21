---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67c10e9f52ad598fc92d0584dd5a6f1273a4eabd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a108f67c9b0e4efff113397c5f6ada797be71b7c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/removeFavorite')
    .version('beta')
    .post();

```
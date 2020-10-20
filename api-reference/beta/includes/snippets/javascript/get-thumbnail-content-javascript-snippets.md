---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb08a332ec248166e43b1996427483d178d20362
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .version('beta')
    .get();

```
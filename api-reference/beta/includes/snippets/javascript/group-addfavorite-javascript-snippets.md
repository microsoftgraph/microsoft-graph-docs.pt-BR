---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 101b788f3acc271fec281cbae184e3f1225869ef
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/addFavorite')
    .version('beta')
    .post();

```
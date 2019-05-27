---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a108f67c9b0e4efff113397c5f6ada797be71b7c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444724"
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
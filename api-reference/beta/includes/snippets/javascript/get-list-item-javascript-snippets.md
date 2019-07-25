---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9eeeff72289312701e8fa37764583a1a0df908f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41a16df56d1ad555eef06869938d86081850392c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/items/TSP228082938')
    .version('beta')
    .delete();

```
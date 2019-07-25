---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61ccaf936632396b98b92dc7f6656153b4c50512
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35704973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}')
    .get();

```
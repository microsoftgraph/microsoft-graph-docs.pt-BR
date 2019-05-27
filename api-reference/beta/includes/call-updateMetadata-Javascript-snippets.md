---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5444b6bf58454917e84d80714421e2eea44bfedf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  metadata: "metadata-value",
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/updateMetadata')
    .version('beta')
    .post(CommsOperation);

```
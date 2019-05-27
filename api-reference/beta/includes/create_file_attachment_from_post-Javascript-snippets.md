---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44fd630a038f92cd8ec25c6acbd59a5051b52f92
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "name-value",
  contentBytes: "contentBytes-value"
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/attachments')
    .version('beta')
    .post({attachment : attachment});

```
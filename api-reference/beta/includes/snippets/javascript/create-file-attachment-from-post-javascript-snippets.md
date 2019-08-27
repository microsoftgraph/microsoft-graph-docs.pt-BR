---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44fd630a038f92cd8ec25c6acbd59a5051b52f92
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633892"
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
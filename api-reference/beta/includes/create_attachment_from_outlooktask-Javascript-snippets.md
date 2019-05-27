---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b8afb2ab222cd54a681fbf8a8f8ccff0a5a5ec5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  lastModifiedDateTime: "datetime-value",
  name: "name-value",
  contentType: "contentType-value",
  size: 99,
  isInline: true
};

let res = await client.api('/users/{id}/outlook/tasks/{id}/attachments')
    .version('beta')
    .post({attachment : attachment});

```
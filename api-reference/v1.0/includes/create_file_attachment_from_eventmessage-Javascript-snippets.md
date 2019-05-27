---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c634633cce1ec4fea0efa612bf9e292d39579d85
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "microsoft.graph.fileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "base64-contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .post({attachment : attachment});

```
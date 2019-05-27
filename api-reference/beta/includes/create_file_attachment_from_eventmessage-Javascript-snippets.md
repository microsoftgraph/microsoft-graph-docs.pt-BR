---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6e6648284cc49b0e5384a918668055201922c67
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.FileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .post({attachment : attachment});

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e5fbe9bb42988962981337f9db73cdcf208267c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "smile",
  contentBytes: "a0b1c76de9f7="
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post({attachment : attachment});

```
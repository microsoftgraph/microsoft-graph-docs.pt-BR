---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f27f06d0cb79674396f2c3c2ac2da53aa081c40b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480726"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.fileAttachment",
    name: "menu.txt",
    contentBytes: "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
};

let res = await client.api('/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments')
    .version('beta')
    .post({attachment : attachment});

```
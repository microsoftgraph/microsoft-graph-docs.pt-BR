---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f27f06d0cb79674396f2c3c2ac2da53aa081c40b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714095"
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
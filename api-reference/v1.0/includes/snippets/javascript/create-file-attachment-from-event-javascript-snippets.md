---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b981006aa71d7bd70cc6740553657f78fea81528
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.fileAttachment",
    name: "menu.txt",
    contentBytes: "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
};

let res = await client.api('/me/events/AAMkAGI1AAAt9AHjAAA=/attachments')
    .post({attachment : attachment});

```
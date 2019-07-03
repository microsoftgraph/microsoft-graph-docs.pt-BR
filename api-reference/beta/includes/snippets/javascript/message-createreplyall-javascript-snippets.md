---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bab95dbfa2f2c8b34ac3bb67734ce3858bdbddfe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    message:{
      attachments: [ 
        { 
          @odata.type: "#microsoft.graph.fileAttachment", 
          name: "guidelines.txt", 
          contentBytes: "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    comment: "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll')
    .version('beta')
    .post(message);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 211e3d566240cdc113fbb967a63f31f2fb9b6031
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498259"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.referenceAttachment", 
    name: "Personal pictures", 
    sourceUrl: "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    providerType: "oneDriveConsumer", 
    permission: "Edit", 
    isFolder: "True" 
};

let res = await client.api('/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments')
    .version('beta')
    .post({attachment : attachment});

```
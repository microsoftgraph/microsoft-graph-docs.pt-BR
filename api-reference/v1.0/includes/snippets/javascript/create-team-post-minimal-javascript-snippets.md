---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f249eca84d828faa97baf6f5e90bc64aa52a953
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   template@odata.bind:"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   displayName:"My Sample Team",
   description:"My Sample Team’s Description",
   members:[
      {
         @odata.type:"#microsoft.graph.aadUserConversationMember",
         roles:[
            "owner"
         ],
         user@odata.bind:"https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')"
      }
   ]
};

let res = await client.api('/teams')
    .post(team);

```
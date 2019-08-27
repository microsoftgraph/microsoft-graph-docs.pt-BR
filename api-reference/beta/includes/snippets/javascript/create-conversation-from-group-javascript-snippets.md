---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ba70ea6ded17cfa71f714cc7217629599302cb7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636078"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
    topic:"New head count",
    threads:[
        {
            posts:[
                {
                    body:{
                        contentType:"html",
                        content:"The confirmation will come by the end of the week."
                    },
                    newParticipants:[
                        {
                            emailAddress:{
                                name:"Adele Vance",
                                address:"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
};

let res = await client.api('/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations')
    .version('beta')
    .post(conversation);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: debc87bf6d655a51d7d47edcf51ff2ba214d20ce
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = Content-Type: application/json

{
    topic: {
        source: "text",
        value: "Deployment Approvals Channel",
        webUrl: "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    activityType: "deploymentApprovalRequired",
    previewText: {
        content: "New deployment requires your approval"
    },
    templateParameters: [
        {
            name: "deploymentId",
            value: "6788662"
        }
    ]
};

let res = await client.api('/users/{userId}/teamwork/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```
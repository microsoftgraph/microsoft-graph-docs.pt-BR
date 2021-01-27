---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f010e79490f52097d9c96537e1531c7ef5bedcc
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: "text",
        value: "Deployment Approvals Channel",
        webUrl: "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    activityType: "deploymentApprovalRequired",
    previewText: {
        content: "New deployment requires your approval"
    },
    recipient: {
        @odata.type: "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        userId: "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    templateParameters: [
        {
            name: "deploymentId",
            value: "6788662"
        }
    ]
};

let res = await client.api('/teams/{teamId}/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```
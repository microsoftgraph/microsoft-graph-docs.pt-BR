---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ca46b1a518bb136f740e945ca8acc6170e61f64
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}'
    },
    activityType: 'taskCreated',
    previewText: {
        content: 'New Task Created'
    },
    templateParameters: [
        {
            name: 'taskId',
            value: 'Task 12322'
        }
    ]
};

await client.api('/users/{userId}/teamwork/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```
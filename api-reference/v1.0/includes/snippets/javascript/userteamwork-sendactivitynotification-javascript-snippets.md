---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c25c2e9ff5e9381c14a46f88b091ae09eb3839da
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: 'entityUrl',
        value: 'https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}'
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
    .post(sendActivityNotification);

```
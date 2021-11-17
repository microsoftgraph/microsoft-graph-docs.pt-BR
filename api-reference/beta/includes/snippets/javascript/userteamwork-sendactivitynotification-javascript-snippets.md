---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e43060001a3c48053e5be591d8d0eec81e7c205d38c6dc563394cf2f80040b82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158210"
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
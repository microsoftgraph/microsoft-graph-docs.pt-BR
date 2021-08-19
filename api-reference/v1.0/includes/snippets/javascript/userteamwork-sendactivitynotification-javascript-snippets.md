---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04cda35b2ae15612d6b01de2fb07be6987b41592edb6b7ab68e42e89e5ada9db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102727"
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
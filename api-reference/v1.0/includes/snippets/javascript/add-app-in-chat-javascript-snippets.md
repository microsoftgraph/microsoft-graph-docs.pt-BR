---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e503be50a9da3a308810ee6449fe426f463b9e071274cf432e226adc16c16692
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
'teamsApp@odata.bind':'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a'
};

await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps')
    .post(teamsAppInstallation);

```
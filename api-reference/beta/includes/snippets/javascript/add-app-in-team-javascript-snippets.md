---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 113860a84e07a7c65aeee7536e1933dd6086ae22
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/teams/87654321-0abc-zqf0-321456789q/installedApps')
    .version('beta')
    .post(teamsAppInstallation);

```
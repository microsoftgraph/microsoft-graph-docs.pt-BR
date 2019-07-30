---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cdf130c8e1ec3453affe5c3d179e315963cd15e6
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931678"
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
    .post({teamsAppInstallation : teamsAppInstallation});

```
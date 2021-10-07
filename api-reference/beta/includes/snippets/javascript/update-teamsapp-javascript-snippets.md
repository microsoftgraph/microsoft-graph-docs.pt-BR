---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f3c8ff58aa12e8b3606e6181d816208426862c73daf1085e6a66851919b091c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppDefinition = [Zip file containing a Teams app package];

await client.api('/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true')
    .version('beta')
    .post(teamsAppDefinition);

```
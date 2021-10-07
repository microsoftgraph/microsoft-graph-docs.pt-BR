---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0f870fe4e17d95e08faff7b0ff75b98ee0adf03b805be3d2c44b3fdd17b2319
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsApp = [Zip file containing a Teams app package];

await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .post(teamsApp);

```
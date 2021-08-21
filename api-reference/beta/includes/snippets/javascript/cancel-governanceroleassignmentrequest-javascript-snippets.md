---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00a224c14fbe7594988304f47c12be778ba7ac3f6740410ef044300b0d69d40d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel')
    .version('beta')
    .post();

```
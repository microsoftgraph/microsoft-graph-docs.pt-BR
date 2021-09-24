---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16e7ff2e48ff3ecb61e6b46f83ac575e9e7e8aa94488559216a1ddb49a2ab2f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPC = await client.api('/deviceManagement/virtualEndpoint/cloudPCs/{id}')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 325ed9a8aea3df1574130f8bf6e7b37e71b8d946
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/6a720ba5-7373-463b-bc9f-4cd04b5c6742/channels')
    .version('beta')
    .filter('membershipType eq \'shared\'')
    .get();

```
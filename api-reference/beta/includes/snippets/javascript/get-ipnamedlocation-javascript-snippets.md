---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c131b7e47ddf3e830a7c1e46ed0d5e78264711a
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .get();

```
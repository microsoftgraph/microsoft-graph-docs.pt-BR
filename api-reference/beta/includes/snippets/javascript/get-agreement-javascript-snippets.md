---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4bd3575f8d0bdf4976102f862b4c9353bba475ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreement = await client.api('/identityGovernance/termsOfUse/agreements/{id}')
    .version('beta')
    .expand('files')
    .get();

```
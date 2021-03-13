---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2363039cbe9035d427362cb32e12c0bc11b839bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let policies = await client.api('/trustFramework/policies')
    .version('beta')
    .get();

```
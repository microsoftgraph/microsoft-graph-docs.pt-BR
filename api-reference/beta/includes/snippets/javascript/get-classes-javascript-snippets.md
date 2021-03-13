---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b754d283e380120fe482f49fbe31806c1fee4fd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/classes')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01551a0a1eab36ab1f2631b9fd1ebd739ecc3b93
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/planner/plans')
    .get();

```
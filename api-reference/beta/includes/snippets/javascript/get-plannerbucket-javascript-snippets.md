---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5216a826cb81f5afc87c122537c1f4755cf7c51c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucket = await client.api('/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR')
    .version('beta')
    .get();

```
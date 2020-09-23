---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23b556dffde29f24c2469327d102d5ca291f0401
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/continuousAccessEvaluationPolicy')
    .version('beta')
    .get();

```
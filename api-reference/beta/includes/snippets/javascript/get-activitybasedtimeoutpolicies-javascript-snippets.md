---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa479ff46f8090efd20d64ce84ea792667d99154
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/activityBasedTimeoutPolicies')
    .version('beta')
    .get();

```
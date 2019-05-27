---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03a08f1b39d02ffe9162013cd693ba248b86f7a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Boolean = {
  groupId: "ffffffff-ffff-ffff-ffff-ffffffffffff"
};

let res = await client.api('/groupLifecyclePolicies/renewGroup')
    .version('beta')
    .post(Boolean);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebcc192d9edb2fd9a611c70290be363e9f661eb5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462b6fe2c91155e0a849710e8da766385b52ca26
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/recent')
    .version('beta')
    .get();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4accd33262b044837928ecfbb9492eb79ad1fa37
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 762a6cd49d9354ed591267feb2844c854879b282
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11022')
    .version('beta')
    .delete();

```
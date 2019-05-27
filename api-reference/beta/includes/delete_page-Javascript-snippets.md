---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c994f0260f61a4bf213b34b063d5c208cd2cb63f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437745"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .version('beta')
    .delete();

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 443d5ae391ca2140ea0bd1b70befd3cd615c2928
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}')
    .version('beta')
    .delete();

```
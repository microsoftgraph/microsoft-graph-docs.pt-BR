---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81efc74f2adbc8c5acb7df5d48caf18108df8d0d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .version('beta')
    .post();

```
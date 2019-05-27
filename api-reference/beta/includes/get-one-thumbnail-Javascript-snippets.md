---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02f234567705ab4050a624d8cfd3fcbfa8e92378
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}')
    .version('beta')
    .get();

```
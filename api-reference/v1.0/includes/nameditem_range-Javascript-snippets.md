---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aea6bdfbc04e7b8e564dd489632ed0d90829bfbb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range')
    .post();

```
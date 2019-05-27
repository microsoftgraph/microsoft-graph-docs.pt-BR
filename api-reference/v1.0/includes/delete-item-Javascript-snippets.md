---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 743f327c4adaef1f47eddc4d218f8335eb08bb17
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}')
    .delete();

```
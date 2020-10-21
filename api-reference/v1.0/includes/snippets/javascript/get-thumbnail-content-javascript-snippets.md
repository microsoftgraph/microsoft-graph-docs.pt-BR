---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21363560b6efd0e3e9909158cc012ee433ac9410
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .get();

```